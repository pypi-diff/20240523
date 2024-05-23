# Comparing `tmp/flask_imp-4.0.1.tar.gz` & `tmp/flask_imp-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_imp-4.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "flask_imp-4.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flask_imp-4.0.1.tar` & `flask_imp-4.0.2.tar`

### file list

```diff
@@ -1,91 +1,54 @@
--rw-r--r--   0        0        0     1063 2024-04-10 12:24:23.959533 flask_imp-4.0.1/LICENSE
--rw-r--r--   0        0        0     2813 2024-04-10 12:59:59.761172 flask_imp-4.0.1/README.md
--rw-r--r--   0        0        0     2771 2024-04-10 11:19:08.711168 flask_imp-4.0.1/docs_md/Blueprint-Introduction.md
--rw-r--r--   0        0        0     4015 2024-04-10 11:19:08.711269 flask_imp-4.0.1/docs_md/Blueprint-config-x.md
--rw-r--r--   0        0        0      375 2024-03-11 17:31:21.990920 flask_imp-4.0.1/docs_md/Blueprint-init.md
--rw-r--r--   0        0        0     1432 2024-03-11 17:31:21.990986 flask_imp-4.0.1/docs_md/Blueprint_x-import_models.md
--rw-r--r--   0        0        0     1414 2024-03-11 17:31:21.991095 flask_imp-4.0.1/docs_md/Blueprint_x-import_nested_blueprint.md
--rw-r--r--   0        0        0     1383 2024-03-11 17:31:21.991151 flask_imp-4.0.1/docs_md/Blueprint_x-import_nested_blueprints.md
--rw-r--r--   0        0        0     1080 2024-03-11 17:31:21.991224 flask_imp-4.0.1/docs_md/Blueprint_x-import_resources.md
--rw-r--r--   0        0        0      341 2024-03-11 17:31:21.991285 flask_imp-4.0.1/docs_md/Blueprint_x-init_session.md
--rw-r--r--   0        0        0      904 2024-03-11 17:31:21.991350 flask_imp-4.0.1/docs_md/Blueprint_x-tmpl.md
--rw-r--r--   0        0        0     2876 2024-04-10 11:19:08.711483 flask_imp-4.0.1/docs_md/CLI Commands-flask-imp blueprint.md
--rw-r--r--   0        0        0     6032 2024-04-10 11:19:08.711690 flask_imp-4.0.1/docs_md/CLI Commands-flask-imp init.md
--rw-r--r--   0        0        0     2674 2024-04-10 11:19:08.711991 flask_imp-4.0.1/docs_md/Imp-Introduction.md
--rw-r--r--   0        0        0     7475 2024-04-10 11:19:08.712087 flask_imp-4.0.1/docs_md/Imp-config-x.md
--rw-r--r--   0        0        0     2429 2024-03-11 17:31:21.991756 flask_imp-4.0.1/docs_md/Imp_x-import_app_resources.md
--rw-r--r--   0        0        0     2104 2024-03-11 17:31:21.991824 flask_imp-4.0.1/docs_md/Imp_x-import_blueprint.md
--rw-r--r--   0        0        0      971 2024-03-11 17:31:21.991888 flask_imp-4.0.1/docs_md/Imp_x-import_blueprints.md
--rw-r--r--   0        0        0     1401 2024-03-11 17:31:21.991949 flask_imp-4.0.1/docs_md/Imp_x-import_models.md
--rw-r--r--   0        0        0     1236 2024-04-10 11:19:08.712300 flask_imp-4.0.1/docs_md/Imp_x-init_app-init.md
--rw-r--r--   0        0        0      734 2024-04-10 11:19:08.712558 flask_imp-4.0.1/docs_md/Imp_x-init_session.md
--rw-r--r--   0        0        0      965 2024-03-11 17:31:21.992158 flask_imp-4.0.1/docs_md/Imp_x-model.md
--rw-r--r--   0        0        0     4354 2024-04-10 11:19:08.712814 flask_imp-4.0.1/docs_md/__index__.md
--rw-r--r--   0        0        0      935 2024-04-10 11:19:08.713090 flask_imp-4.0.1/docs_md/__menu__.md
--rw-r--r--   0        0        0     1630 2024-03-11 17:31:21.992361 flask_imp-4.0.1/docs_md/flask_imp_auth-authenticate_password.md
--rw-r--r--   0        0        0     1566 2024-03-11 17:31:21.992429 flask_imp-4.0.1/docs_md/flask_imp_auth-encrypt_password.md
--rw-r--r--   0        0        0      440 2024-03-11 17:31:21.992490 flask_imp-4.0.1/docs_md/flask_imp_auth-generate_alphanumeric_validator.md
--rw-r--r--   0        0        0      502 2024-03-11 17:31:21.992550 flask_imp-4.0.1/docs_md/flask_imp_auth-generate_csrf_token.md
--rw-r--r--   0        0        0      588 2024-03-11 17:31:21.992597 flask_imp-4.0.1/docs_md/flask_imp_auth-generate_email_validator.md
--rw-r--r--   0        0        0      507 2024-03-11 17:31:21.992684 flask_imp-4.0.1/docs_md/flask_imp_auth-generate_numeric_validator.md
--rw-r--r--   0        0        0      474 2024-03-11 17:31:21.992776 flask_imp-4.0.1/docs_md/flask_imp_auth-generate_password.md
--rw-r--r--   0        0        0      904 2024-03-11 17:31:21.992914 flask_imp-4.0.1/docs_md/flask_imp_auth-generate_private_key.md
--rw-r--r--   0        0        0      856 2024-03-11 17:31:21.992979 flask_imp-4.0.1/docs_md/flask_imp_auth-generate_salt.md
--rw-r--r--   0        0        0      865 2024-03-11 17:31:21.993047 flask_imp-4.0.1/docs_md/flask_imp_auth-is_email_address_valid.md
--rw-r--r--   0        0        0     1037 2024-03-11 17:31:21.993124 flask_imp-4.0.1/docs_md/flask_imp_auth-is_username_valid.md
--rw-r--r--   0        0        0     1018 2024-03-11 17:31:21.993190 flask_imp-4.0.1/docs_md/flask_imp_security-api_login_check.md
--rw-r--r--   0        0        0     1104 2024-03-11 17:31:21.993250 flask_imp-4.0.1/docs_md/flask_imp_security-include_csrf.md
--rw-r--r--   0        0        0     1641 2024-03-11 17:31:21.993327 flask_imp-4.0.1/docs_md/flask_imp_security-login_check.md
--rw-r--r--   0        0        0      169 2024-03-11 17:31:21.993393 flask_imp-4.0.1/docs_md/flask_imp_security-pass_function_check.md
--rw-r--r--   0        0        0     1403 2024-03-11 17:31:21.993454 flask_imp-4.0.1/docs_md/flask_imp_security-permission_check.md
--rw-r--r--   0        0        0      673 2024-04-10 13:00:11.700776 flask_imp-4.0.1/flask_imp/__init__.py
--rw-r--r--   0        0        0     3144 2024-04-10 11:19:08.713710 flask_imp-4.0.1/flask_imp/_cli/__init__.py
--rw-r--r--   0        0        0     4990 2024-04-10 11:19:08.714051 flask_imp-4.0.1/flask_imp/_cli/blueprint.py
--rw-r--r--   0        0        0      299 2024-03-11 17:31:21.993886 flask_imp-4.0.1/flask_imp/_cli/filelib/__init__.py
--rw-r--r--   0        0        0     6517 2024-03-11 17:31:21.994015 flask_imp-4.0.1/flask_imp/_cli/filelib/all_files.py
--rw-r--r--   0        0        0    14125 2024-04-10 11:19:08.714430 flask_imp-4.0.1/flask_imp/_cli/filelib/app.py
--rw-r--r--   0        0        0     4527 2024-04-10 11:54:53.832600 flask_imp-4.0.1/flask_imp/_cli/filelib/blueprint.py
--rw-r--r--   0        0        0    33707 2024-03-11 17:31:21.994306 flask_imp-4.0.1/flask_imp/_cli/filelib/favicon.py
--rw-r--r--   0        0        0    17864 2024-03-11 17:31:21.994420 flask_imp-4.0.1/flask_imp/_cli/filelib/flask_imp_logo.py
--rw-r--r--   0        0        0      823 2024-03-11 17:31:21.994511 flask_imp-4.0.1/flask_imp/_cli/filelib/head_tag_generator.py
--rw-r--r--   0        0        0       88 2024-03-11 17:31:21.994564 flask_imp-4.0.1/flask_imp/_cli/filelib/main_js.py
--rw-r--r--   0        0        0    17166 2024-03-11 17:31:21.994646 flask_imp-4.0.1/flask_imp/_cli/filelib/water_css.py
--rw-r--r--   0        0        0      587 2024-03-11 17:31:21.994731 flask_imp-4.0.1/flask_imp/_cli/helpers.py
--rw-r--r--   0        0        0     9739 2024-04-10 11:19:08.715059 flask_imp-4.0.1/flask_imp/_cli/init.py
--rw-r--r--   0        0        0     1057 2024-03-11 17:31:21.994913 flask_imp-4.0.1/flask_imp/auth/__init__.py
--rw-r--r--   0        0        0     6432 2024-03-11 17:31:21.995112 flask_imp-4.0.1/flask_imp/auth/__legacy__.py
--rw-r--r--   0        0        0      850 2024-03-11 17:31:21.995175 flask_imp-4.0.1/flask_imp/auth/__private_funcs__.py
--rw-r--r--   0        0        0     2748 2024-03-11 17:31:21.995246 flask_imp-4.0.1/flask_imp/auth/authenticate_password.py
--rw-r--r--   0        0        0    14294 2024-03-11 17:31:21.995365 flask_imp-4.0.1/flask_imp/auth/dataclasses.py
--rw-r--r--   0        0        0     1844 2024-03-11 17:31:21.995427 flask_imp-4.0.1/flask_imp/auth/encrypt_password.py
--rw-r--r--   0        0        0      535 2024-03-11 17:31:21.995484 flask_imp-4.0.1/flask_imp/auth/generate_alphanumeric_validator.py
--rw-r--r--   0        0        0      385 2024-03-11 17:31:21.995544 flask_imp-4.0.1/flask_imp/auth/generate_csrf_token.py
--rw-r--r--   0        0        0      524 2024-03-11 17:31:21.995600 flask_imp-4.0.1/flask_imp/auth/generate_email_validator.py
--rw-r--r--   0        0        0      607 2024-03-11 17:31:21.995686 flask_imp-4.0.1/flask_imp/auth/generate_numeric_validator.py
--rw-r--r--   0        0        0     1545 2024-03-11 17:31:21.995743 flask_imp-4.0.1/flask_imp/auth/generate_password.py
--rw-r--r--   0        0        0      697 2024-03-11 17:31:21.995815 flask_imp-4.0.1/flask_imp/auth/generate_private_key.py
--rw-r--r--   0        0        0      426 2024-03-11 17:31:21.995879 flask_imp-4.0.1/flask_imp/auth/generate_salt.py
--rw-r--r--   0        0        0     1139 2024-03-11 17:31:21.995940 flask_imp-4.0.1/flask_imp/auth/is_email_address_valid.py
--rw-r--r--   0        0        0     1872 2024-03-11 17:31:21.995999 flask_imp-4.0.1/flask_imp/auth/is_username_valid.py
--rw-r--r--   0        0        0     1558 2024-04-10 11:19:08.715176 flask_imp-4.0.1/flask_imp/config_database_template.py
--rw-r--r--   0        0        0     8880 2024-04-10 11:19:08.715330 flask_imp-4.0.1/flask_imp/config_flask_template.py
--rw-r--r--   0        0        0     2528 2024-04-10 11:19:08.715438 flask_imp-4.0.1/flask_imp/config_imp_blueprint_template.py
--rw-r--r--   0        0        0     2067 2024-04-10 11:19:08.715555 flask_imp-4.0.1/flask_imp/config_imp_template.py
--rw-r--r--   0        0        0      932 2024-04-10 11:19:08.715674 flask_imp-4.0.1/flask_imp/config_object_parser.py
--rw-r--r--   0        0        0     6370 2024-04-10 11:19:08.715800 flask_imp-4.0.1/flask_imp/config_toml_parser.py
--rw-r--r--   0        0        0       87 2024-04-10 11:19:08.715907 flask_imp-4.0.1/flask_imp/exceptions.py
--rw-r--r--   0        0        0    24112 2024-04-10 11:19:08.716353 flask_imp-4.0.1/flask_imp/imp.py
--rw-r--r--   0        0        0    14397 2024-04-10 11:55:17.235524 flask_imp-4.0.1/flask_imp/imp_blueprint.py
--rw-r--r--   0        0        0     4840 2024-04-10 11:43:13.630660 flask_imp-4.0.1/flask_imp/protocols.py
--rw-r--r--   0        0        0      917 2024-03-11 17:31:21.996484 flask_imp-4.0.1/flask_imp/registeries.py
--rw-r--r--   0        0        0      349 2024-03-11 17:31:21.996580 flask_imp-4.0.1/flask_imp/security/__init__.py
--rw-r--r--   0        0        0      708 2024-03-11 17:31:21.996651 flask_imp-4.0.1/flask_imp/security/__private_funcs__.py
--rw-r--r--   0        0        0     1802 2024-03-11 17:31:21.996745 flask_imp-4.0.1/flask_imp/security/api_login_check.py
--rw-r--r--   0        0        0     2222 2024-03-11 17:31:21.996828 flask_imp-4.0.1/flask_imp/security/include_csrf.py
--rw-r--r--   0        0        0     3880 2024-03-11 17:31:21.996900 flask_imp-4.0.1/flask_imp/security/login_check.py
--rw-r--r--   0        0        0     7117 2024-03-11 17:31:21.997016 flask_imp-4.0.1/flask_imp/security/pass_function_check.py
--rw-r--r--   0        0        0     2688 2024-03-11 17:31:21.997074 flask_imp-4.0.1/flask_imp/security/permission_check.py
--rw-r--r--   0        0        0     5476 2024-04-10 11:19:08.717102 flask_imp-4.0.1/flask_imp/utilities.py
--rw-r--r--   0        0        0     1883 2024-04-10 12:54:20.642886 flask_imp-4.0.1/pyproject.toml
--rw-r--r--   0        0        0       27 2024-04-10 11:19:08.717892 flask_imp-4.0.1/requirements.txt
--rw-r--r--   0        0        0     4020 1970-01-01 00:00:00.000000 flask_imp-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-10 12:24:23.959533 flask_imp-4.0.2/LICENSE
+-rw-r--r--   0        0        0     2785 2024-05-13 15:48:30.789222 flask_imp-4.0.2/README.md
+-rw-r--r--   0        0        0      673 2024-05-23 19:26:13.518354 flask_imp-4.0.2/flask_imp/__init__.py
+-rw-r--r--   0        0        0     3144 2024-04-10 11:19:08.713710 flask_imp-4.0.2/flask_imp/_cli/__init__.py
+-rw-r--r--   0        0        0     4990 2024-04-10 11:19:08.714051 flask_imp-4.0.2/flask_imp/_cli/blueprint.py
+-rw-r--r--   0        0        0      299 2024-03-11 17:31:21.993886 flask_imp-4.0.2/flask_imp/_cli/filelib/__init__.py
+-rw-r--r--   0        0        0     6466 2024-05-23 19:20:13.052450 flask_imp-4.0.2/flask_imp/_cli/filelib/all_files.py
+-rw-r--r--   0        0        0    14125 2024-04-10 11:19:08.714430 flask_imp-4.0.2/flask_imp/_cli/filelib/app.py
+-rw-r--r--   0        0        0     4548 2024-05-23 19:16:39.159053 flask_imp-4.0.2/flask_imp/_cli/filelib/blueprint.py
+-rw-r--r--   0        0        0    33707 2024-03-11 17:31:21.994306 flask_imp-4.0.2/flask_imp/_cli/filelib/favicon.py
+-rw-r--r--   0        0        0    17864 2024-03-11 17:31:21.994420 flask_imp-4.0.2/flask_imp/_cli/filelib/flask_imp_logo.py
+-rw-r--r--   0        0        0      823 2024-03-11 17:31:21.994511 flask_imp-4.0.2/flask_imp/_cli/filelib/head_tag_generator.py
+-rw-r--r--   0        0        0       88 2024-03-11 17:31:21.994564 flask_imp-4.0.2/flask_imp/_cli/filelib/main_js.py
+-rw-r--r--   0        0        0    17166 2024-03-11 17:31:21.994646 flask_imp-4.0.2/flask_imp/_cli/filelib/water_css.py
+-rw-r--r--   0        0        0      587 2024-03-11 17:31:21.994731 flask_imp-4.0.2/flask_imp/_cli/helpers.py
+-rw-r--r--   0        0        0     9739 2024-04-10 11:19:08.715059 flask_imp-4.0.2/flask_imp/_cli/init.py
+-rw-r--r--   0        0        0     1057 2024-03-11 17:31:21.994913 flask_imp-4.0.2/flask_imp/auth/__init__.py
+-rw-r--r--   0        0        0     6432 2024-03-11 17:31:21.995112 flask_imp-4.0.2/flask_imp/auth/__legacy__.py
+-rw-r--r--   0        0        0      850 2024-03-11 17:31:21.995175 flask_imp-4.0.2/flask_imp/auth/__private_funcs__.py
+-rw-r--r--   0        0        0     2748 2024-03-11 17:31:21.995246 flask_imp-4.0.2/flask_imp/auth/authenticate_password.py
+-rw-r--r--   0        0        0    14294 2024-03-11 17:31:21.995365 flask_imp-4.0.2/flask_imp/auth/dataclasses.py
+-rw-r--r--   0        0        0     1844 2024-03-11 17:31:21.995427 flask_imp-4.0.2/flask_imp/auth/encrypt_password.py
+-rw-r--r--   0        0        0      535 2024-03-11 17:31:21.995484 flask_imp-4.0.2/flask_imp/auth/generate_alphanumeric_validator.py
+-rw-r--r--   0        0        0      385 2024-03-11 17:31:21.995544 flask_imp-4.0.2/flask_imp/auth/generate_csrf_token.py
+-rw-r--r--   0        0        0      524 2024-03-11 17:31:21.995600 flask_imp-4.0.2/flask_imp/auth/generate_email_validator.py
+-rw-r--r--   0        0        0      607 2024-03-11 17:31:21.995686 flask_imp-4.0.2/flask_imp/auth/generate_numeric_validator.py
+-rw-r--r--   0        0        0     1545 2024-03-11 17:31:21.995743 flask_imp-4.0.2/flask_imp/auth/generate_password.py
+-rw-r--r--   0        0        0      697 2024-03-11 17:31:21.995815 flask_imp-4.0.2/flask_imp/auth/generate_private_key.py
+-rw-r--r--   0        0        0      426 2024-03-11 17:31:21.995879 flask_imp-4.0.2/flask_imp/auth/generate_salt.py
+-rw-r--r--   0        0        0     1139 2024-03-11 17:31:21.995940 flask_imp-4.0.2/flask_imp/auth/is_email_address_valid.py
+-rw-r--r--   0        0        0     1872 2024-03-11 17:31:21.995999 flask_imp-4.0.2/flask_imp/auth/is_username_valid.py
+-rw-r--r--   0        0        0     1558 2024-04-10 11:19:08.715176 flask_imp-4.0.2/flask_imp/config_database_template.py
+-rw-r--r--   0        0        0     8880 2024-04-10 11:19:08.715330 flask_imp-4.0.2/flask_imp/config_flask_template.py
+-rw-r--r--   0        0        0     2528 2024-04-10 11:19:08.715438 flask_imp-4.0.2/flask_imp/config_imp_blueprint_template.py
+-rw-r--r--   0        0        0     2067 2024-04-10 11:19:08.715555 flask_imp-4.0.2/flask_imp/config_imp_template.py
+-rw-r--r--   0        0        0      932 2024-04-10 11:19:08.715674 flask_imp-4.0.2/flask_imp/config_object_parser.py
+-rw-r--r--   0        0        0     6370 2024-04-10 11:19:08.715800 flask_imp-4.0.2/flask_imp/config_toml_parser.py
+-rw-r--r--   0        0        0       87 2024-04-10 11:19:08.715907 flask_imp-4.0.2/flask_imp/exceptions.py
+-rw-r--r--   0        0        0    24112 2024-04-10 11:19:08.716353 flask_imp-4.0.2/flask_imp/imp.py
+-rw-r--r--   0        0        0    14397 2024-04-10 11:55:17.235524 flask_imp-4.0.2/flask_imp/imp_blueprint.py
+-rw-r--r--   0        0        0     4840 2024-04-10 11:43:13.630660 flask_imp-4.0.2/flask_imp/protocols.py
+-rw-r--r--   0        0        0      917 2024-03-11 17:31:21.996484 flask_imp-4.0.2/flask_imp/registeries.py
+-rw-r--r--   0        0        0      349 2024-03-11 17:31:21.996580 flask_imp-4.0.2/flask_imp/security/__init__.py
+-rw-r--r--   0        0        0      708 2024-03-11 17:31:21.996651 flask_imp-4.0.2/flask_imp/security/__private_funcs__.py
+-rw-r--r--   0        0        0     1802 2024-03-11 17:31:21.996745 flask_imp-4.0.2/flask_imp/security/api_login_check.py
+-rw-r--r--   0        0        0     2222 2024-03-11 17:31:21.996828 flask_imp-4.0.2/flask_imp/security/include_csrf.py
+-rw-r--r--   0        0        0     3880 2024-03-11 17:31:21.996900 flask_imp-4.0.2/flask_imp/security/login_check.py
+-rw-r--r--   0        0        0     7117 2024-03-11 17:31:21.997016 flask_imp-4.0.2/flask_imp/security/pass_function_check.py
+-rw-r--r--   0        0        0     2688 2024-03-11 17:31:21.997074 flask_imp-4.0.2/flask_imp/security/permission_check.py
+-rw-r--r--   0        0        0     5476 2024-04-10 11:19:08.717102 flask_imp-4.0.2/flask_imp/utilities.py
+-rw-r--r--   0        0        0     1883 2024-04-10 12:54:20.642886 flask_imp-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0       83 2024-05-13 15:48:30.805509 flask_imp-4.0.2/requirements/development.txt
+-rw-r--r--   0        0        0       27 2024-05-13 15:48:30.805619 flask_imp-4.0.2/requirements/main.txt
+-rw-r--r--   0        0        0     3992 1970-01-01 00:00:00.000000 flask_imp-4.0.2/PKG-INFO
```

