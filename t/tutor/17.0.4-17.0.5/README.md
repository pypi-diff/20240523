# Comparing `tmp/tutor-17.0.4.tar.gz` & `tmp/tutor-17.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-17.0.4.tar", last modified: Thu Apr 11 09:44:08 2024, max compression
+gzip compressed data, was "tutor-17.0.5.tar", last modified: Thu May 23 17:42:40 2024, max compression
```

## Comparing `tutor-17.0.4.tar` & `tutor-17.0.5.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.376849 tutor-17.0.4/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2024-04-11 09:43:37.000000 tutor-17.0.4/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)      150 2024-04-11 09:43:37.000000 tutor-17.0.4/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     6528 2024-04-11 09:44:08.376849 tutor-17.0.4/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     4566 2024-04-11 09:43:37.000000 tutor-17.0.4/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       50 2024-04-11 09:43:37.000000 tutor-17.0.4/pyproject.toml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.353516 tutor-17.0.4/requirements/
--rw-r--r--   0 ci        (1000) ci        (1000)      159 2024-04-11 09:43:37.000000 tutor-17.0.4/requirements/base.in
--rw-r--r--   0 ci        (1000) ci        (1000)     4775 2024-04-11 09:43:37.000000 tutor-17.0.4/requirements/dev.txt
--rw-r--r--   0 ci        (1000) ci        (1000)      433 2024-04-11 09:43:37.000000 tutor-17.0.4/requirements/plugins.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2024-04-11 09:44:08.376849 tutor-17.0.4/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     2580 2024-04-11 09:43:37.000000 tutor-17.0.4/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.353516 tutor-17.0.4/tests/
--rw-r--r--   0 ci        (1000) ci        (1000)     2067 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_bindmount.py
--rw-r--r--   0 ci        (1000) ci        (1000)     4172 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_config.py
--rw-r--r--   0 ci        (1000) ci        (1000)    15988 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_env.py
--rw-r--r--   0 ci        (1000) ci        (1000)     3063 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_plugin_indexes.py
--rw-r--r--   0 ci        (1000) ci        (1000)      539 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_plugins.py
--rw-r--r--   0 ci        (1000) ci        (1000)     8281 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_plugins_v0.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2588 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_serialize.py
--rw-r--r--   0 ci        (1000) ci        (1000)    11633 2024-04-11 09:43:37.000000 tutor-17.0.4/tests/test_utils.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.356849 tutor-17.0.4/tutor/
--rw-r--r--   0 ci        (1000) ci        (1000)     1159 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2549 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/bindmount.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.360182 tutor-17.0.4/tutor/commands/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/commands/__init__.py
--rwxr-xr-x   0 ci        (1000) ci        (1000)     4219 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/cli.py
--rw-r--r--   0 ci        (1000) ci        (1000)    15893 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/compose.py
--rw-r--r--   0 ci        (1000) ci        (1000)     7390 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/config.py
--rw-r--r--   0 ci        (1000) ci        (1000)      794 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/context.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2240 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/dev.py
--rw-r--r--   0 ci        (1000) ci        (1000)    11114 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/images.py
--rw-r--r--   0 ci        (1000) ci        (1000)    13579 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/jobs.py
--rw-r--r--   0 ci        (1000) ci        (1000)    21075 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/k8s.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1772 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/local.py
--rw-r--r--   0 ci        (1000) ci        (1000)     4446 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/mounts.py
--rw-r--r--   0 ci        (1000) ci        (1000)      741 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/params.py
--rw-r--r--   0 ci        (1000) ci        (1000)    13420 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/plugins.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.360182 tutor-17.0.4/tutor/commands/upgrade/
--rw-r--r--   0 ci        (1000) ci        (1000)      213 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/upgrade/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2082 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/upgrade/common.py
--rw-r--r--   0 ci        (1000) ci        (1000)     6117 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/upgrade/compose.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5755 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/commands/upgrade/k8s.py
--rw-r--r--   0 ci        (1000) ci        (1000)    10932 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.360182 tutor-17.0.4/tutor/core/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/core/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.363516 tutor-17.0.4/tutor/core/hooks/
--rw-r--r--   0 ci        (1000) ci        (1000)      292 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/core/hooks/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5707 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/core/hooks/actions.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2929 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/core/hooks/contexts.py
--rw-r--r--   0 ci        (1000) ci        (1000)     9006 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/core/hooks/filters.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1007 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/core/hooks/priorities.py
--rw-r--r--   0 ci        (1000) ci        (1000)    17927 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/env.py
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/exceptions.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1213 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/fmt.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.363516 tutor-17.0.4/tutor/hooks/
--rw-r--r--   0 ci        (1000) ci        (1000)     1195 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/hooks/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)    27389 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/hooks/catalog.py
--rw-r--r--   0 ci        (1000) ci        (1000)      673 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/images.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5182 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/interactive.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.363516 tutor-17.0.4/tutor/plugins/
--rw-r--r--   0 ci        (1000) ci        (1000)     3484 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/plugins/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      548 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/plugins/base.py
--rw-r--r--   0 ci        (1000) ci        (1000)     6935 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/plugins/indexes.py
--rw-r--r--   0 ci        (1000) ci        (1000)     4582 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/plugins/openedx.py
--rw-r--r--   0 ci        (1000) ci        (1000)    15220 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/plugins/v0.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2482 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/plugins/v1.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/py.typed
--rw-r--r--   0 ci        (1000) ci        (1000)     2180 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/serialize.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1385 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/tasks.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.363516 tutor-17.0.4/tutor/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.346849 tutor-17.0.4/tutor/templates/apps/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.363516 tutor-17.0.4/tutor/templates/apps/caddy/
--rw-r--r--   0 ci        (1000) ci        (1000)     1989 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/caddy/Caddyfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.363516 tutor-17.0.4/tutor/templates/apps/openedx/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.366849 tutor-17.0.4/tutor/templates/apps/openedx/config/
--rw-r--r--   0 ci        (1000) ci        (1000)     1542 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/config/cms.env.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1787 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/config/lms.env.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.366849 tutor-17.0.4/tutor/templates/apps/openedx/config/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)      743 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/config/partials/auth.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.346849 tutor-17.0.4/tutor/templates/apps/openedx/settings/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.366849 tutor-17.0.4/tutor/templates/apps/openedx/settings/cms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/cms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      661 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/cms/development.py
--rw-r--r--   0 ci        (1000) ci        (1000)      529 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/cms/production.py
--rw-r--r--   0 ci        (1000) ci        (1000)       91 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/cms/test.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/apps/openedx/settings/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/lms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1132 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/lms/development.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1039 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/lms/production.py
--rw-r--r--   0 ci        (1000) ci        (1000)       91 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/lms/test.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)    10504 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/common_all.py
--rw-r--r--   0 ci        (1000) ci        (1000)      961 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/common_cms.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1450 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/common_lms.py
--rw-r--r--   0 ci        (1000) ci        (1000)      105 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/common_test.py
--rw-r--r--   0 ci        (1000) ci        (1000)       78 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/openedx/uwsgi.ini
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/apps/permissions/
--rw-r--r--   0 ci        (1000) ci        (1000)      380 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/permissions/setowners.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/apps/redis/
--rw-r--r--   0 ci        (1000) ci        (1000)     1008 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/apps/redis/redis.conf
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.350182 tutor-17.0.4/tutor/templates/build/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/build/openedx/
--rw-r--r--   0 ci        (1000) ci        (1000)    12940 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/build/openedx/bin/
--rwxr-xr-x   0 ci        (1000) ci        (1000)     7042 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/bin/openedx-assets
--rwxr-xr-x   0 ci        (1000) ci        (1000)      116 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/bin/reload-uwsgi
--rw-r--r--   0 ci        (1000) ci        (1000)     2329 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/bin/site-configuration
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/build/openedx/locale/
--rw-r--r--   0 ci        (1000) ci        (1000)      438 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/locale/customlocales.md
--rw-r--r--   0 ci        (1000) ci        (1000)       30 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/revisions.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/build/openedx/settings/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/build/openedx/settings/cms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/cms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      317 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/cms/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)       56 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/cms/i18n.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.370183 tutor-17.0.4/tutor/templates/build/openedx/settings/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-11 09:43:39.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/lms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      306 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/lms/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)       56 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/lms/i18n.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.373516 tutor-17.0.4/tutor/templates/build/openedx/settings/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)      441 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/partials/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)      420 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/partials/i18n.py
--rw-r--r--   0 ci        (1000) ci        (1000)      262 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/settings/uwsgi.ini
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.373516 tutor-17.0.4/tutor/templates/build/openedx/themes/
--rw-r--r--   0 ci        (1000) ci        (1000)       75 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/openedx/themes/README
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.373516 tutor-17.0.4/tutor/templates/build/permissions/
--rw-r--r--   0 ci        (1000) ci        (1000)      189 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/permissions/Dockerfile
--rw-r--r--   0 ci        (1000) ci        (1000)      302 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/build/permissions/setowner.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.373516 tutor-17.0.4/tutor/templates/config/
--rw-r--r--   0 ci        (1000) ci        (1000)      518 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/config/base.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2901 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/config/defaults.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.373516 tutor-17.0.4/tutor/templates/dev/
--rw-r--r--   0 ci        (1000) ci        (1000)      799 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/dev/docker-compose.jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1353 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/dev/docker-compose.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.350182 tutor-17.0.4/tutor/templates/jobs/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.373516 tutor-17.0.4/tutor/templates/jobs/init/
--rw-r--r--   0 ci        (1000) ci        (1000)      781 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/jobs/init/cms.sh
--rw-r--r--   0 ci        (1000) ci        (1000)     1807 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/jobs/init/lms.sh
--rw-r--r--   0 ci        (1000) ci        (1000)     1569 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/jobs/init/mounted-directories.sh
--rw-r--r--   0 ci        (1000) ci        (1000)     1455 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/jobs/init/mysql.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.373516 tutor-17.0.4/tutor/templates/k8s/
--rw-r--r--   0 ci        (1000) ci        (1000)    13048 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/k8s/deployments.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2090 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/k8s/jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)      125 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/k8s/namespace.yml
--rw-r--r--   0 ci        (1000) ci        (1000)       28 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/k8s/override.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2465 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/k8s/services.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1428 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/k8s/volumes.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2142 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/kustomization.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.376849 tutor-17.0.4/tutor/templates/local/
--rw-r--r--   0 ci        (1000) ci        (1000)     2207 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/local/docker-compose.jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1017 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/local/docker-compose.prod.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     6608 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/local/docker-compose.yml
--rw-r--r--   0 ci        (1000) ci        (1000)       19 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/templates/version
--rw-r--r--   0 ci        (1000) ci        (1000)     1327 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/types.py
--rw-r--r--   0 ci        (1000) ci        (1000)    10766 2024-04-11 09:43:37.000000 tutor-17.0.4/tutor/utils.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-11 09:44:08.360182 tutor-17.0.4/tutor.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     6528 2024-04-11 09:44:08.000000 tutor-17.0.4/tutor.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     4103 2024-04-11 09:44:08.000000 tutor-17.0.4/tutor.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2024-04-11 09:44:08.000000 tutor-17.0.4/tutor.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       51 2024-04-11 09:44:08.000000 tutor-17.0.4/tutor.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)     1840 2024-04-11 09:44:08.000000 tutor-17.0.4/tutor.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        6 2024-04-11 09:44:08.000000 tutor-17.0.4/tutor.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.860028 tutor-17.0.5/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2024-05-23 17:41:35.000000 tutor-17.0.5/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)      150 2024-05-23 17:41:35.000000 tutor-17.0.5/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     6528 2024-05-23 17:42:40.853361 tutor-17.0.5/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     4566 2024-05-23 17:41:35.000000 tutor-17.0.5/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2024-05-23 17:41:35.000000 tutor-17.0.5/pyproject.toml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.136690 tutor-17.0.5/requirements/
+-rw-r--r--   0 ci        (1000) ci        (1000)      159 2024-05-23 17:41:35.000000 tutor-17.0.5/requirements/base.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     4775 2024-05-23 17:41:35.000000 tutor-17.0.5/requirements/dev.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)      433 2024-05-23 17:41:35.000000 tutor-17.0.5/requirements/plugins.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2024-05-23 17:42:40.860028 tutor-17.0.5/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     2580 2024-05-23 17:41:35.000000 tutor-17.0.5/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.190024 tutor-17.0.5/tests/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2067 2024-05-23 17:41:35.000000 tutor-17.0.5/tests/test_bindmount.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     4172 2024-05-23 17:41:35.000000 tutor-17.0.5/tests/test_config.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    15988 2024-05-23 17:41:35.000000 tutor-17.0.5/tests/test_env.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     3063 2024-05-23 17:41:35.000000 tutor-17.0.5/tests/test_plugin_indexes.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      539 2024-05-23 17:41:35.000000 tutor-17.0.5/tests/test_plugins.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     8281 2024-05-23 17:41:35.000000 tutor-17.0.5/tests/test_plugins_v0.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2588 2024-05-23 17:41:35.000000 tutor-17.0.5/tests/test_serialize.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    11633 2024-05-23 17:41:35.000000 tutor-17.0.5/tests/test_utils.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.270024 tutor-17.0.5/tutor/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1159 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-05-23 17:41:36.000000 tutor-17.0.5/tutor/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2549 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/bindmount.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.433359 tutor-17.0.5/tutor/commands/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-05-23 17:41:36.000000 tutor-17.0.5/tutor/commands/__init__.py
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     4219 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/cli.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    15893 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/compose.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     7390 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/config.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      794 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/context.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2240 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/dev.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    11114 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/images.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    13579 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/jobs.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    21075 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/k8s.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1772 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/local.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     4446 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/mounts.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      741 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/params.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    13420 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/plugins.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.466692 tutor-17.0.5/tutor/commands/upgrade/
+-rw-r--r--   0 ci        (1000) ci        (1000)      213 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/upgrade/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2082 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/upgrade/common.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     6117 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/upgrade/compose.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5755 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/commands/upgrade/k8s.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    11022 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.473359 tutor-17.0.5/tutor/core/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-05-23 17:41:36.000000 tutor-17.0.5/tutor/core/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.503359 tutor-17.0.5/tutor/core/hooks/
+-rw-r--r--   0 ci        (1000) ci        (1000)      292 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/core/hooks/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5707 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/core/hooks/actions.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2929 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/core/hooks/contexts.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     9006 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/core/hooks/filters.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1007 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/core/hooks/priorities.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    17927 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/env.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/exceptions.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1213 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/fmt.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.513359 tutor-17.0.5/tutor/hooks/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1195 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/hooks/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    28162 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/hooks/catalog.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      673 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/images.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5182 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/interactive.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.583360 tutor-17.0.5/tutor/plugins/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3484 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/plugins/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      548 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/plugins/base.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     6935 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/plugins/indexes.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     4582 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/plugins/openedx.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    15220 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/plugins/v0.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2482 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/plugins/v1.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-05-23 17:41:36.000000 tutor-17.0.5/tutor/py.typed
+-rw-r--r--   0 ci        (1000) ci        (1000)     2180 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/serialize.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1385 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/tasks.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.593360 tutor-17.0.5/tutor/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.060023 tutor-17.0.5/tutor/templates/apps/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.596693 tutor-17.0.5/tutor/templates/apps/caddy/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2035 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/caddy/Caddyfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.600026 tutor-17.0.5/tutor/templates/apps/openedx/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.610026 tutor-17.0.5/tutor/templates/apps/openedx/config/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1542 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/openedx/config/cms.env.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1787 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/openedx/config/lms.env.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.613360 tutor-17.0.5/tutor/templates/apps/openedx/config/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)      743 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/openedx/config/partials/auth.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.060023 tutor-17.0.5/tutor/templates/apps/openedx/settings/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.626693 tutor-17.0.5/tutor/templates/apps/openedx/settings/cms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-05-23 17:41:36.000000 tutor-17.0.5/tutor/templates/apps/openedx/settings/cms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      661 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/openedx/settings/cms/development.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      529 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/openedx/settings/cms/production.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       91 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/openedx/settings/cms/test.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.640027 tutor-17.0.5/tutor/templates/apps/openedx/settings/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-05-23 17:41:36.000000 tutor-17.0.5/tutor/templates/apps/openedx/settings/lms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1132 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/openedx/settings/lms/development.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1039 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/openedx/settings/lms/production.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       91 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/openedx/settings/lms/test.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.666694 tutor-17.0.5/tutor/templates/apps/openedx/settings/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)    10504 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/openedx/settings/partials/common_all.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      961 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/openedx/settings/partials/common_cms.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1450 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/openedx/settings/partials/common_lms.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      105 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/openedx/settings/partials/common_test.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       78 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/openedx/uwsgi.ini
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.673360 tutor-17.0.5/tutor/templates/apps/permissions/
+-rw-r--r--   0 ci        (1000) ci        (1000)      380 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/permissions/setowners.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.676694 tutor-17.0.5/tutor/templates/apps/redis/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1008 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/apps/redis/redis.conf
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.066690 tutor-17.0.5/tutor/templates/build/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.696694 tutor-17.0.5/tutor/templates/build/openedx/
+-rw-r--r--   0 ci        (1000) ci        (1000)    13315 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/openedx/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.713361 tutor-17.0.5/tutor/templates/build/openedx/bin/
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     7042 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/openedx/bin/openedx-assets
+-rwxr-xr-x   0 ci        (1000) ci        (1000)      116 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/openedx/bin/reload-uwsgi
+-rw-r--r--   0 ci        (1000) ci        (1000)     2329 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/openedx/bin/site-configuration
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.720027 tutor-17.0.5/tutor/templates/build/openedx/locale/
+-rw-r--r--   0 ci        (1000) ci        (1000)      438 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/openedx/locale/customlocales.md
+-rw-r--r--   0 ci        (1000) ci        (1000)       30 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/openedx/revisions.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.723361 tutor-17.0.5/tutor/templates/build/openedx/settings/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.730027 tutor-17.0.5/tutor/templates/build/openedx/settings/cms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-05-23 17:41:36.000000 tutor-17.0.5/tutor/templates/build/openedx/settings/cms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      317 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/openedx/settings/cms/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       56 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/openedx/settings/cms/i18n.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.740027 tutor-17.0.5/tutor/templates/build/openedx/settings/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-05-23 17:41:36.000000 tutor-17.0.5/tutor/templates/build/openedx/settings/lms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      306 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/openedx/settings/lms/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       56 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/openedx/settings/lms/i18n.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.746694 tutor-17.0.5/tutor/templates/build/openedx/settings/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)      441 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/openedx/settings/partials/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      420 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/openedx/settings/partials/i18n.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      262 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/openedx/settings/uwsgi.ini
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.750028 tutor-17.0.5/tutor/templates/build/openedx/themes/
+-rw-r--r--   0 ci        (1000) ci        (1000)       75 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/openedx/themes/README
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.760028 tutor-17.0.5/tutor/templates/build/permissions/
+-rw-r--r--   0 ci        (1000) ci        (1000)      189 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/permissions/Dockerfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      302 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/build/permissions/setowner.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.770027 tutor-17.0.5/tutor/templates/config/
+-rw-r--r--   0 ci        (1000) ci        (1000)      518 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/config/base.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2901 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/config/defaults.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.776694 tutor-17.0.5/tutor/templates/dev/
+-rw-r--r--   0 ci        (1000) ci        (1000)      799 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/dev/docker-compose.jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1353 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/dev/docker-compose.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.070023 tutor-17.0.5/tutor/templates/jobs/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.793361 tutor-17.0.5/tutor/templates/jobs/init/
+-rw-r--r--   0 ci        (1000) ci        (1000)      781 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/jobs/init/cms.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)     1807 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/jobs/init/lms.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)     1569 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/jobs/init/mounted-directories.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)     1455 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/jobs/init/mysql.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.830028 tutor-17.0.5/tutor/templates/k8s/
+-rw-r--r--   0 ci        (1000) ci        (1000)    13048 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/k8s/deployments.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2090 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/k8s/jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)      125 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/k8s/namespace.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)       28 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/k8s/override.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2465 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/k8s/services.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1428 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/k8s/volumes.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2142 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/kustomization.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.843361 tutor-17.0.5/tutor/templates/local/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2207 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/local/docker-compose.jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1017 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/local/docker-compose.prod.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     6608 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/local/docker-compose.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)       19 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/templates/version
+-rw-r--r--   0 ci        (1000) ci        (1000)     1327 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/types.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    10766 2024-05-23 17:41:35.000000 tutor-17.0.5/tutor/utils.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-05-23 17:42:40.306691 tutor-17.0.5/tutor.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     6528 2024-05-23 17:42:39.000000 tutor-17.0.5/tutor.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     4103 2024-05-23 17:42:39.000000 tutor-17.0.5/tutor.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2024-05-23 17:42:39.000000 tutor-17.0.5/tutor.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       51 2024-05-23 17:42:39.000000 tutor-17.0.5/tutor.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)     1840 2024-05-23 17:42:39.000000 tutor-17.0.5/tutor.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        6 2024-05-23 17:42:39.000000 tutor-17.0.5/tutor.egg-info/top_level.txt
```

### Comparing `tutor-17.0.4/LICENSE.txt` & `tutor-17.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/PKG-INFO` & `tutor-17.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor
-Version: 17.0.4
+Version: 17.0.5
 Summary: The Docker-based Open edX distribution designed for peace of mind
 Home-page: https://docs.tutor.edly.io/
 Author: Edly
 Author-email: hello@edly.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.edly.io/
 Project-URL: Code, https://github.com/overhangio/tutor
