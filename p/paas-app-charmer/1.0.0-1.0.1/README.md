# Comparing `tmp/paas-app-charmer-1.0.0.tar.gz` & `tmp/paas_app_charmer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paas-app-charmer-1.0.0.tar", last modified: Wed Apr  3 23:20:32 2024, max compression
+gzip compressed data, was "paas_app_charmer-1.0.1.tar", last modified: Thu May 23 07:17:20 2024, max compression
```

## Comparing `paas-app-charmer-1.0.0.tar` & `paas_app_charmer-1.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.158874 paas-app-charmer-1.0.0/paas_app_charmer/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.158874 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/charm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/charm_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/observability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/secret_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/wsgi_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/database_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.158874 paas-app-charmer-1.0.0/paas_app_charmer/django/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/django/charm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.154874 paas-app-charmer-1.0.0/paas_app_charmer/django/cos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer/django/cos/grafana_dashboards/
--rw-r--r--   0 runner    (1001) docker     (127)    26134 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/django/cos/grafana_dashboards/django.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer/django/cos/loki_alert_rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/django/cos/loki_alert_rules/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer/django/cos/prometheus_alert_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/django/cos/prometheus_alert_rules/django.rule
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer/flask/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/flask/charm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.158874 paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/grafana_dashboards/
--rw-r--r--   0 runner    (1001) docker     (127)    26108 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/grafana_dashboards/flask.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/loki_alert_rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/loki_alert_rules/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/prometheus_alert_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/prometheus_alert_rules/flask.rule
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/secret_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-03 23:20:32.000000 paas-app-charmer-1.0.0/paas_app_charmer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 23:20:32.000000 paas-app-charmer-1.0.0/paas_app_charmer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:20:32.000000 paas-app-charmer-1.0.0/paas_app_charmer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 23:20:32.000000 paas-app-charmer-1.0.0/paas_app_charmer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 23:20:32.000000 paas-app-charmer-1.0.0/paas_app_charmer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.958857 paas_app_charmer-1.0.1/paas_app_charmer/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.958857 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/charm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/charm_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/observability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/secret_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/wsgi_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/database_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.958857 paas_app_charmer-1.0.1/paas_app_charmer/django/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/django/charm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.954857 paas_app_charmer-1.0.1/paas_app_charmer/django/cos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.958857 paas_app_charmer-1.0.1/paas_app_charmer/django/cos/grafana_dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)    26134 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/django/cos/grafana_dashboards/django.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/paas_app_charmer/django/cos/loki_alert_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/django/cos/loki_alert_rules/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/paas_app_charmer/django/cos/prometheus_alert_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/django/cos/prometheus_alert_rules/django.rule
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/paas_app_charmer/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/flask/charm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.954857 paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/grafana_dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)    26108 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/grafana_dashboards/flask.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/loki_alert_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/loki_alert_rules/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/prometheus_alert_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/prometheus_alert_rules/flask.rule
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/paas_app_charmer/secret_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/paas_app_charmer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-23 07:17:20.000000 paas_app_charmer-1.0.1/paas_app_charmer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-23 07:17:20.000000 paas_app_charmer-1.0.1/paas_app_charmer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:17:20.000000 paas_app_charmer-1.0.1/paas_app_charmer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 07:17:20.000000 paas_app_charmer-1.0.1/paas_app_charmer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 07:17:20.000000 paas_app_charmer-1.0.1/paas_app_charmer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 07:17:20.962857 paas_app_charmer-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-23 07:17:16.000000 paas_app_charmer-1.0.1/setup.py
```

### Comparing `paas-app-charmer-1.0.0/PKG-INFO` & `paas_app_charmer-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paas-app-charmer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Companion library for PaaS app charmer.
 Author-email: Canonical IS DevOps team <is-devops-team@canonical.com>
 Project-URL: Repository, https://github.com/canonical/paas-app-charmer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,27 +14,27 @@
 Requires-Dist: cosl
 Requires-Dist: jsonschema<4.20,>=4.19
 Requires-Dist: ops>=2.6
 Requires-Dist: pydantic==2.6.4
 
 # PaaS App Charmer
 
-Easily deploy and operate your flask applications and associated infrastructure,
+Easily deploy and operate your Flask or Django applications and associated infrastructure,
 such as databases and ingress, using open source tooling. This lets you focus on
 creating applications for your users backed with the confidence that your
 operations are taken care of by world class tooling developed by Canonical, the
 creators of Ubuntu.
 
 Have you ever created an application and then wanted to deploy it for your users
 only to either be forced to use a proprietary public cloud platform or manage