### Comparing `flask_imp-4.0.1/LICENSE` & `flask_imp-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/README.md` & `flask_imp-4.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -97,16 +97,15 @@
 ```bash
 .\venv\Scripts\activate
 ```
 
 ### Install the requirements.
 
 ```bash
-pip install -r requirements.txt
-pip install -r requirements_dev.txt
+pip install -r requirements/development.txt
 ```
 
 ### Install the local version of Flask-Imp.
 
 ```bash
 flit install
 ```
@@ -137,18 +136,20 @@
 
 The test Flask app is located in the `tests/test_app` folder. 
 
 The tests are linked to the tests blueprint located at `test_app/blueprints/tests`.
 
 ### Building the docs.
 
-All docs are generated from the [docs_md](docs_md) folder. Edit these files then run the following command to generate the docs.
+All docs are generated from the [docs](docs) folder. 
+
+Edit these files, then run the following command to generate the docs.
 
 ```bash
-flask --app gdocs compile
+flask --app docs compile
 ```
 
 You can set it to watch for changes and automatically recompile the docs by adding the `--watch` flag.
 
 ```bash
 flask --app gdocs compile --watch
 ```
```

### Comparing `flask_imp-4.0.1/docs_md/flask_imp_auth-authenticate_password.md` & `flask_imp-4.0.2/flask_imp/auth/authenticate_password.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,172 @@
-00000000: 6060 600a 4d65 6e75 203d 2066 6c61 736b  ```.Menu = flask
-00000010: 5f69 6d70 2e61 7574 682f 6175 7468 656e  _imp.auth/authen
-00000020: 7469 6361 7465 5f70 6173 7377 6f72 640a  ticate_password.
-00000030: 5469 746c 6520 3d20 6175 7468 656e 7469  Title = authenti
-00000040: 6361 7465 5f70 6173 7377 6f72 6420 2d20  cate_password - 
-00000050: 666c 6173 6b5f 696d 702e 6175 7468 0a60  flask_imp.auth.`
-00000060: 6060 0a0a 6060 6070 7974 686f 6e0a 6672  ``..```python.fr
-00000070: 6f6d 2066 6c61 736b 5f69 6d70 2e61 7574  om flask_imp.aut
-00000080: 6820 696d 706f 7274 2061 7574 6865 6e74  h import authent
-00000090: 6963 6174 655f 7061 7373 776f 7264 0a60  icate_password.`
-000000a0: 6060 0a0a 6060 6070 7974 686f 6e0a 6175  ``..```python.au
-000000b0: 7468 656e 7469 6361 7465 5f70 6173 7377  thenticate_passw
-000000c0: 6f72 6428 0a20 2020 2069 6e70 7574 5f70  ord(.    input_p
-000000d0: 6173 7377 6f72 643a 2073 7472 2c0a 2020  assword: str,.  
-000000e0: 2020 6461 7461 6261 7365 5f70 6173 7377    database_passw
-000000f0: 6f72 643a 2073 7472 2c0a 2020 2020 6461  ord: str,.    da
-00000100: 7461 6261 7365 5f73 616c 743a 2073 7472  tabase_salt: str
-00000110: 2c0a 2020 2020 656e 6372 7970 7469 6f6e  ,.    encryption
-00000120: 5f6c 6576 656c 3a20 696e 7420 3d20 3531  _level: int = 51
-00000130: 322c 0a20 2020 2070 6570 7065 725f 6c65  2,.    pepper_le
-00000140: 6e67 7468 3a20 696e 7420 3d20 312c 0a20  ngth: int = 1,. 
-00000150: 2020 2070 6570 7065 725f 706f 7369 7469     pepper_positi
-00000160: 6f6e 3a20 742e 4c69 7465 7261 6c5b 2273  on: t.Literal["s
-00000170: 7461 7274 222c 2022 656e 6422 5d20 3d20  tart", "end"] = 
-00000180: 2265 6e64 222c 0a20 2020 2075 7365 5f6d  "end",.    use_m
-00000190: 756c 7469 7072 6f63 6573 7369 6e67 3a20  ultiprocessing: 
-000001a0: 626f 6f6c 203d 2046 616c 7365 0a29 202d  bool = False.) -
-000001b0: 3e20 626f 6f6c 0a60 6060 0a0a 2d2d 2d0a  > bool.```..---.
-000001c0: 0a46 6f72 2075 7365 2069 6e20 7061 7373  .For use in pass
-000001d0: 776f 7264 2068 6173 6869 6e67 2e0a 0a54  word hashing...T
-000001e0: 6f20 6265 2075 7365 6420 616c 6f6e 6773  o be used alongs
-000001f0: 6964 6520 7468 6520 5b66 6c61 736b 5f69  ide the [flask_i
-00000200: 6d70 2e61 7574 6820 2f20 656e 6372 7970  mp.auth / encryp
-00000210: 745f 7061 7373 776f 7264 5d28 666c 6173  t_password](flas
-00000220: 6b5f 696d 705f 6175 7468 2d65 6e63 7279  k_imp_auth-encry
-00000230: 7074 5f70 6173 7377 6f72 642e 6874 6d6c  pt_password.html
-00000240: 2920 6675 6e63 7469 6f6e 2e0a 0a54 616b  ) function...Tak
-00000250: 6573 2074 6865 2070 6c61 696e 2069 6e70  es the plain inp
-00000260: 7574 2070 6173 7377 6f72 642c 2074 6865  ut password, the
-00000270: 2073 746f 7265 6420 6861 7368 6564 2070   stored hashed p
-00000280: 6173 7377 6f72 6420 616c 6f6e 6720 7769  assword along wi
-00000290: 7468 2074 6865 2073 746f 7265 6420 7361  th the stored sa
-000002a0: 6c74 0a61 6e64 2077 696c 6c20 7472 7920  lt.and will try 
-000002b0: 6576 6572 7920 706f 7373 6962 6c65 2063  every possible c
-000002c0: 6f6d 6269 6e61 7469 6f6e 206f 6620 7065  ombination of pe
-000002d0: 7070 6572 2076 616c 7565 7320 746f 2066  pper values to f
-000002e0: 696e 6420 6120 6d61 7463 682e 0a0a 2a2a  ind a match...**
-000002f0: 4e6f 7465 3a2a 2a0a 0a2a 2a75 7365 5f6d  Note:**..**use_m
-00000300: 756c 7469 7072 6f63 6573 7369 6e67 2069  ultiprocessing i
-00000310: 7320 6e6f 7420 636f 6d70 6174 6962 6c65  s not compatible
-00000320: 2077 6974 6820 636f 726f 7574 696e 6520   with coroutine 
-00000330: 776f 726b 6572 732c 2065 2e67 2e20 6576  workers, e.g. ev
-00000340: 656e 746c 6574 2f67 6576 656e 740a 636f  entlet/gevent.co
-00000350: 6d6d 6f6e 6c79 2075 7365 6420 7769 7468  mmonly used with
-00000360: 2073 6f63 6b65 7469 6f2e 2a2a 0a0a 4966   socketio.**..If
-00000370: 2079 6f75 2061 7265 2075 7369 6e67 2073   you are using s
-00000380: 6f63 6b65 7469 6f2c 2079 6f75 206d 7573  ocketio, you mus
-00000390: 7420 7365 7420 7573 655f 6d75 6c74 6970  t set use_multip
-000003a0: 726f 6365 7373 696e 6720 746f 2046 616c  rocessing to Fal
-000003b0: 7365 2028 6465 6661 756c 7429 2e0a 0a2a  se (default)...*
-000003c0: 2a4e 6f74 653a 2a2a 0a0a 2d20 596f 7520  *Note:**..- You 
-000003d0: 6d75 7374 206b 6e6f 7720 7468 6520 7065  must know the pe
-000003e0: 7070 6572 206c 656e 6774 6820 7573 6564  pper length used
-000003f0: 2074 6f20 6861 7368 2074 6865 2070 6173   to hash the pas
-00000400: 7377 6f72 642e 0a2d 2059 6f75 206d 7573  sword..- You mus
-00000410: 7420 6b6e 6f77 2074 6865 2070 6f73 6974  t know the posit
-00000420: 696f 6e20 6f66 2074 6865 2070 6570 7065  ion of the peppe
-00000430: 7220 7573 6564 2074 6f20 6861 7368 2074  r used to hash t
-00000440: 6865 2070 6173 7377 6f72 642e 0a2d 2059  he password..- Y
-00000450: 6f75 206d 7573 7420 6b6e 6f77 2074 6865  ou must know the
-00000460: 2065 6e63 7279 7074 696f 6e20 6c65 7665   encryption leve
-00000470: 6c20 7573 6564 2074 6f20 6861 7368 2074  l used to hash t
-00000480: 6865 2070 6173 7377 6f72 642e 0a0a 2323  he password...##
-00000490: 2323 2041 7574 6865 6e74 6963 6174 696f  ## Authenticatio
-000004a0: 6e20 5363 656e 6172 696f 3a0a 0a60 6060  n Scenario:..```
-000004b0: 0a50 6c61 696e 2070 6173 7377 6f72 643a  .Plain password:
-000004c0: 2022 7061 7373 776f 7264 220a 4765 6e65   "password".Gene
-000004d0: 7261 7465 6420 7361 6c74 3a20 225e 2524  rated salt: "^%$
-000004e0: 2a22 2028 7261 6e64 6f6d 6c79 2067 656e  *" (randomly gen
-000004f0: 6572 6174 6564 290a 4765 6e65 7261 7465  erated).Generate
-00000500: 6420 7065 7070 6572 2028 6c65 6e67 7468  d pepper (length
-00000510: 2031 293a 2022 4122 2028 7261 6e64 6f6d   1): "A" (random
-00000520: 6c79 2067 656e 6572 6174 6564 290a 5065  ly generated).Pe
-00000530: 7070 6572 2070 6f73 6974 696f 6e3a 2022  pper position: "
-00000540: 656e 6422 0a60 6060 0a0a 6060 6070 7974  end".```..```pyt
-00000550: 686f 6e0a 696e 7075 745f 7061 7373 776f  hon.input_passwo
-00000560: 7264 203d 2022 7061 7373 776f 7264 220a  rd = "password".
-00000570: 6461 7461 6261 7365 5f70 6173 7377 6f72  database_passwor
-00000580: 6420 3d20 2261 3162 3263 3364 3465 3566  d = "a1b2c3d4e5f
-00000590: 3667 3768 3869 396a 306b 316c 326d 336e  6g7h8i9j0k1l2m3n
-000005a0: 346f 3570 3671 3772 3873 3974 302e 2e2e  4o5p6q7r8s9t0...
-000005b0: 2220 2320 7075 6c6c 6564 2066 726f 6d20  " # pulled from 
-000005c0: 6461 7461 6261 7365 0a64 6174 6162 6173  database.databas
-000005d0: 655f 7361 6c74 203d 2022 5e25 242a 2220  e_salt = "^%$*" 
-000005e0: 2320 7075 6c6c 6564 2066 726f 6d20 6461  # pulled from da
-000005f0: 7461 6261 7365 0a0a 6175 7468 656e 7469  tabase..authenti
-00000600: 6361 7465 5f70 6173 7377 6f72 6428 0a20  cate_password(. 
-00000610: 2020 2069 6e70 7574 5f70 6173 7377 6f72     input_passwor
-00000620: 642c 0a20 2020 2064 6174 6162 6173 655f  d,.    database_
-00000630: 7061 7373 776f 7264 2c0a 2020 2020 6461  password,.    da
-00000640: 7461 6261 7365 5f73 616c 740a 2920 2023  tabase_salt.)  #
-00000650: 203e 3e3e 2054 7275 650a 6060 600a        >>> True.```.
+00000000: 696d 706f 7274 206d 756c 7469 7072 6f63  import multiproc
+00000010: 6573 7369 6e67 0a69 6d70 6f72 7420 7479  essing.import ty
+00000020: 7069 6e67 2061 7320 740a 6672 6f6d 2069  ping as t.from i
+00000030: 7465 7274 6f6f 6c73 2069 6d70 6f72 7420  tertools import 
+00000040: 7072 6f64 7563 740a 6672 6f6d 2073 7472  product.from str
+00000050: 696e 6720 696d 706f 7274 2061 7363 6969  ing import ascii
+00000060: 5f6c 6574 7465 7273 0a0a 6672 6f6d 206d  _letters..from m
+00000070: 6f72 655f 6974 6572 746f 6f6c 7320 696d  ore_itertools im
+00000080: 706f 7274 2062 6174 6368 6564 0a0a 6672  port batched..fr
+00000090: 6f6d 202e 5f5f 7072 6976 6174 655f 6675  om .__private_fu
+000000a0: 6e63 735f 5f20 696d 706f 7274 205f 6775  ncs__ import _gu
+000000b0: 6573 735f 626c 6f63 6b0a 0a0a 6465 6620  ess_block...def 
+000000c0: 6175 7468 656e 7469 6361 7465 5f70 6173  authenticate_pas
+000000d0: 7377 6f72 6428 0a20 2020 2069 6e70 7574  sword(.    input
+000000e0: 5f70 6173 7377 6f72 643a 2073 7472 2c0a  _password: str,.
+000000f0: 2020 2020 6461 7461 6261 7365 5f70 6173      database_pas
+00000100: 7377 6f72 643a 2073 7472 2c0a 2020 2020  sword: str,.    
+00000110: 6461 7461 6261 7365 5f73 616c 743a 2073  database_salt: s
+00000120: 7472 2c0a 2020 2020 656e 6372 7970 7469  tr,.    encrypti
+00000130: 6f6e 5f6c 6576 656c 3a20 696e 7420 3d20  on_level: int = 
+00000140: 3531 322c 0a20 2020 2070 6570 7065 725f  512,.    pepper_
+00000150: 6c65 6e67 7468 3a20 696e 7420 3d20 312c  length: int = 1,
+00000160: 0a20 2020 2070 6570 7065 725f 706f 7369  .    pepper_posi
+00000170: 7469 6f6e 3a20 742e 4c69 7465 7261 6c5b  tion: t.Literal[
+00000180: 2273 7461 7274 222c 2022 656e 6422 5d20  "start", "end"] 
+00000190: 3d20 2265 6e64 222c 0a20 2020 2075 7365  = "end",.    use
+000001a0: 5f6d 756c 7469 7072 6f63 6573 7369 6e67  _multiprocessing
+000001b0: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+000001c0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2022  ) -> bool:.    "
+000001d0: 2222 0a20 2020 2054 616b 6573 2074 6865  "".    Takes the
+000001e0: 2070 6c61 696e 2069 6e70 7574 2070 6173   plain input pas
+000001f0: 7377 6f72 642c 2074 6865 2073 746f 7265  sword, the store
+00000200: 6420 6861 7368 6564 2070 6173 7377 6f72  d hashed passwor
+00000210: 6420 616c 6f6e 6720 7769 7468 2074 6865  d along with the
+00000220: 2073 746f 7265 6420 7361 6c74 0a20 2020   stored salt.   
+00000230: 2061 6e64 2077 696c 6c20 7472 7920 6576   and will try ev
+00000240: 6572 7920 706f 7373 6962 6c65 2063 6f6d  ery possible com
+00000250: 6269 6e61 7469 6f6e 206f 6620 7065 7070  bination of pepp
+00000260: 6572 2076 616c 7565 7320 746f 2066 696e  er values to fin
+00000270: 6420 6120 6d61 7463 682e 0a0a 2020 2020  d a match...    
+00000280: 3a72 6177 2d68 746d 6c3a 603c 6272 202f  :raw-html:`<br /
+00000290: 3e60 0a0a 2020 2020 4e4f 5445 3a20 7573  >`..    NOTE: us
+000002a0: 655f 6d75 6c74 6970 726f 6365 7373 696e  e_multiprocessin
+000002b0: 6720 6973 206e 6f74 2063 6f6d 7061 7469  g is not compati
+000002c0: 626c 6520 7769 7468 2063 6f72 6f75 7469  ble with corouti
+000002d0: 6e65 2077 6f72 6b65 7273 2c20 652e 672e  ne workers, e.g.
+000002e0: 2065 7665 6e74 6c65 742f 6765 7665 6e74   eventlet/gevent
+000002f0: 0a20 2020 2020 636f 6d6d 6f6e 6c79 2075  .     commonly u
+00000300: 7365 6420 7769 7468 2073 6f63 6b65 7469  sed with socketi
+00000310: 6f2e 0a0a 2020 2020 2e2e 204e 6f74 653a  o...    .. Note:
+00000320: 3a0a 0a20 2020 2020 2020 2059 6f75 206d  :..        You m
+00000330: 7573 7420 6b6e 6f77 2074 6865 206c 656e  ust know the len
+00000340: 6774 6820 6f66 2074 6865 2070 6570 7065  gth of the peppe
+00000350: 7220 7573 6564 2074 6f20 6861 7368 2074  r used to hash t
+00000360: 6865 2070 6173 7377 6f72 642e 0a0a 2020  he password...  
+00000370: 2020 2020 2020 596f 7520 6d75 7374 206b        You must k
+00000380: 6e6f 7720 7468 6520 706f 7369 7469 6f6e  now the position
+00000390: 206f 6620 7468 6520 7065 7070 6572 2075   of the pepper u
+000003a0: 7365 6420 746f 2068 6173 6820 7468 6520  sed to hash the 
+000003b0: 7061 7373 776f 7264 2e0a 0a20 2020 2020  password...     
+000003c0: 2020 2059 6f75 206d 7573 7420 6b6e 6f77     You must know
+000003d0: 2074 6865 2065 6e63 7279 7074 696f 6e20   the encryption 
+000003e0: 6c65 7665 6c20 7573 6564 2074 6f20 6861  level used to ha
+000003f0: 7368 2074 6865 2070 6173 7377 6f72 642e  sh the password.
+00000400: 0a0a 2020 2020 3a72 6177 2d68 746d 6c3a  ..    :raw-html:
+00000410: 603c 6272 202f 3e60 0a0a 2020 2020 2d2d  `<br />`..    --
+00000420: 2d2d 2d0a 0a20 2020 203a 7061 7261 6d20  ---..    :param 
+00000430: 696e 7075 745f 7061 7373 776f 7264 3a20  input_password: 
+00000440: 7374 7220 2d20 706c 6169 6e20 7061 7373  str - plain pass
+00000450: 776f 7264 0a20 2020 203a 7061 7261 6d20  word.    :param 
+00000460: 6461 7461 6261 7365 5f70 6173 7377 6f72  database_passwor
+00000470: 643a 2073 7472 202d 2068 6173 6865 6420  d: str - hashed 
+00000480: 7061 7373 776f 7264 2066 726f 6d20 6461  password from da
+00000490: 7461 6261 7365 0a20 2020 203a 7061 7261  tabase.    :para
+000004a0: 6d20 6461 7461 6261 7365 5f73 616c 743a  m database_salt:
+000004b0: 2073 7472 202d 2073 616c 7420 6672 6f6d   str - salt from
+000004c0: 2064 6174 6162 6173 650a 2020 2020 3a70   database.    :p
+000004d0: 6172 616d 2065 6e63 7279 7074 696f 6e5f  aram encryption_
+000004e0: 6c65 7665 6c3a 2069 6e74 202d 2065 6e63  level: int - enc
+000004f0: 7279 7074 696f 6e20 7573 6564 2074 6f20  ryption used to 
+00000500: 6765 6e65 7261 7465 2064 6174 6162 6173  generate databas
+00000510: 6520 7061 7373 776f 7264 0a20 2020 203a  e password.    :
+00000520: 7061 7261 6d20 7065 7070 6572 5f6c 656e  param pepper_len
+00000530: 6774 683a 2069 6e74 202d 206c 656e 6774  gth: int - lengt
+00000540: 6820 6f66 2070 6570 7065 7220 7573 6564  h of pepper used
+00000550: 2074 6f20 6765 6e65 7261 7465 2064 6174   to generate dat
+00000560: 6162 6173 6520 7061 7373 776f 7264 0a20  abase password. 
+00000570: 2020 203a 7061 7261 6d20 7065 7070 6572     :param pepper
+00000580: 5f70 6f73 6974 696f 6e3a 2073 7472 202d  _position: str -
+00000590: 2022 7374 6172 7422 206f 7220 2265 6e64   "start" or "end
+000005a0: 2220 2d20 706f 7369 7469 6f6e 206f 6620  " - position of 
+000005b0: 7065 7070 6572 2075 7365 6420 746f 2067  pepper used to g
+000005c0: 656e 6572 6174 6520 6461 7461 6261 7365  enerate database
+000005d0: 2070 6173 7377 6f72 640a 2020 2020 3a70   password.    :p
+000005e0: 6172 616d 2075 7365 5f6d 756c 7469 7072  aram use_multipr
+000005f0: 6f63 6573 7369 6e67 3a20 626f 6f6c 202d  ocessing: bool -
+00000600: 2075 7365 206d 756c 7469 7072 6f63 6573   use multiproces
+00000610: 7369 6e67 2074 6f20 7370 6565 6420 7570  sing to speed up
+00000620: 2074 6865 2070 726f 6365 7373 2028 6e6f   the process (no
+00000630: 7420 636f 6d70 6174 6962 6c65 2077 6974  t compatible wit
+00000640: 6820 6576 656e 746c 6574 2f67 6576 656e  h eventlet/geven
+00000650: 7429 0a20 2020 203a 7265 7475 726e 3a20  t).    :return: 
+00000660: 626f 6f6c 202d 2054 7275 6520 6966 206d  bool - True if m
+00000670: 6174 6368 2c20 4661 6c73 6520 6966 206e  atch, False if n
+00000680: 6f74 0a20 2020 2022 2222 0a0a 2020 2020  ot.    """..    
+00000690: 6966 2070 6570 7065 725f 6c65 6e67 7468  if pepper_length
+000006a0: 203e 2033 3a0a 2020 2020 2020 2020 7065   > 3:.        pe
+000006b0: 7070 6572 5f6c 656e 6774 6820 3d20 330a  pper_length = 3.
+000006c0: 0a20 2020 205f 6775 6573 7365 7320 3d20  .    _guesses = 
+000006d0: 7b22 222e 6a6f 696e 2869 2920 666f 7220  {"".join(i) for 
+000006e0: 6920 696e 2070 726f 6475 6374 2861 7363  i in product(asc
+000006f0: 6969 5f6c 6574 7465 7273 2c20 7265 7065  ii_letters, repe
+00000700: 6174 3d70 6570 7065 725f 6c65 6e67 7468  at=pepper_length
+00000710: 297d 0a0a 2020 2020 6966 206e 6f74 2075  )}..    if not u
+00000720: 7365 5f6d 756c 7469 7072 6f63 6573 7369  se_multiprocessi
+00000730: 6e67 3a0a 2020 2020 2020 2020 666f 7220  ng:.        for 
+00000740: 6775 6573 7320 696e 205f 6775 6573 7365  guess in _guesse
+00000750: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+00000760: 6620 5f67 7565 7373 5f62 6c6f 636b 280a  f _guess_block(.
+00000770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000780: 7b67 7565 7373 7d2c 0a20 2020 2020 2020  {guess},.       
+00000790: 2020 2020 2020 2020 2069 6e70 7574 5f70           input_p
+000007a0: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
+000007b0: 2020 2020 2020 2020 2064 6174 6162 6173           databas
+000007c0: 655f 7061 7373 776f 7264 2c0a 2020 2020  e_password,.    
+000007d0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+000007e0: 6261 7365 5f73 616c 742c 0a20 2020 2020  base_salt,.     
+000007f0: 2020 2020 2020 2020 2020 2065 6e63 7279             encry
+00000800: 7074 696f 6e5f 6c65 7665 6c2c 0a20 2020  ption_level,.   
+00000810: 2020 2020 2020 2020 2020 2020 2070 6570               pep
+00000820: 7065 725f 706f 7369 7469 6f6e 2c0a 2020  per_position,.  
+00000830: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+00000840: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00000850: 7572 6e20 5472 7565 0a0a 2020 2020 2020  urn True..      
+00000860: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+00000870: 2020 2020 7468 7265 6164 5f70 6f6f 6c20      thread_pool 
+00000880: 3d20 6d75 6c74 6970 726f 6365 7373 696e  = multiprocessin
+00000890: 672e 506f 6f6c 2870 726f 6365 7373 6573  g.Pool(processes
+000008a0: 3d70 6570 7065 725f 6c65 6e67 7468 290a  =pepper_length).
+000008b0: 2020 2020 7468 7265 6164 7320 3d20 5b5d      threads = []
+000008c0: 0a0a 2020 2020 666f 7220 6261 7463 6820  ..    for batch 
+000008d0: 696e 2062 6174 6368 6564 285f 6775 6573  in batched(_gues
+000008e0: 7365 732c 2031 3030 3029 3a0a 2020 2020  ses, 1000):.    
+000008f0: 2020 2020 7468 7265 6164 732e 6170 7065      threads.appe
+00000900: 6e64 280a 2020 2020 2020 2020 2020 2020  nd(.            
+00000910: 7468 7265 6164 5f70 6f6f 6c2e 6170 706c  thread_pool.appl
+00000920: 795f 6173 796e 6328 0a20 2020 2020 2020  y_async(.       
+00000930: 2020 2020 2020 2020 205f 6775 6573 735f           _guess_
+00000940: 626c 6f63 6b2c 0a20 2020 2020 2020 2020  block,.         
+00000950: 2020 2020 2020 2061 7267 733d 280a 2020         args=(.  
+00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000970: 2020 6261 7463 682c 0a20 2020 2020 2020    batch,.       
+00000980: 2020 2020 2020 2020 2020 2020 2069 6e70               inp
+00000990: 7574 5f70 6173 7377 6f72 642c 0a20 2020  ut_password,.   
+000009a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009b0: 2064 6174 6162 6173 655f 7061 7373 776f   database_passwo
+000009c0: 7264 2c0a 2020 2020 2020 2020 2020 2020  rd,.            
+000009d0: 2020 2020 2020 2020 6461 7461 6261 7365          database
+000009e0: 5f73 616c 742c 0a20 2020 2020 2020 2020  _salt,.         
+000009f0: 2020 2020 2020 2020 2020 2065 6e63 7279             encry
+00000a00: 7074 696f 6e5f 6c65 7665 6c2c 0a20 2020  ption_level,.   
+00000a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a20: 2070 6570 7065 725f 706f 7369 7469 6f6e   pepper_position
+00000a30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000a40: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+00000a50: 2029 0a20 2020 2020 2020 2029 0a0a 2020   ).        )..  
+00000a60: 2020 666f 7220 7468 7265 6164 2069 6e20    for thread in 
+00000a70: 7468 7265 6164 733a 0a20 2020 2020 2020  threads:.       
+00000a80: 2069 6620 7468 7265 6164 2e67 6574 2829   if thread.get()
+00000a90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00000aa0: 7475 726e 2054 7275 650a 0a20 2020 2072  turn True..    r
+00000ab0: 6574 7572 6e20 4661 6c73 650a            eturn False.
```

### Comparing `flask_imp-4.0.1/flask_imp/__init__.py` & `flask_imp-4.0.2/flask_imp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .config_imp_blueprint_template import (
     ImpBlueprintConfigTemplate as ImpBlueprintConfig,
 )
 from .config_imp_template import ImpConfigTemplate as ImpConfig
 from .imp import Imp as Imp
 from .imp_blueprint import ImpBlueprint as Blueprint
 
-__version__ = "4.0.1"
+__version__ = "4.0.2"
 
 __all__ = [
     "Auth",
     "PasswordGeneration",
     "Imp",
     "Blueprint",
     "ImpConfig",
```

### Comparing `flask_imp-4.0.1/flask_imp/_cli/__init__.py` & `flask_imp-4.0.2/flask_imp/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/_cli/blueprint.py` & `flask_imp-4.0.2/flask_imp/_cli/blueprint.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/_cli/filelib/all_files.py` & `flask_imp-4.0.2/flask_imp/_cli/filelib/all_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,14 @@
     collections_routes_py = """\
 from flask import current_app as app
 from flask import render_template
 
 
 @app.route("/resources")
 def index():