```

### Comparing `tutor-17.0.4/README.rst` & `tutor-17.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/requirements/dev.txt` & `tutor-17.0.5/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/setup.py` & `tutor-17.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tests/test_bindmount.py` & `tutor-17.0.5/tests/test_bindmount.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tests/test_config.py` & `tutor-17.0.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tests/test_env.py` & `tutor-17.0.5/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tests/test_plugin_indexes.py` & `tutor-17.0.5/tests/test_plugin_indexes.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tests/test_plugins.py` & `tutor-17.0.5/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tests/test_plugins_v0.py` & `tutor-17.0.5/tests/test_plugins_v0.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tests/test_serialize.py` & `tutor-17.0.5/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tests/test_utils.py` & `tutor-17.0.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/__about__.py` & `tutor-17.0.5/tutor/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 # Increment this version number to trigger a new release. See
 # docs/tutor.html#versioning for information on the versioning scheme.
-__version__ = "17.0.4"
+__version__ = "17.0.5"
 
 # The version suffix will be appended to the actual version, separated by a
 # dash. Use this suffix to differentiate between the actual released version and
 # the versions from other branches. For instance: set the suffix to "nightly" in
 # the nightly branch.
 # The suffix is cleanly separated from the __version__ in this module to avoid
 # conflicts when merging branches.
