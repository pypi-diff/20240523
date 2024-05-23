# Comparing `tmp/pypnusershub-2.1.4.tar.gz` & `tmp/pypnusershub-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypnusershub-2.1.4.tar", last modified: Tue Apr 23 12:23:07 2024, max compression
+gzip compressed data, was "pypnusershub-2.1.5.tar", last modified: Thu May 23 15:03:14 2024, max compression
```

## Comparing `pypnusershub-2.1.4.tar` & `pypnusershub-2.1.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.468631 pypnusershub-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-04-23 12:23:07.468631 pypnusershub-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/requirements-common.in
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/requirements-dependencies.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 12:23:07.468631 pypnusershub-2.1.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1564 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.460631 pypnusershub-2.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.464631 pypnusershub-2.1.4/src/pypnusershub/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.464631 pypnusershub-2.1.4/src/pypnusershub/db/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/db/fixtures.sql
--rw-r--r--   0 runner    (1001) docker     (127)    14767 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/db/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/db/models_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/db/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/login_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.464631 pypnusershub-2.1.4/src/pypnusershub/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.464631 pypnusershub-2.1.4/src/pypnusershub/migrations/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/data/utilisateurs-samples.sql
--rw-r--r--   0 runner    (1001) docker     (127)    15812 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/data/utilisateurs.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.468631 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/f4bf21ac6238_fix_temp_user_organism_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/f9d3b95946cd_set_code_profil_in_integer.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6956 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/routes_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.468631 pypnusershub-2.1.4/src/pypnusershub/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/tests/test_utilisateurs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.468631 pypnusershub-2.1.4/src/pypnusershub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-04-23 12:23:07.000000 pypnusershub-2.1.4/src/pypnusershub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-23 12:23:07.000000 pypnusershub-2.1.4/src/pypnusershub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:23:07.000000 pypnusershub-2.1.4/src/pypnusershub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 12:23:07.000000 pypnusershub-2.1.4/src/pypnusershub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-23 12:23:07.000000 pypnusershub-2.1.4/src/pypnusershub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 12:23:07.000000 pypnusershub-2.1.4/src/pypnusershub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:03:14.242059 pypnusershub-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-05-23 15:03:14.242059 pypnusershub-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/requirements-common.in
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/requirements-dependencies.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:03:14.242059 pypnusershub-2.1.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1564 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:03:14.230059 pypnusershub-2.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:03:14.238059 pypnusershub-2.1.5/src/pypnusershub/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:03:14.238059 pypnusershub-2.1.5/src/pypnusershub/db/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/db/fixtures.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    14767 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/db/models_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/db/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/login_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:03:14.238059 pypnusershub-2.1.5/src/pypnusershub/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:03:14.238059 pypnusershub-2.1.5/src/pypnusershub/migrations/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/migrations/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/migrations/data/utilisateurs-samples.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    15812 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/migrations/data/utilisateurs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:03:14.242059 pypnusershub-2.1.5/src/pypnusershub/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/migrations/versions/f4bf21ac6238_fix_temp_user_organism_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/migrations/versions/f9d3b95946cd_set_code_profil_in_integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7510 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/routes_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:03:14.242059 pypnusershub-2.1.5/src/pypnusershub/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/tests/test_utilisateurs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-23 15:03:09.000000 pypnusershub-2.1.5/src/pypnusershub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:03:14.242059 pypnusershub-2.1.5/src/pypnusershub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-05-23 15:03:14.000000 pypnusershub-2.1.5/src/pypnusershub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-23 15:03:14.000000 pypnusershub-2.1.5/src/pypnusershub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:03:14.000000 pypnusershub-2.1.5/src/pypnusershub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 15:03:14.000000 pypnusershub-2.1.5/src/pypnusershub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-23 15:03:14.000000 pypnusershub-2.1.5/src/pypnusershub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 15:03:14.000000 pypnusershub-2.1.5/src/pypnusershub.egg-info/top_level.txt
```

### Comparing `pypnusershub-2.1.4/LICENSE` & `pypnusershub-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/PKG-INFO` & `pypnusershub-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypnusershub
-Version: 2.1.4
+Version: 2.1.5
 Summary: Python lib to authenticate using PN's UsersHub
 Home-page: https://github.com/PnX-SI/UsersHub-authentification-module
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pypnusershub-2.1.4/README.md` & `pypnusershub-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/setup.py` & `pypnusershub-2.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/__main__.py` & `pypnusershub-2.1.5/src/pypnusershub/__main__.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/db/fixtures.sql` & `pypnusershub-2.1.5/src/pypnusershub/db/fixtures.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/db/models.py` & `pypnusershub-2.1.5/src/pypnusershub/db/models.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/db/models_register.py` & `pypnusershub-2.1.5/src/pypnusershub/db/models_register.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/db/tools.py` & `pypnusershub-2.1.5/src/pypnusershub/db/tools.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/decorators.py` & `pypnusershub-2.1.5/src/pypnusershub/decorators.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/env.py` & `pypnusershub-2.1.5/src/pypnusershub/env.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/login_manager.py` & `pypnusershub-2.1.5/src/pypnusershub/login_manager.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/migrations/data/utilisateurs-samples.sql` & `pypnusershub-2.1.5/src/pypnusershub/migrations/data/utilisateurs-samples.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/migrations/data/utilisateurs.sql` & `pypnusershub-2.1.5/src/pypnusershub/migrations/data/utilisateurs.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/migrations/env.py` & `pypnusershub-2.1.5/src/pypnusershub/migrations/env.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py` & `pypnusershub-2.1.5/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py` & `pypnusershub-2.1.5/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py` & `pypnusershub-2.1.5/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py` & `pypnusershub-2.1.5/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py` & `pypnusershub-2.1.5/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py` & `pypnusershub-2.1.5/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/f9d3b95946cd_set_code_profil_in_integer.py` & `pypnusershub-2.1.5/src/pypnusershub/migrations/versions/f9d3b95946cd_set_code_profil_in_integer.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py` & `pypnusershub-2.1.5/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/routes.py` & `pypnusershub-2.1.5/src/pypnusershub/routes.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 routes relatives aux application, utilisateurs et à l'authentification
 """
 
 import json
 import logging
 
 import datetime
-from flask_login import login_user, logout_user, current_user
+from flask_login import login_required, login_user, logout_user, current_user
 from flask import (
     Blueprint,
     request,
     Response,
     current_app,
     redirect,
     g,
@@ -85,14 +85,34 @@
 
 routes = ConfigurableBlueprint("auth", __name__)
 
 # retrocompatibilité before 2.0
 from pypnusershub.decorators import check_auth
 
 
+@routes.route("/get_current_user")
+@login_required
+def get_user_data():
+    user_dict = UserSchema(exclude=["remarques"], only=["+max_level_profil"]).dump(
+        g.current_user
+    )
+
+    token_exp = datetime.datetime.now(datetime.timezone.utc)
+    token_exp += datetime.timedelta(
+        seconds=current_app.config.get("COOKIE_EXPIRATION", 3600)
+    )
+    data = {
+        "user": user_dict,
+        "token": encode_token(g.current_user.as_dict()).decode(),
+        "expires": token_exp.isoformat(),
+    }
+
+    return jsonify(data)
+
+
 @routes.route("/login", methods=["POST"])
 def login():
     user_data = request.json
     try:
         login = user_data.get("login")
         password = user_data.get("password")
         id_app = user_data.get("id_application", get_current_app_id())
```

### Comparing `pypnusershub-2.1.4/src/pypnusershub/routes_register.py` & `pypnusershub-2.1.5/src/pypnusershub/routes_register.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/schemas.py` & `pypnusershub-2.1.5/src/pypnusershub/schemas.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/tests/conftest.py` & `pypnusershub-2.1.5/src/pypnusershub/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/tests/fixtures.py` & `pypnusershub-2.1.5/src/pypnusershub/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/tests/test_utilisateurs.py` & `pypnusershub-2.1.5/src/pypnusershub/tests/test_utilisateurs.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/tests/test_utils.py` & `pypnusershub-2.1.5/src/pypnusershub/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/tests/utils.py` & `pypnusershub-2.1.5/src/pypnusershub/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub/utils.py` & `pypnusershub-2.1.5/src/pypnusershub/utils.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.4/src/pypnusershub.egg-info/PKG-INFO` & `pypnusershub-2.1.5/src/pypnusershub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypnusershub
-Version: 2.1.4
+Version: 2.1.5
 Summary: Python lib to authenticate using PN's UsersHub
 Home-page: https://github.com/PnX-SI/UsersHub-authentification-module
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pypnusershub-2.1.4/src/pypnusershub.egg-info/SOURCES.txt` & `pypnusershub-2.1.5/src/pypnusershub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