-the deployment and operations yourself? PAAS App Charmer will take your
-application and create an OCI image using rockcraft and operations code using
-charmcraft for you. The full suite of tools is open source so you can see
+the deployment and operations yourself? PaaS App Charmer will take your
+application and create an OCI image using Rockcraft and operations code using
+Charmcraft for you. The full suite of tools is open source so you can see
 exactly how it works and even contribute! After creating the app charm and
-image, you can then deploy your application into any kubernetes cluster using
-juju. Need a database? Using juju you can deploy a range of popular open source
-databases, such as [postgreSQL](https://charmhub.io/postgresql) or
+image, you can then deploy your application into any Kubernetes cluster using
+Juju. Need a database? Using Juju you can deploy a range of popular open source
+databases, such as [PostgreSQL](https://charmhub.io/postgresql) or
 [MySQL](https://charmhub.io/mysql), and integrate them with your application
-with a few commands. Need an ingress to serve traffic? Use juju to deploy and
-integrate a range of ingress, such as
-[traefik](https://charmhub.io/traefik-k8s), and expose your application to
+with a few commands. Need an ingress to serve traffic? Use Juju to deploy and
+integrate a range of ingresses, such as
+[Traefik](https://charmhub.io/traefik-k8s), and expose your application to
 external traffic in seconds.
```

### Comparing `paas-app-charmer-1.0.0/README.md` & `paas_app_charmer-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # PaaS App Charmer
 
-Easily deploy and operate your flask applications and associated infrastructure,
+Easily deploy and operate your Flask or Django applications and associated infrastructure,
 such as databases and ingress, using open source tooling. This lets you focus on
 creating applications for your users backed with the confidence that your
 operations are taken care of by world class tooling developed by Canonical, the
 creators of Ubuntu.
 
 Have you ever created an application and then wanted to deploy it for your users
 only to either be forced to use a proprietary public cloud platform or manage
-the deployment and operations yourself? PAAS App Charmer will take your
-application and create an OCI image using rockcraft and operations code using
-charmcraft for you. The full suite of tools is open source so you can see
+the deployment and operations yourself? PaaS App Charmer will take your
+application and create an OCI image using Rockcraft and operations code using
+Charmcraft for you. The full suite of tools is open source so you can see
 exactly how it works and even contribute! After creating the app charm and
-image, you can then deploy your application into any kubernetes cluster using
-juju. Need a database? Using juju you can deploy a range of popular open source
-databases, such as [postgreSQL](https://charmhub.io/postgresql) or
+image, you can then deploy your application into any Kubernetes cluster using
+Juju. Need a database? Using Juju you can deploy a range of popular open source
+databases, such as [PostgreSQL](https://charmhub.io/postgresql) or
 [MySQL](https://charmhub.io/mysql), and integrate them with your application
-with a few commands. Need an ingress to serve traffic? Use juju to deploy and
-integrate a range of ingress, such as
-[traefik](https://charmhub.io/traefik-k8s), and expose your application to
+with a few commands. Need an ingress to serve traffic? Use Juju to deploy and
+integrate a range of ingresses, such as
+[Traefik](https://charmhub.io/traefik-k8s), and expose your application to
 external traffic in seconds.
```

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/charm.py` & `paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/charm.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             )
             self.framework.observe(
                 self.on[database_requirer.relation_name].relation_broken,
                 getattr(self, f"_on_{database}_database_relation_broken"),
             )
 
     def _on_config_changed(self, _event: ops.EventBase) -> None:
-        """Configure the flask pebble service layer.
+        """Configure the application pebble service layer.
 
         Args:
             _event: the config-changed event that triggers this callback function.
         """
         self.restart()
 
     def _on_rotate_secret_key_action(self, event: ops.ActionEvent) -> None:
@@ -143,15 +143,15 @@
         Args:
             event: the action event that trigger this callback.
         """
         if not self.unit.is_leader():
             event.fail("only leader unit can rotate secret key")
             return
         if not self._secret_storage.is_initialized:
-            event.fail("flask charm is still initializing")
+            event.fail("charm is still initializing")
             return
         self._secret_storage.reset_secret_key()
         event.set_results({"status": "success"})
         self.restart()
 
     def _on_secret_storage_relation_changed(self, _event: ops.RelationEvent) -> None:
         """Handle the secret-storage-relation-changed event.
@@ -186,61 +186,64 @@
         if not self._charm_state.is_secret_storage_ready:
             logger.info("secret storage is not initialized")
             self._update_app_and_unit_status(ops.WaitingStatus("Waiting for peer integration"))
             return False
         return True
 
     def restart(self) -> None:
-        """Restart or start the flask service if not started with the latest configuration."""
+        """Restart or start the service if not started with the latest configuration."""
         if not self.is_ready():
             return
         try:
+            self._update_app_and_unit_status(
+                ops.MaintenanceStatus("Preparing service for restart")
+            )
             self._wsgi_app.restart()
         except CharmConfigInvalidError as exc:
             self._update_app_and_unit_status(ops.BlockedStatus(exc.msg))
             return
         self._update_app_and_unit_status(ops.ActiveStatus())
 
     def _on_update_status(self, _: ops.HookEvent) -> None:
         """Handle the update-status event."""
         if self._database_migration.get_status() == DatabaseMigrationStatus.FAILED:
             self.restart()
 
     def _on_mysql_database_database_created(self, _event: DatabaseRequiresEvent) -> None:
-        """Handle the mysql's database-created event."""
+        """Handle mysql's database-created event."""
         self.restart()
 
     def _on_mysql_database_endpoints_changed(self, _event: DatabaseRequiresEvent) -> None:
-        """Handle the mysql's endpoints-changed event."""
+        """Handle mysql's endpoints-changed event."""
         self.restart()
 
     def _on_mysql_database_relation_broken(self, _event: ops.RelationBrokenEvent) -> None:
-        """Handle the mysql's relation-broken event."""
+        """Handle mysql's relation-broken event."""
         self.restart()
 
     def _on_postgresql_database_database_created(self, _event: DatabaseRequiresEvent) -> None:
-        """Handle the postgresql's database-created event."""
+        """Handle postgresql's database-created event."""
         self.restart()
 
     def _on_postgresql_database_endpoints_changed(self, _event: DatabaseRequiresEvent) -> None:
-        """Handle the mysql's endpoints-changed event."""
+        """Handle mysql's endpoints-changed event."""
         self.restart()
 
     def _on_postgresql_database_relation_broken(self, _event: ops.RelationBrokenEvent) -> None:
-        """Handle the postgresql's relation-broken event."""
+        """Handle postgresql's relation-broken event."""
         self.restart()
 
     def _on_mongodb_database_database_created(self, _event: DatabaseRequiresEvent) -> None:
-        """Handle the mongodb's database-created event."""
+        """Handle mongodb's database-created event."""
         self.restart()
 
     def _on_mongodb_database_endpoints_changed(self, _event: DatabaseRequiresEvent) -> None:
-        """Handle the mysql's endpoints-changed event."""
+        """Handle mysql's endpoints-changed event."""
         self.restart()
 
     def _on_mongodb_database_relation_broken(self, _event: ops.RelationBrokenEvent) -> None:
-        """Handle the postgresql's relation-broken event."""
+        """Handle postgresql's relation-broken event."""
         self.restart()
 
     def _on_redis_relation_updated(self, _event: DatabaseRequiresEvent) -> None:
-        """Handle the redis's database-created event."""
+        """Handle redis's database-created event."""
         self.restart()
```

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/charm_state.py` & `paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/charm_state.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/observability.py` & `paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/observability.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/secret_storage.py` & `paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/secret_storage.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/webserver.py` & `paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/webserver.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/wsgi_app.py` & `paas_app_charmer-1.0.1/paas_app_charmer/_gunicorn/wsgi_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,18 @@
         migration_command = None
         app_dir = self._charm_state.app_dir
         if self._container.exists(app_dir / "migrate"):
             migration_command = [str((app_dir / "migrate").absolute())]
         if self._container.exists(app_dir / "migrate.sh"):
             migration_command = ["bash", "-eo", "pipefail", "migrate.sh"]
         if self._container.exists(app_dir / "migrate.py"):
-            migration_command = ["python", "migrate.py"]
+            migration_command = ["python3", "migrate.py"]
+        if self._container.exists(app_dir / "manage.py"):
+            # Django migrate command
+            migration_command = ["python3", "manage.py", "migrate"]
         if migration_command:
             self._database_migration.run(
                 command=migration_command,
                 environment=self.gen_environment(),
                 working_dir=app_dir,
                 user=self._charm_state.user,
                 group=self._charm_state.group,
```

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer/database_migration.py` & `paas_app_charmer-1.0.1/paas_app_charmer/database_migration.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer/databases.py` & `paas_app_charmer-1.0.1/paas_app_charmer/databases.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer/django/charm.py` & `paas_app_charmer-1.0.1/paas_app_charmer/django/charm.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         Raises:
             CharmConfigInvalidError: if charm config is not valid.
         """
         django_config: dict[str, typing.Any] = {
             "debug": self.config.get("django-debug"),
             "secret_key": self.config.get("django-secret-key"),
         }
-        allowed_hosts = self.config.get("django-allowed-hosts", "")
+        allowed_hosts = str(self.config.get("django-allowed-hosts", ""))
         if allowed_hosts.strip():
             django_config["allowed_hosts"] = [h.strip() for h in allowed_hosts.split(",")]
         else:
             django_config["allowed_hosts"] = []
         try:
             return DjangoConfig.model_validate(django_config)
         except ValidationError as exc:
@@ -95,15 +95,15 @@
             event: the action event object.
         """
         if not self.is_ready():
             event.fail("django-app container is not ready")
         try:
             password = secrets.token_urlsafe(16)
             self._container.exec(
-                ["python", "manage.py", "createsuperuser", "--noinput"],
+                ["python3", "manage.py", "createsuperuser", "--noinput"],
                 environment={
                     "DJANGO_SUPERUSER_PASSWORD": password,
                     "DJANGO_SUPERUSER_USERNAME": event.params["username"],
                     "DJANGO_SUPERUSER_EMAIL": event.params["email"],
                     **self._wsgi_app.gen_environment(),
                 },
                 combine_stderr=True,
```

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer/django/cos/grafana_dashboards/django.json` & `paas_app_charmer-1.0.1/paas_app_charmer/django/cos/grafana_dashboards/django.json`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer/exceptions.py` & `paas_app_charmer-1.0.1/paas_app_charmer/exceptions.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer/flask/charm.py` & `paas_app_charmer-1.0.1/paas_app_charmer/flask/charm.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/grafana_dashboards/flask.json` & `paas_app_charmer-1.0.1/paas_app_charmer/flask/cos/grafana_dashboards/flask.json`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer/helpers.py` & `paas_app_charmer-1.0.1/paas_app_charmer/helpers.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer/secret_storage.py` & `paas_app_charmer-1.0.1/paas_app_charmer/secret_storage.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer.egg-info/PKG-INFO` & `paas_app_charmer-1.0.1/paas_app_charmer.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paas-app-charmer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Companion library for PaaS app charmer.
 Author-email: Canonical IS DevOps team <is-devops-team@canonical.com>
 Project-URL: Repository, https://github.com/canonical/paas-app-charmer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,27 +14,27 @@
 Requires-Dist: cosl
 Requires-Dist: jsonschema<4.20,>=4.19
 Requires-Dist: ops>=2.6
 Requires-Dist: pydantic==2.6.4
 
 # PaaS App Charmer
 
-Easily deploy and operate your flask applications and associated infrastructure,
+Easily deploy and operate your Flask or Django applications and associated infrastructure,
 such as databases and ingress, using open source tooling. This lets you focus on
 creating applications for your users backed with the confidence that your
 operations are taken care of by world class tooling developed by Canonical, the
 creators of Ubuntu.
 
 Have you ever created an application and then wanted to deploy it for your users
 only to either be forced to use a proprietary public cloud platform or manage
-the deployment and operations yourself? PAAS App Charmer will take your
-application and create an OCI image using rockcraft and operations code using
-charmcraft for you. The full suite of tools is open source so you can see
+the deployment and operations yourself? PaaS App Charmer will take your
+application and create an OCI image using Rockcraft and operations code using
+Charmcraft for you. The full suite of tools is open source so you can see
 exactly how it works and even contribute! After creating the app charm and
-image, you can then deploy your application into any kubernetes cluster using
-juju. Need a database? Using juju you can deploy a range of popular open source
-databases, such as [postgreSQL](https://charmhub.io/postgresql) or
+image, you can then deploy your application into any Kubernetes cluster using
+Juju. Need a database? Using Juju you can deploy a range of popular open source
+databases, such as [PostgreSQL](https://charmhub.io/postgresql) or
 [MySQL](https://charmhub.io/mysql), and integrate them with your application
-with a few commands. Need an ingress to serve traffic? Use juju to deploy and
-integrate a range of ingress, such as
-[traefik](https://charmhub.io/traefik-k8s), and expose your application to
+with a few commands. Need an ingress to serve traffic? Use Juju to deploy and
+integrate a range of ingresses, such as
+[Traefik](https://charmhub.io/traefik-k8s), and expose your application to
 external traffic in seconds.
```

### Comparing `paas-app-charmer-1.0.0/paas_app_charmer.egg-info/SOURCES.txt` & `paas_app_charmer-1.0.1/paas_app_charmer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-1.0.0/pyproject.toml` & `paas_app_charmer-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright 2024 Canonical Ltd.
 # See LICENSE file for licensing details.
 [project]
 name = "paas-app-charmer"
-version = "1.0.0"
+version = "1.0.1"
 description = "Companion library for PaaS app charmer."
 readme = "README.md"
 authors = [
     {name = "Canonical IS DevOps team", email="is-devops-team@canonical.com"},
 ]
 requires-python = ">=3.10"
 dynamic = ["dependencies"]
```