```

### Comparing `tutor-17.0.4/tutor/bindmount.py` & `tutor-17.0.5/tutor/bindmount.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/commands/cli.py` & `tutor-17.0.5/tutor/commands/cli.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/commands/compose.py` & `tutor-17.0.5/tutor/commands/compose.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/commands/config.py` & `tutor-17.0.5/tutor/commands/config.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/commands/context.py` & `tutor-17.0.5/tutor/commands/context.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/commands/dev.py` & `tutor-17.0.5/tutor/commands/dev.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/commands/images.py` & `tutor-17.0.5/tutor/commands/images.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/commands/jobs.py` & `tutor-17.0.5/tutor/commands/jobs.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/commands/k8s.py` & `tutor-17.0.5/tutor/commands/k8s.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/commands/local.py` & `tutor-17.0.5/tutor/commands/local.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/commands/mounts.py` & `tutor-17.0.5/tutor/commands/mounts.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/commands/params.py` & `tutor-17.0.5/tutor/commands/params.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/commands/plugins.py` & `tutor-17.0.5/tutor/commands/plugins.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/commands/upgrade/common.py` & `tutor-17.0.5/tutor/commands/upgrade/common.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/commands/upgrade/compose.py` & `tutor-17.0.5/tutor/commands/upgrade/compose.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/commands/upgrade/k8s.py` & `tutor-17.0.5/tutor/commands/upgrade/k8s.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/config.py` & `tutor-17.0.5/tutor/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,17 @@
     convert_json2yml(root)
     path = config_path(root)
     config = {}
     if os.path.exists(path):
         config = get_yaml_file(path)
     upgrade_obsolete(config)
     update_with_env(config)