-    head = Head(title="Flask Imp Global Template")
     return render_template("index.html")
 """
 
     minimal_collections_routes_py = """\
 from flask import current_app as app
 from flask import render_template
```

### Comparing `flask_imp-4.0.1/flask_imp/_cli/filelib/app.py` & `flask_imp-4.0.2/flask_imp/_cli/filelib/app.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/_cli/filelib/blueprint.py` & `flask_imp-4.0.2/flask_imp/_cli/filelib/blueprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     # ROOT_PATH: str = ""
     # CLI_GROUP: str = ""
 
     INIT_SESSION: dict = {{
         "{name}_session": "yes"
     }}
 
-    DATABASE_BINDS: = {{
+    DATABASE_BINDS: dict[DatabaseConfig] = {{
         DatabaseConfig(
             ENABLED=False,
             DIALECT="sqlite",
             NAME="{name}",
             BIND_KEY="{name}",
             LOCATION="",
             PORT=0,
```

### Comparing `flask_imp-4.0.1/flask_imp/_cli/filelib/favicon.py` & `flask_imp-4.0.2/flask_imp/_cli/filelib/favicon.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/_cli/filelib/flask_imp_logo.py` & `flask_imp-4.0.2/flask_imp/_cli/filelib/flask_imp_logo.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/_cli/filelib/head_tag_generator.py` & `flask_imp-4.0.2/flask_imp/_cli/filelib/head_tag_generator.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/_cli/filelib/water_css.py` & `flask_imp-4.0.2/flask_imp/_cli/filelib/water_css.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/_cli/helpers.py` & `flask_imp-4.0.2/flask_imp/_cli/helpers.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/_cli/init.py` & `flask_imp-4.0.2/flask_imp/_cli/init.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/auth/__init__.py` & `flask_imp-4.0.2/flask_imp/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/auth/__legacy__.py` & `flask_imp-4.0.2/flask_imp/auth/__legacy__.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/auth/__private_funcs__.py` & `flask_imp-4.0.2/flask_imp/auth/__private_funcs__.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/auth/dataclasses.py` & `flask_imp-4.0.2/flask_imp/auth/dataclasses.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/auth/encrypt_password.py` & `flask_imp-4.0.2/flask_imp/auth/encrypt_password.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/auth/generate_alphanumeric_validator.py` & `flask_imp-4.0.2/flask_imp/auth/generate_alphanumeric_validator.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/auth/generate_email_validator.py` & `flask_imp-4.0.2/flask_imp/auth/generate_email_validator.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/auth/generate_numeric_validator.py` & `flask_imp-4.0.2/flask_imp/auth/generate_numeric_validator.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/auth/generate_password.py` & `flask_imp-4.0.2/flask_imp/auth/generate_password.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/auth/generate_private_key.py` & `flask_imp-4.0.2/flask_imp/auth/generate_private_key.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/auth/is_email_address_valid.py` & `flask_imp-4.0.2/flask_imp/auth/is_email_address_valid.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/auth/is_username_valid.py` & `flask_imp-4.0.2/flask_imp/auth/is_username_valid.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/config_database_template.py` & `flask_imp-4.0.2/flask_imp/config_database_template.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/config_flask_template.py` & `flask_imp-4.0.2/flask_imp/config_flask_template.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/config_imp_blueprint_template.py` & `flask_imp-4.0.2/flask_imp/config_imp_blueprint_template.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/config_imp_template.py` & `flask_imp-4.0.2/flask_imp/config_imp_template.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/config_object_parser.py` & `flask_imp-4.0.2/flask_imp/config_object_parser.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/config_toml_parser.py` & `flask_imp-4.0.2/flask_imp/config_toml_parser.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/imp.py` & `flask_imp-4.0.2/flask_imp/imp.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/imp_blueprint.py` & `flask_imp-4.0.2/flask_imp/imp_blueprint.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/protocols.py` & `flask_imp-4.0.2/flask_imp/protocols.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/registeries.py` & `flask_imp-4.0.2/flask_imp/registeries.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/security/__private_funcs__.py` & `flask_imp-4.0.2/flask_imp/security/__private_funcs__.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/security/api_login_check.py` & `flask_imp-4.0.2/flask_imp/security/api_login_check.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/security/include_csrf.py` & `flask_imp-4.0.2/flask_imp/security/include_csrf.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/security/login_check.py` & `flask_imp-4.0.2/flask_imp/security/login_check.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/security/pass_function_check.py` & `flask_imp-4.0.2/flask_imp/security/pass_function_check.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/security/permission_check.py` & `flask_imp-4.0.2/flask_imp/security/permission_check.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/flask_imp/utilities.py` & `flask_imp-4.0.2/flask_imp/utilities.py`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/pyproject.toml` & `flask_imp-4.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_imp-4.0.1/PKG-INFO` & `flask_imp-4.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-imp
-Version: 4.0.1
+Version: 4.0.2
 Summary: A Flask auto importer that allows your Flask apps to grow big.
 Author-email: David Carmichael <david@uilix.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -126,16 +126,15 @@
 ```bash
 .\venv\Scripts\activate
 ```
 
 ### Install the requirements.
 
 ```bash
-pip install -r requirements.txt
-pip install -r requirements_dev.txt
+pip install -r requirements/development.txt
 ```
 
 ### Install the local version of Flask-Imp.
 
 ```bash
 flit install
 ```
@@ -166,18 +165,20 @@
 
 The test Flask app is located in the `tests/test_app` folder. 
 
 The tests are linked to the tests blueprint located at `test_app/blueprints/tests`.
 
 ### Building the docs.
 
-All docs are generated from the [docs_md](docs_md) folder. Edit these files then run the following command to generate the docs.
+All docs are generated from the [docs](docs) folder. 
+
+Edit these files, then run the following command to generate the docs.
 
 ```bash
-flask --app gdocs compile
+flask --app docs compile
 ```
 
 You can set it to watch for changes and automatically recompile the docs by adding the `--watch` flag.
 
 ```bash
 flask --app gdocs compile --watch
 ```
```