+
+    for name, value in hooks.Filters.CONFIG_USER.iterate():
+        config[name] = value
     return config
 
 
 def get_base() -> Config:
     """
     Load the base configuration.
```

### Comparing `tutor-17.0.4/tutor/core/hooks/actions.py` & `tutor-17.0.5/tutor/core/hooks/actions.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/core/hooks/contexts.py` & `tutor-17.0.5/tutor/core/hooks/contexts.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/core/hooks/filters.py` & `tutor-17.0.5/tutor/core/hooks/filters.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/core/hooks/priorities.py` & `tutor-17.0.5/tutor/core/hooks/priorities.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/env.py` & `tutor-17.0.5/tutor/env.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/fmt.py` & `tutor-17.0.5/tutor/fmt.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/hooks/__init__.py` & `tutor-17.0.5/tutor/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/hooks/catalog.py` & `tutor-17.0.5/tutor/hooks/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,14 +253,25 @@
     #: Declare unique configuration settings that must be saved in the user ``config.yml`` file. This is where
     #: you should declare passwords and randomly-generated values that are different from one environment to the next.
     #:
     #: :parameter list[tuple[str, ...]] items: list of (name, value) new settings. All
     #:   names must be prefixed with the plugin name in all-caps.
     CONFIG_UNIQUE: Filter[list[tuple[str, Any]], []] = Filter()
 
+    #: Used to declare unique key:value pairs in the ``config.yml`` file that will be overwritten on ``tutor config save``.
+    #: This is where you should declare passwords and other secrets that need to be fetched live from an external secrets
+    #: store. Most users will not need to use this filter but it will allow you to programmatically fetch and set secrets
+    #: from an external secrets store such as AWS Secrets Manager via boto3.
+    #:
+    #: Values passed in to this filter will overwrite existing values in the ``config.yml`` file.
+    #:
+    #: :parameter list[tuple[str, ...]] items: list of (name, value) new settings. All
+    #:   names must be prefixed with the plugin name in all-caps.
+    CONFIG_USER: Filter[list[tuple[str, Any]], []] = Filter()
+
     #: Use this filter to modify the ``docker build`` command.
     #:
     #: :parameter list[str] command: the full build command, including options and
     #:   arguments. Note that these arguments do not include the leading ``docker`` command.
     DOCKER_BUILD_COMMAND: Filter[list[str], []] = Filter()
 
     #: List of patches that should be inserted in a given location of the templates.
```

### Comparing `tutor-17.0.4/tutor/images.py` & `tutor-17.0.5/tutor/images.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/interactive.py` & `tutor-17.0.5/tutor/interactive.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/plugins/__init__.py` & `tutor-17.0.5/tutor/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/plugins/base.py` & `tutor-17.0.5/tutor/plugins/base.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/plugins/indexes.py` & `tutor-17.0.5/tutor/plugins/indexes.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/plugins/openedx.py` & `tutor-17.0.5/tutor/plugins/openedx.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/plugins/v0.py` & `tutor-17.0.5/tutor/plugins/v0.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/plugins/v1.py` & `tutor-17.0.5/tutor/plugins/v1.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/serialize.py` & `tutor-17.0.5/tutor/serialize.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/tasks.py` & `tutor-17.0.5/tutor/tasks.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/apps/caddy/Caddyfile` & `tutor-17.0.5/tutor/templates/apps/caddy/Caddyfile`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     # see https://caddyserver.com/docs/caddyfile/directives/encode
     # for information about the defaults; i.e. how/when this will be applied.
     encode gzip
 
     reverse_proxy {args.0} {
         header_up X-Forwarded-Port {{ 443 if ENABLE_HTTPS else 80 }}
     }
+
+    {{ patch("caddyfile-proxy")|indent(4) }}
 }
 
 {{ LMS_HOST }}{$default_site_port}, {{ PREVIEW_LMS_HOST }}{$default_site_port} {
     @favicon_matcher {
         path_regexp ^/favicon.ico$
     }
     rewrite @favicon_matcher /theming/asset/images/favicon.ico
```

### Comparing `tutor-17.0.4/tutor/templates/apps/openedx/config/cms.env.yml` & `tutor-17.0.5/tutor/templates/apps/openedx/config/cms.env.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/apps/openedx/config/lms.env.yml` & `tutor-17.0.5/tutor/templates/apps/openedx/config/lms.env.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/apps/openedx/config/partials/auth.yml` & `tutor-17.0.5/tutor/templates/apps/openedx/config/partials/auth.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/apps/openedx/settings/cms/development.py` & `tutor-17.0.5/tutor/templates/apps/openedx/settings/cms/development.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/apps/openedx/settings/cms/production.py` & `tutor-17.0.5/tutor/templates/apps/openedx/settings/cms/production.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/apps/openedx/settings/lms/development.py` & `tutor-17.0.5/tutor/templates/apps/openedx/settings/lms/development.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/apps/openedx/settings/lms/production.py` & `tutor-17.0.5/tutor/templates/apps/openedx/settings/lms/production.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/common_all.py` & `tutor-17.0.5/tutor/templates/apps/openedx/settings/partials/common_all.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/common_cms.py` & `tutor-17.0.5/tutor/templates/apps/openedx/settings/partials/common_cms.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/apps/openedx/settings/partials/common_lms.py` & `tutor-17.0.5/tutor/templates/apps/openedx/settings/partials/common_lms.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/apps/redis/redis.conf` & `tutor-17.0.5/tutor/templates/apps/redis/redis.conf`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/build/openedx/Dockerfile` & `tutor-17.0.5/tutor/templates/build/openedx/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,18 @@
 {%- elif EDX_PLATFORM_VERSION == "master" %}
 # Patches in nightly node
 {%- else %}
 # Patches in non-nightly mode
 # Prevent course structure cache infinite growth
 # https://github.com/openedx/edx-platform/pull/34210
 RUN curl -fsSL https://github.com/openedx/edx-platform/commit/ad201cd664b6c722cbefcbda23ae390c06daf621.patch | git am
+# Security patch for "Privilege re-escalation in Studio after staff access removed"
+# https://github.com/openedx/edx-platform/security/advisories/GHSA-99vw-2wrq-xh9x
+# https://discuss.openedx.org/t/upcoming-security-fix-for-edx-platform-on-2024-05-17/13004
+RUN curl -fsSL https://github.com/openedx/edx-platform/commit/3ff69fd5813256f935f19c237ea0c42d4c16edbf.patch | git am
 {%- endif %}
 
 {# Example: RUN curl -fsSL https://github.com/openedx/edx-platform/commit/<GITSHA1>.patch | git am #}
 {{ patch("openedx-dockerfile-post-git-checkout") }}
 
 ##### Empty layer with just the repo at the root.
 # This is useful when overriding the build context with a host repo:
```

### Comparing `tutor-17.0.4/tutor/templates/build/openedx/bin/openedx-assets` & `tutor-17.0.5/tutor/templates/build/openedx/bin/openedx-assets`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/build/openedx/bin/site-configuration` & `tutor-17.0.5/tutor/templates/build/openedx/bin/site-configuration`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/config/base.yml` & `tutor-17.0.5/tutor/templates/config/base.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/config/defaults.yml` & `tutor-17.0.5/tutor/templates/config/defaults.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/dev/docker-compose.jobs.yml` & `tutor-17.0.5/tutor/templates/dev/docker-compose.jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/dev/docker-compose.yml` & `tutor-17.0.5/tutor/templates/dev/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/jobs/init/cms.sh` & `tutor-17.0.5/tutor/templates/jobs/init/cms.sh`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/jobs/init/lms.sh` & `tutor-17.0.5/tutor/templates/jobs/init/lms.sh`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/jobs/init/mounted-directories.sh` & `tutor-17.0.5/tutor/templates/jobs/init/mounted-directories.sh`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/jobs/init/mysql.sh` & `tutor-17.0.5/tutor/templates/jobs/init/mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/k8s/deployments.yml` & `tutor-17.0.5/tutor/templates/k8s/deployments.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/k8s/jobs.yml` & `tutor-17.0.5/tutor/templates/k8s/jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/k8s/services.yml` & `tutor-17.0.5/tutor/templates/k8s/services.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/k8s/volumes.yml` & `tutor-17.0.5/tutor/templates/k8s/volumes.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/kustomization.yml` & `tutor-17.0.5/tutor/templates/kustomization.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/local/docker-compose.jobs.yml` & `tutor-17.0.5/tutor/templates/local/docker-compose.jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/local/docker-compose.prod.yml` & `tutor-17.0.5/tutor/templates/local/docker-compose.prod.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/templates/local/docker-compose.yml` & `tutor-17.0.5/tutor/templates/local/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/types.py` & `tutor-17.0.5/tutor/types.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor/utils.py` & `tutor-17.0.5/tutor/utils.py`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor.egg-info/PKG-INFO` & `tutor-17.0.5/tutor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor
-Version: 17.0.4
+Version: 17.0.5
 Summary: The Docker-based Open edX distribution designed for peace of mind
 Home-page: https://docs.tutor.edly.io/
 Author: Edly
 Author-email: hello@edly.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.edly.io/
 Project-URL: Code, https://github.com/overhangio/tutor
```

### Comparing `tutor-17.0.4/tutor.egg-info/SOURCES.txt` & `tutor-17.0.5/tutor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-17.0.4/tutor.egg-info/requires.txt` & `tutor-17.0.5/tutor.egg-info/requires.txt`

 * *Files identical despite different names*

