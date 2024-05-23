# Comparing `tmp/qbraid_cli-0.8.1.tar.gz` & `tmp/qbraid_cli-0.8.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid_cli-0.8.1.tar", last modified: Thu May 23 20:33:33 2024, max compression
+gzip compressed data, was "qbraid_cli-0.8.1a0.tar", last modified: Wed Apr 24 21:39:40 2024, max compression
```

## Comparing `qbraid_cli-0.8.1.tar` & `qbraid_cli-0.8.1a0.tar`

### file list

```diff
@@ -1,155 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.336829 qbraid_cli-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.312829 qbraid_cli-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.312829 qbraid_cli-0.8.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.312829 qbraid_cli-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/.github/workflows/pre-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/MANIFEST.IN
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-23 20:33:33.336829 qbraid_cli-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.316829 qbraid_cli-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.316829 qbraid_cli-0.8.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    30522 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/_static/api-key.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.316829 qbraid_cli-0.8.1/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/_static/cards/terminal.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.316829 qbraid_cli-0.8.1/docs/_static/style/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/_static/style/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/_static/style/s4defs-roles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.320829 qbraid_cli-0.8.1/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/cli/configure.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/cli/credits.rst
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/cli/devices-list.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/cli/devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/cli/envs-activate.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/cli/envs-list.rst
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/cli/envs-uninstall.rst
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/cli/envs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/cli/jobs-add.rst
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/cli/jobs-disable.rst
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/cli/jobs-enable.rst
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/cli/jobs-list.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/cli/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/cli/kernels.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/cli/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.320829 qbraid_cli-0.8.1/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/guide/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.320829 qbraid_cli-0.8.1/qbraid_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-23 20:33:33.000000 qbraid_cli-0.8.1/qbraid_cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.324829 qbraid_cli-0.8.1/qbraid_cli/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/admin/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/admin/buildlogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/admin/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/admin/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.324829 qbraid_cli-0.8.1/qbraid_cli/configure/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/configure/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/configure/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.324829 qbraid_cli-0.8.1/qbraid_cli/credits/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/credits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/credits/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.324829 qbraid_cli-0.8.1/qbraid_cli/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/devices/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/devices/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.324829 qbraid_cli-0.8.1/qbraid_cli/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/envs/activate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/envs/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/envs/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/envs/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.324829 qbraid_cli-0.8.1/qbraid_cli/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/jobs/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/jobs/toggle_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/jobs/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.328829 qbraid_cli-0.8.1/qbraid_cli/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/kernels/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.328829 qbraid_cli-0.8.1/qbraid_cli/pip/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/pip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/pip/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/pip/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/qbraid_cli/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.336829 qbraid_cli-0.8.1/qbraid_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-23 20:33:33.000000 qbraid_cli-0.8.1/qbraid_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-23 20:33:33.000000 qbraid_cli-0.8.1/qbraid_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:33:33.000000 qbraid_cli-0.8.1/qbraid_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 20:33:33.000000 qbraid_cli-0.8.1/qbraid_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-23 20:33:33.000000 qbraid_cli-0.8.1/qbraid_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 20:33:33.000000 qbraid_cli-0.8.1/qbraid_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:33:33.336829 qbraid_cli-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.328829 qbraid_cli-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.328829 qbraid_cli-0.8.1/tests/configure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/configure/test_configure_prompt_for_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/configure/test_configure_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/configure/test_configure_validate_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.328829 qbraid_cli-0.8.1/tests/credits/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/credits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/credits/test_credits_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.328829 qbraid_cli-0.8.1/tests/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/devices/test_devices_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/devices/test_devices_validations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.332829 qbraid_cli-0.8.1/tests/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/envs/test_envs_activate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/envs/test_envs_activate_find_shell_rc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/envs/test_envs_activate_print_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/envs/test_envs_activate_pyenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/envs/test_envs_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/envs/test_envs_create_qbraid_env_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/envs/test_envs_create_validate_env_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/envs/test_envs_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/envs/test_envs_remove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.332829 qbraid_cli-0.8.1/tests/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/jobs/test_jobs_disable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/jobs/test_jobs_enable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/jobs/test_jobs_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/jobs/test_jobs_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/jobs/test_jobs_toggle_braket_confirm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/jobs/test_jobs_toggle_braket_disable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/jobs/test_jobs_toggle_braket_enable.py
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/jobs/test_jobs_toggle_braket_get_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/jobs/test_jobs_validate_get_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/jobs/test_jobs_validate_handle_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/jobs/test_jobs_validate_library.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.332829 qbraid_cli-0.8.1/tests/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tests/kernels/test_kernels_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:33:33.336829 qbraid_cli-0.8.1/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2584 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tools/create_dev_build.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1849 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tools/install_wheel_extras.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tools/split_md.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4026 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tools/split_rst.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1401 2024-05-23 20:33:29.000000 qbraid_cli-0.8.1/tools/stamp_pre_release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.443476 qbraid_cli-0.8.1a0/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.419476 qbraid_cli-0.8.1a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.419476 qbraid_cli-0.8.1a0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.423476 qbraid_cli-0.8.1a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/.github/workflows/pre-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/MANIFEST.IN
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-24 21:39:40.443476 qbraid_cli-0.8.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.423476 qbraid_cli-0.8.1a0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.423476 qbraid_cli-0.8.1a0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    30522 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/_static/api-key.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.423476 qbraid_cli-0.8.1a0/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/_static/cards/terminal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.423476 qbraid_cli-0.8.1a0/docs/_static/style/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/_static/style/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/_static/style/s4defs-roles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.427476 qbraid_cli-0.8.1a0/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/cli/configure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/cli/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/cli/devices-list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/cli/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/cli/envs-activate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/cli/envs-list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/cli/envs-uninstall.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/cli/envs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/cli/jobs-add.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/cli/jobs-disable.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/cli/jobs-enable.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/cli/jobs-list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/cli/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/cli/kernels.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/cli/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.427476 qbraid_cli-0.8.1a0/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/guide/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.427476 qbraid_cli-0.8.1a0/qbraid_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-24 21:39:40.000000 qbraid_cli-0.8.1a0/qbraid_cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.427476 qbraid_cli-0.8.1a0/qbraid_cli/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/admin/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/admin/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/admin/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.431476 qbraid_cli-0.8.1a0/qbraid_cli/configure/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/configure/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/configure/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.431476 qbraid_cli-0.8.1a0/qbraid_cli/credits/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/credits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/credits/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.431476 qbraid_cli-0.8.1a0/qbraid_cli/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/devices/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/devices/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.431476 qbraid_cli-0.8.1a0/qbraid_cli/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/envs/activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/envs/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/envs/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/envs/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.431476 qbraid_cli-0.8.1a0/qbraid_cli/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/jobs/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/jobs/toggle_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/jobs/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.431476 qbraid_cli-0.8.1a0/qbraid_cli/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/kernels/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/qbraid_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.439476 qbraid_cli-0.8.1a0/qbraid_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-24 21:39:40.000000 qbraid_cli-0.8.1a0/qbraid_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-24 21:39:40.000000 qbraid_cli-0.8.1a0/qbraid_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:39:40.000000 qbraid_cli-0.8.1a0/qbraid_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 21:39:40.000000 qbraid_cli-0.8.1a0/qbraid_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-24 21:39:40.000000 qbraid_cli-0.8.1a0/qbraid_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 21:39:40.000000 qbraid_cli-0.8.1a0/qbraid_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 21:39:40.443476 qbraid_cli-0.8.1a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.431476 qbraid_cli-0.8.1a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.431476 qbraid_cli-0.8.1a0/tests/test_configure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_configure/test_configure_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_configure/test_prompt_for_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_configure/test_validate_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.435476 qbraid_cli-0.8.1a0/tests/test_credits/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_credits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_credits/test_credits_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.435476 qbraid_cli-0.8.1a0/tests/test_devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_devices/test_devices_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_devices/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.435476 qbraid_cli-0.8.1a0/tests/test_envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.435476 qbraid_cli-0.8.1a0/tests/test_envs/test_activate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_activate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_activate/test_activate_pyenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_activate/test_find_shell_rc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_activate/test_print_activate_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.435476 qbraid_cli-0.8.1a0/tests/test_envs/test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_app/test_envs_activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_app/test_envs_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_app/test_envs_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_app/test_envs_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.435476 qbraid_cli-0.8.1a0/tests/test_envs/test_create/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_create/test_create_qbraid_env_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_create/test_replace_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_create/test_update_state_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.435476 qbraid_cli-0.8.1a0/tests/test_envs/test_data_handling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_data_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_data_handling/test_installed_envs_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_data_handling/test_is_valid_env_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_data_handling/test_request_delete_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_envs/test_data_handling/test_validate_env_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.435476 qbraid_cli-0.8.1a0/tests/test_jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.439476 qbraid_cli-0.8.1a0/tests/test_jobs/test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/test_app/test_jobs_disable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/test_app/test_jobs_enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/test_app/test_jobs_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/test_app/test_jobs_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.439476 qbraid_cli-0.8.1a0/tests/test_jobs/test_toggle_braket/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/test_toggle_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/test_toggle_braket/test_confirm_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/test_toggle_braket/test_disable_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/test_toggle_braket/test_enable_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/test_toggle_braket/test_get_package_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.439476 qbraid_cli-0.8.1a0/tests/test_jobs/test_validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/test_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/test_validation/test_get_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/test_validation/test_handle_jobs_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/test_validation/test_run_progress_get_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_jobs/test_validation/test_validate_library.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.439476 qbraid_cli-0.8.1a0/tests/test_kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tests/test_kernels/test_kernels_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:39:40.439476 qbraid_cli-0.8.1a0/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2584 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tools/create_dev_build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1849 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tools/install_wheel_extras.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3862 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tools/split_rst.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2723 2024-04-24 21:39:30.000000 qbraid_cli-0.8.1a0/tools/stamp_pre_release.py
```

### Comparing `qbraid_cli-0.8.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid_cli-0.8.1a0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid_cli-0.8.1a0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/.github/workflows/docs.yml` & `qbraid_cli-0.8.1a0/.github/workflows/docs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,19 @@
       uses: actions/setup-python@v4
       with:
         python-version: '3.10'
         cache: pip
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools build
-        python -m pip install -r docs/requirements.txt
     - name: Build & install package
       run: |
         python -m build .
         python -m pip install dist/*.whl
+        tools/install_wheel_extras.sh dist --extra docs
     - name: Generate docs assets
       run: |
         python -c "import pathlib; pathlib.Path('docs/tree').mkdir(parents=True, exist_ok=True)"
         python -c "import glob, os; [os.remove(f) for f in glob.glob('docs/tree/*.rst')]"
         typer qbraid_cli.main utils docs --name=qbraid --output=docs/tree/qbraid.md
         m2r docs/tree/qbraid.md
         python -c "import os; os.remove('docs/tree/qbraid.md')"
```

### Comparing `qbraid_cli-0.8.1/.github/workflows/format.yml` & `qbraid_cli-0.8.1a0/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/.github/workflows/main.yml` & `qbraid_cli-0.8.1a0/.github/workflows/main.yml`

 * *Files 13% similar despite different names*

```diff
@@ -60,25 +60,13 @@
             Get-ChildItem dist/*.whl | ForEach-Object { pip install $_.FullName }
           } else {
             pip install dist/*.whl
           }
         shell: pwsh
       - name: Install testing dependencies
         run: |
-          pip install pytest coverage
+          pip install pytest
       - name: Run tests with pytest
         run: |
-          coverage run -m pytest -x tests
-          coverage combine
-          coverage report
-          coverage html
-          coverage xml
+          pytest
         env:
-          QBRAID_API_KEY: ${{ secrets.QBRAID_API_KEY }}
-      - name: Upload coverage to Codecov
-        if: matrix.python-version == '3.11' && matrix.os == 'ubuntu-latest'
-        uses: codecov/codecov-action@v3
-        with:
-          token: ${{ secrets.CODECOV_TOKEN }}
-          fail_ci_if_error: false
-          files: ./build/coverage/coverage.xml
-          verbose: true
+          QBRAID_API_KEY: ${{ secrets.QBRAID_API_KEY }}
```

### Comparing `qbraid_cli-0.8.1/.github/workflows/pre-release.yml` & `qbraid_cli-0.8.1a0/.github/workflows/pre-release.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/.github/workflows/publish.yml` & `qbraid_cli-0.8.1a0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/.gitignore` & `qbraid_cli-0.8.1a0/.gitignore`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/.readthedocs.yml` & `qbraid_cli-0.8.1a0/.readthedocs.yml`

 * *Files 15% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 
 # Set the version of Python and other tools you might need
 build:
   os: ubuntu-20.04
   tools:
     python: "3.10"
   commands:
-    - python -m pip install -r docs/requirements.txt
-    - python -m pip install build
     - python -m build .
     - python -m pip install dist/*.whl
+    - tools/install_wheel_extras.sh dist --extra docs
     - mkdir -p docs/tree
     - rm -f docs/tree/*.rst
     - typer qbraid_cli.main utils docs --name=qbraid --output=docs/tree/qbraid.md
     - m2r docs/tree/qbraid.md
     - rm docs/tree/qbraid.md
     - python tools/split_rst.py docs/tree/qbraid.rst
     - sphinx-build -W -b html docs $READTHEDOCS_OUTPUT/html
```

### Comparing `qbraid_cli-0.8.1/Makefile` & `qbraid_cli-0.8.1a0/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/PKG-INFO` & `qbraid_cli-0.8.1a0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-cli
-Version: 0.8.1
+Version: 0.8.1a0
 Summary: Command Line Interface for interacting with all parts of the qBraid platform.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
@@ -22,35 +22,43 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: typer>=0.12.1
 Requires-Dist: rich>=10.11.0
 Requires-Dist: jupyter_client<9.0.0,>=7.0.0
 Requires-Dist: ipykernel
-Requires-Dist: qbraid-core>=0.1.10
+Requires-Dist: qbraid-core>=0.1.4
 Provides-Extra: jobs
 Requires-Dist: amazon-braket-sdk>=1.48.1; extra == "jobs"
 Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: isort; extra == "dev"
 Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: sphinx<7.4.0,>=7.2.6; extra == "docs"
+Requires-Dist: sphinx-rtd-theme<2.1,>=1.3; extra == "docs"
+Requires-Dist: docutils<0.22; extra == "docs"
+Requires-Dist: toml; extra == "docs"
+Requires-Dist: build; extra == "docs"
+Requires-Dist: m2r; extra == "docs"
+Requires-Dist: typer; extra == "docs"
 
 <img width="full" alt="qbraid_cli" src="https://qbraid-static.s3.amazonaws.com/logos/qbraid-cli-banner.png">
 
 [![Documentation](https://img.shields.io/badge/Documentation-DF0982)](https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html)
 [![PyPI version](https://img.shields.io/pypi/v/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
 [![Python verions](https://img.shields.io/pypi/pyversions/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
 [![Downloads](https://static.pepy.tech/badge/qbraid-cli)](https://pepy.tech/project/qbraid-cli)
 [![GitHub](https://img.shields.io/badge/issue_tracking-github-blue?logo=github)](https://github.com/qBraid/qBraid-Lab/issues)
+[![Discord](https://img.shields.io/discord/771898982564626445.svg?color=pink)](https://discord.gg/KugF6Cnncm)
 
 Command Line Interface for interacting with all parts of the qBraid platform.
 
 The **qBraid CLI** is a versatile command-line interface tool designed for seamless interaction with qBraid cloud services and quantum software management tools. Initially exclusive to the [qBraid Lab](https://docs.qbraid.com/projects/lab/en/latest/lab/overview.html) platform, the CLI now supports local installations as well. This enhancement broadens access to features like [qBraid Quantum Jobs](https://docs.qbraid.com/projects/lab/en/latest/lab/quantum_jobs.html), enabling direct acess to QPU devices from leading providers like IonQ, Oxford Quantum Circuits, QuEra, and Rigetti, as well as on-demand simulators from AWS, all using qBraid credits, with no additional access keys required.
 
 ## Getting Started
 
@@ -59,35 +67,35 @@
 - [Launch qBraid Lab &rarr;](https://lab.qbraid.com/)
 - [Make an account &rarr;](https://account.qbraid.com/)
 
 For help, see qBraid Lab User Guide: [Getting Started](https://docs.qbraid.com/projects/lab/en/latest/lab/getting_started.html).
 
 You can also install the qBraid-CLI from PyPI with:
 
-```bash
+```shell
 pip install qbraid-cli
 ```
 
 ## Local configuration
 
 After installation, you must configure your account credentials to use the CLI locally:
 
 1. Create a qBraid account or log in to your existing account by visiting
    [account.qbraid.com](https://account.qbraid.com/)
 2. Copy your API Key token from the left side of
     your [account page](https://account.qbraid.com/):
 3. Save your API key from step 2 in local configuration file `~/.qbraid/qbraidrc` using:
 
-```bash
+```shell
 $ qbraid configure
 ```
 
 ## Basic Commands
 
-```bash
+```shell
 $ qbraid
 ----------------------------------
   * Welcome to the qBraid CLI! * 
 ----------------------------------
 
         ____            _     _  
    __ _| __ ) _ __ __ _(_) __| | 
@@ -102,35 +110,35 @@
 - Use 'qbraid --version' to see the current version.
 
 Reference Docs: https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 ```
 
 A qBraid CLI command has the following structure:
 
-```bash
+```shell
 $ qbraid <command> <subcommand> [options and parameters]
 ```
 
 For example, to list installed environments, the command would be:
 
-```bash
+```shell
 $ qbraid envs list
 ```
 
 To view help documentation, use one of the following:
 
-```bash
+```shell
 $ qbraid --help
 $ qbraid <command> --help
 $ qbraid <command> <subcommand> --help
 ```
 
 For example:
 
-```bash
+```shell
 $ qbraid --help
 
 Usage: qbraid [OPTIONS] COMMAND [ARGS]...
 
 The qBraid CLI.
 
 Options
@@ -146,23 +154,23 @@
   envs                          Manage qBraid environments.
   jobs                          Manage qBraid quantum jobs.
   kernels                       Manage qBraid kernels.
 ```
 
 To get the version of the qBraid CLI:
 
-```bash
+```shell
 $ qbraid --version
 ```
 
 ## Magic Commands
 
 You can also access the CLI directly from within [Notebooks](https://docs.qbraid.com/projects/lab/en/latest/lab/notebooks.html) using IPython [magic commands](https://ipython.readthedocs.io/en/stable/interactive/magics.html). First, configure the qBraid magic commands extension using:
 
-```bash
+```shell
 $ qbraid configure magic
 ```
 
 The above command can also be executed from within a Jupyter notebook using the ``!`` operator. Then, from within a notebook cell, load the qBraid magic IPython extension using:
 
 ```python
 In [1]: %load_ext qbraid_magic
```

### Comparing `qbraid_cli-0.8.1/README.md` & `qbraid_cli-0.8.1a0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <img width="full" alt="qbraid_cli" src="https://qbraid-static.s3.amazonaws.com/logos/qbraid-cli-banner.png">
 
 [![Documentation](https://img.shields.io/badge/Documentation-DF0982)](https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html)
 [![PyPI version](https://img.shields.io/pypi/v/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
 [![Python verions](https://img.shields.io/pypi/pyversions/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
 [![Downloads](https://static.pepy.tech/badge/qbraid-cli)](https://pepy.tech/project/qbraid-cli)
 [![GitHub](https://img.shields.io/badge/issue_tracking-github-blue?logo=github)](https://github.com/qBraid/qBraid-Lab/issues)
+[![Discord](https://img.shields.io/discord/771898982564626445.svg?color=pink)](https://discord.gg/KugF6Cnncm)
 
 Command Line Interface for interacting with all parts of the qBraid platform.
 
 The **qBraid CLI** is a versatile command-line interface tool designed for seamless interaction with qBraid cloud services and quantum software management tools. Initially exclusive to the [qBraid Lab](https://docs.qbraid.com/projects/lab/en/latest/lab/overview.html) platform, the CLI now supports local installations as well. This enhancement broadens access to features like [qBraid Quantum Jobs](https://docs.qbraid.com/projects/lab/en/latest/lab/quantum_jobs.html), enabling direct acess to QPU devices from leading providers like IonQ, Oxford Quantum Circuits, QuEra, and Rigetti, as well as on-demand simulators from AWS, all using qBraid credits, with no additional access keys required.
 
 ## Getting Started
 
@@ -17,35 +18,35 @@
 - [Launch qBraid Lab &rarr;](https://lab.qbraid.com/)
 - [Make an account &rarr;](https://account.qbraid.com/)
 
 For help, see qBraid Lab User Guide: [Getting Started](https://docs.qbraid.com/projects/lab/en/latest/lab/getting_started.html).
 
 You can also install the qBraid-CLI from PyPI with:
 
-```bash
+```shell
 pip install qbraid-cli
 ```
 
 ## Local configuration
 
 After installation, you must configure your account credentials to use the CLI locally:
 
 1. Create a qBraid account or log in to your existing account by visiting
    [account.qbraid.com](https://account.qbraid.com/)
 2. Copy your API Key token from the left side of
     your [account page](https://account.qbraid.com/):
 3. Save your API key from step 2 in local configuration file `~/.qbraid/qbraidrc` using:
 
-```bash
+```shell
 $ qbraid configure
 ```
 
 ## Basic Commands
 
-```bash
+```shell
 $ qbraid
 ----------------------------------
   * Welcome to the qBraid CLI! * 
 ----------------------------------
 
         ____            _     _  
    __ _| __ ) _ __ __ _(_) __| | 
@@ -60,35 +61,35 @@
 - Use 'qbraid --version' to see the current version.
 
 Reference Docs: https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 ```
 
 A qBraid CLI command has the following structure:
 
-```bash
+```shell
 $ qbraid <command> <subcommand> [options and parameters]
 ```
 
 For example, to list installed environments, the command would be:
 
-```bash
+```shell
 $ qbraid envs list
 ```
 
 To view help documentation, use one of the following:
 
-```bash
+```shell
 $ qbraid --help
 $ qbraid <command> --help
 $ qbraid <command> <subcommand> --help
 ```
 
 For example:
 
-```bash
+```shell
 $ qbraid --help
 
 Usage: qbraid [OPTIONS] COMMAND [ARGS]...
 
 The qBraid CLI.
 
 Options
@@ -104,23 +105,23 @@
   envs                          Manage qBraid environments.
   jobs                          Manage qBraid quantum jobs.
   kernels                       Manage qBraid kernels.
 ```
 
 To get the version of the qBraid CLI:
 
-```bash
+```shell
 $ qbraid --version
 ```
 
 ## Magic Commands
 
 You can also access the CLI directly from within [Notebooks](https://docs.qbraid.com/projects/lab/en/latest/lab/notebooks.html) using IPython [magic commands](https://ipython.readthedocs.io/en/stable/interactive/magics.html). First, configure the qBraid magic commands extension using:
 
-```bash
+```shell
 $ qbraid configure magic
 ```
 
 The above command can also be executed from within a Jupyter notebook using the ``!`` operator. Then, from within a notebook cell, load the qBraid magic IPython extension using:
 
 ```python
 In [1]: %load_ext qbraid_magic
```

### Comparing `qbraid_cli-0.8.1/docs/Makefile` & `qbraid_cli-0.8.1a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/_static/api-key.png` & `qbraid_cli-0.8.1a0/docs/_static/api-key.png`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/_static/cards/jupyter.png` & `qbraid_cli-0.8.1a0/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/_static/cards/python.png` & `qbraid_cli-0.8.1a0/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/_static/cards/terminal.png` & `qbraid_cli-0.8.1a0/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/_static/favicon.ico` & `qbraid_cli-0.8.1a0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/_static/logo.png` & `qbraid_cli-0.8.1a0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/_static/style/custom.css` & `qbraid_cli-0.8.1a0/docs/_static/style/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/_static/style/s4defs-roles.css` & `qbraid_cli-0.8.1a0/docs/_static/style/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/cli/configure.rst` & `qbraid_cli-0.8.1a0/docs/cli/configure.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/cli/devices-list.rst` & `qbraid_cli-0.8.1a0/docs/cli/devices-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/cli/envs-activate.rst` & `qbraid_cli-0.8.1a0/docs/cli/envs-activate.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/cli/envs-list.rst` & `qbraid_cli-0.8.1a0/docs/cli/envs-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/cli/envs-uninstall.rst` & `qbraid_cli-0.8.1a0/docs/cli/envs-uninstall.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/cli/envs.rst` & `qbraid_cli-0.8.1a0/docs/cli/envs.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/cli/jobs-add.rst` & `qbraid_cli-0.8.1a0/docs/cli/jobs-add.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/cli/jobs-disable.rst` & `qbraid_cli-0.8.1a0/docs/cli/jobs-disable.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/cli/jobs-enable.rst` & `qbraid_cli-0.8.1a0/docs/cli/jobs-enable.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/cli/jobs-list.rst` & `qbraid_cli-0.8.1a0/docs/cli/jobs-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/cli/jobs.rst` & `qbraid_cli-0.8.1a0/docs/cli/jobs.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/cli/kernels.rst` & `qbraid_cli-0.8.1a0/docs/cli/kernels.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/cli/qbraid.rst` & `qbraid_cli-0.8.1a0/docs/cli/qbraid.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/conf.py` & `qbraid_cli-0.8.1a0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/guide/overview.rst` & `qbraid_cli-0.8.1a0/docs/guide/overview.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/docs/index.rst` & `qbraid_cli-0.8.1a0/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -105,9 +105,8 @@
    tree/qbraid
    tree/qbraid_admin
    tree/qbraid_configure
    tree/qbraid_credits
    tree/qbraid_devices
    tree/qbraid_envs
    tree/qbraid_jobs
-   tree/qbraid_kernels
-   tree/qbraid_pip
+   tree/qbraid_kernels
```

#### html2text {}

```diff
@@ -6,8 +6,8 @@
 _**_**_**_**_ _CC_LL_II_ _**_**_**_**
 _[_t_e_r_m_i_n_a_l_]
 _**_**_**_**_ _SS_DD_KK_ _**_**_**_**
 _[_t_e_r_m_i_n_a_l_]
 | .. toctree:: :maxdepth: 1 :caption: CLI User Guide :hidden: guide/overview ..
 toctree:: :maxdepth: 1 :caption: CLI API Reference :hidden: tree/qbraid tree/
 qbraid_admin tree/qbraid_configure tree/qbraid_credits tree/qbraid_devices
-tree/qbraid_envs tree/qbraid_jobs tree/qbraid_kernels tree/qbraid_pip
+tree/qbraid_envs tree/qbraid_jobs tree/qbraid_kernels
```

### Comparing `qbraid_cli-0.8.1/docs/make.bat` & `qbraid_cli-0.8.1a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/pyproject.toml` & `qbraid_cli-0.8.1a0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-cli"
-version = "0.8.1"
+version = "0.8.1-alpha"
 description = "Command Line Interface for interacting with all parts of the qBraid platform."
 readme = "README.md"
 authors = [{ name = "qBraid Development Team", email = "contact@qbraid.com" }]
 license = { text = "Proprietary" }
 keywords = ["qbraid", "cli", "quantum", "cloud"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -27,28 +27,29 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "typer>=0.12.1",
     "rich>=10.11.0",
     "jupyter_client>=7.0.0,<9.0.0",
     "ipykernel",
-    "qbraid-core>=0.1.10",
+    "qbraid-core>=0.1.4",
 ]
 requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://www.qbraid.com/"
 Documentation = "https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html"
 "Bug Tracker" = "https://github.com/qBraid/qBraid-Lab/issues"
 Discord = "https://discord.gg/KugF6Cnncm"
 "Launch on Lab" = "https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid-Lab.git"
 
 [project.optional-dependencies]
 jobs = ["amazon-braket-sdk>=1.48.1"]
-dev = ["ruff", "isort", "black", "pytest"]
+dev = ["black", "isort", "pylint", "pytest"]
+docs = ["sphinx>=7.2.6,<7.4.0", "sphinx-rtd-theme>=1.3,<2.1", "docutils<0.22", "toml", "build", "m2r", "typer"]
 
 [project.scripts]
 qbraid = "qbraid_cli.main:app"
 
 [tool.setuptools_scm]
 write_to = "qbraid_cli/_version.py"
 
@@ -72,30 +73,7 @@
 ignore-paths = [
   "^.*\\_version.py$",
 ]
 
 [tool.pytest.ini_options]
 addopts = "-ra"
 testpaths = ["tests"]
-
-[tool.coverage.run]
-parallel = true
-source = ["qbraid_cli"]
-
-[tool.coverage.report]
-show_missing = true
-skip_covered = true
-ignore_errors = true
-exclude_lines = [
-  "raise NotImplementedError",
-  "return NotImplemented",
-  "def __repr__",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
-  "logger.debug"
-]
-
-[tool.coverage.html]
-directory = "build/coverage"
-
-[tool.coverage.xml]
-output = "build/coverage/coverage.xml"
```

### Comparing `qbraid_cli-0.8.1/qbraid_cli/admin/app.py` & `qbraid_cli-0.8.1a0/qbraid_cli/admin/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Copyright (c) 2024, qBraid Development Team
 # All rights reserved.
 
 """
 Module defining commands in the 'qbraid admin' namespace.
+
 """
 
 from typing import List
 
 import typer
 
-from qbraid_cli.admin.buildlogs import buildlogs_app
 from qbraid_cli.admin.headers import check_and_fix_headers
 from qbraid_cli.admin.validation import validate_header_type, validate_paths_exist
 
+# disable pretty_exceptions_show_locals to avoid printing sensative information in the traceback
 admin_app = typer.Typer(
-    help="CI/CD commands for qBraid maintainers.", pretty_exceptions_show_locals=False
+    help="CI/CD commands for qBraid maintainers.",
+    pretty_exceptions_show_locals=False,
 )
-admin_app.add_typer(buildlogs_app, name="buildlogs")
 
 
 @admin_app.command(name="headers")
 def admin_headers(
     src_paths: List[str] = typer.Argument(
         ..., help="Source file or directory paths to verify.", callback=validate_paths_exist
     ),
```

### Comparing `qbraid_cli-0.8.1/qbraid_cli/admin/headers.py` & `qbraid_cli-0.8.1a0/qbraid_cli/admin/headers.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/qbraid_cli/admin/validation.py` & `qbraid_cli-0.8.1a0/qbraid_cli/admin/validation.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/qbraid_cli/configure/actions.py` & `qbraid_cli-0.8.1a0/qbraid_cli/configure/actions.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/qbraid_cli/configure/app.py` & `qbraid_cli-0.8.1a0/qbraid_cli/configure/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/qbraid_cli/credits/app.py` & `qbraid_cli-0.8.1a0/qbraid_cli/credits/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/qbraid_cli/devices/app.py` & `qbraid_cli-0.8.1a0/qbraid_cli/devices/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/qbraid_cli/devices/validation.py` & `qbraid_cli-0.8.1a0/qbraid_cli/devices/validation.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/qbraid_cli/envs/activate.py` & `qbraid_cli-0.8.1a0/qbraid_cli/envs/activate.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/qbraid_cli/envs/app.py` & `qbraid_cli-0.8.1a0/qbraid_cli/envs/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,27 +6,22 @@
 
 """
 
 import shutil
 import subprocess
 import sys
 from pathlib import Path
-from typing import TYPE_CHECKING, Optional, Tuple
+from typing import Any, Dict, Optional, Tuple
 
 import typer
 from rich.console import Console
 
-from qbraid_cli.envs.create import create_qbraid_env_assets, create_venv
-from qbraid_cli.envs.data_handling import get_envs_data as installed_envs_data
-from qbraid_cli.envs.data_handling import validate_env_name
+from qbraid_cli.envs.data_handling import installed_envs_data, request_delete_env, validate_env_name
 from qbraid_cli.handlers import QbraidException, run_progress_task
 
-if TYPE_CHECKING:
-    from qbraid_core.services.environments.client import EnvironmentManagerClient as EMC
-
 envs_app = typer.Typer(help="Manage qBraid environments.")
 
 
 @envs_app.command(name="create")
 def envs_create(  # pylint: disable=too-many-statements
     name: str = typer.Option(
         ..., "--name", "-n", help="Name of the environment to create", callback=validate_env_name
@@ -35,22 +30,33 @@
         None, "--description", "-d", help="Short description of the environment"
     ),
     auto_confirm: bool = typer.Option(
         False, "--yes", "-y", help="Automatically answer 'yes' to all prompts"
     ),
 ) -> None:
     """Create a new qBraid environment."""
-    env_description = description or ""
+    from .create import create_qbraid_env_assets, create_venv
+
+    def request_new_env(req_body: Dict[str, str]) -> Dict[str, Any]:
+        """Send request to create new environment and return the slug."""
+        from qbraid_core import QbraidSession, RequestsApiError
+
+        session = QbraidSession()
+
+        try:
+            env_data = session.post("/environments/create", json=req_body).json()
+        except RequestsApiError as err:
+            raise QbraidException("Create environment request failed") from err
 
-    def create_environment(*args, **kwargs) -> "Tuple[dict, EMC]":
-        """Create a qBraid environment."""
-        from qbraid_core.services.environments.client import EnvironmentManagerClient
+        if env_data is None or len(env_data) == 0 or env_data.get("slug") is None:
+            raise QbraidException(
+                "Create environment request responsed with invalid environment data"
+            )
 
-        client = EnvironmentManagerClient()
-        return client.create_environment(*args, **kwargs), client
+        return env_data
 
     def gather_local_data() -> Tuple[Path, str]:
         """Gather environment data and return the slug."""
         from qbraid_core.services.environments import get_default_envs_paths
 
         env_path = get_default_envs_paths()[0]
 
@@ -61,27 +67,38 @@
             check=True,
         )
 
         python_version = result.stdout or result.stderr
 
         return env_path, python_version
 
-    environment, emc = run_progress_task(
-        create_environment,
-        name,
-        env_description,
+    req_body = {
+        "name": name,
+        "description": description or "",
+        "tags": "",  # comma separated list of tags
+        "code": "",  # newline separated list of packages
+        "visibility": "private",
+        "kernelName": "",
+        "prompt": "",
+        "origin": "CLI",
+    }
+
+    environment = run_progress_task(
+        request_new_env,
+        req_body,
         description="Validating request...",
         error_message="Failed to create qBraid environment",
     )
 
     env_path, python_version = run_progress_task(
         gather_local_data,
         description="Solving environment...",
         error_message="Failed to create qBraid environment",
     )
+
     slug = environment.get("slug")
     display_name = environment.get("displayName")
     prompt = environment.get("prompt")
     description = environment.get("description")
     tags = environment.get("tags")
     kernel_name = environment.get("kernelName")
 
@@ -99,15 +116,15 @@
     typer.echo("\n\n## Environment Plan ##\n")
     typer.echo(f"  location: {slug_path}")
     typer.echo(f"  version: {python_version}\n")
 
     user_confirmation = auto_confirm or typer.confirm("Proceed", default=True)
     typer.echo("")
     if not user_confirmation:
-        emc.delete_environment(slug)
+        request_delete_env(slug)
         typer.echo("qBraidSystemExit: Exiting.")
         raise typer.Exit()
 
     run_progress_task(
         create_qbraid_env_assets,
         slug,
         prompt,
@@ -144,21 +161,14 @@
     name: str = typer.Option(..., "-n", "--name", help="Name of the environment to remove"),
     auto_confirm: bool = typer.Option(
         False, "--yes", "-y", help="Automatically answer 'yes' to all prompts"
     ),
 ) -> None:
     """Delete a qBraid environment."""
 
-    def delete_environment(slug: str) -> None:
-        """Delete a qBraid environment."""
-        from qbraid_core.services.environments.client import EnvironmentManagerClient
-
-        emc = EnvironmentManagerClient()
-        emc.delete_environment(slug)
-
     def gather_local_data(env_name: str) -> Tuple[Path, str]:
         """Get environment path and slug from name (alias)."""
         installed, aliases = installed_envs_data()
         for alias, slug in aliases.items():
             if alias == env_name:
                 path = installed[slug]
 
@@ -176,15 +186,15 @@
         "This operation CANNOT be undone.\n\n"
         "Are you sure you want to continue?"
     )
 
     if auto_confirm or typer.confirm(confirmation_message, abort=True):
         typer.echo("")
         run_progress_task(
-            delete_environment,
+            request_delete_env,
             slug,
             description="Deleting remote environment data...",
             error_message="Failed to delete qBraid environment",
         )
 
         run_progress_task(
             shutil.rmtree,
```

### Comparing `qbraid_cli-0.8.1/qbraid_cli/exceptions.py` & `qbraid_cli-0.8.1a0/qbraid_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/qbraid_cli/handlers.py` & `qbraid_cli-0.8.1a0/qbraid_cli/handlers.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/qbraid_cli/jobs/app.py` & `qbraid_cli-0.8.1a0/qbraid_cli/jobs/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/qbraid_cli/jobs/toggle_braket.py` & `qbraid_cli-0.8.1a0/qbraid_cli/jobs/toggle_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/qbraid_cli/jobs/validation.py` & `qbraid_cli-0.8.1a0/qbraid_cli/jobs/validation.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/qbraid_cli/kernels/app.py` & `qbraid_cli-0.8.1a0/qbraid_cli/kernels/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,22 @@
 import sys
 from pathlib import Path
 
 import typer
 from jupyter_client.kernelspec import KernelSpecManager
 from rich.console import Console
 
+from qbraid_cli.envs.data_handling import installed_envs_data
 from qbraid_cli.handlers import handle_error
 
 kernels_app = typer.Typer(help="Manage qBraid kernels.")
 
 
 def _get_kernels_path(environment: str) -> Path:
     """Get the path to the kernels directory for the given environment."""
-    # pylint: disable-next=import-outside-toplevel
-    from qbraid_core.services.environments.paths import installed_envs_data
-
     slug_to_path, name_to_slug = installed_envs_data()
 
     if environment in name_to_slug:
         slug = name_to_slug.get(environment, None)
     else:
         slug = environment
```

### Comparing `qbraid_cli-0.8.1/qbraid_cli/main.py` & `qbraid_cli-0.8.1a0/qbraid_cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,26 +11,24 @@
 from qbraid_cli.admin.app import admin_app
 from qbraid_cli.configure.app import configure_app
 from qbraid_cli.credits.app import credits_app
 from qbraid_cli.devices.app import devices_app
 from qbraid_cli.envs.app import envs_app
 from qbraid_cli.jobs.app import jobs_app
 from qbraid_cli.kernels.app import kernels_app
-from qbraid_cli.pip.app import pip_app
 
 app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
 
 app.add_typer(admin_app, name="admin")
 app.add_typer(configure_app, name="configure")
 app.add_typer(credits_app, name="credits")
 app.add_typer(devices_app, name="devices")
 app.add_typer(envs_app, name="envs")
 app.add_typer(jobs_app, name="jobs")
 app.add_typer(kernels_app, name="kernels")
-app.add_typer(pip_app, name="pip")
 
 
 def version_callback(value: bool):
     """Show the version and exit."""
     if value:
         # pylint: disable-next=import-error
         from ._version import __version__  # type: ignore
```

### Comparing `qbraid_cli-0.8.1/qbraid_cli.egg-info/PKG-INFO` & `qbraid_cli-0.8.1a0/qbraid_cli.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-cli
-Version: 0.8.1
+Version: 0.8.1a0
 Summary: Command Line Interface for interacting with all parts of the qBraid platform.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
@@ -22,35 +22,43 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: typer>=0.12.1
 Requires-Dist: rich>=10.11.0
 Requires-Dist: jupyter_client<9.0.0,>=7.0.0
 Requires-Dist: ipykernel
-Requires-Dist: qbraid-core>=0.1.10
+Requires-Dist: qbraid-core>=0.1.4
 Provides-Extra: jobs
 Requires-Dist: amazon-braket-sdk>=1.48.1; extra == "jobs"
 Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: isort; extra == "dev"
 Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: sphinx<7.4.0,>=7.2.6; extra == "docs"
+Requires-Dist: sphinx-rtd-theme<2.1,>=1.3; extra == "docs"
+Requires-Dist: docutils<0.22; extra == "docs"
+Requires-Dist: toml; extra == "docs"
+Requires-Dist: build; extra == "docs"
+Requires-Dist: m2r; extra == "docs"
+Requires-Dist: typer; extra == "docs"
 
 <img width="full" alt="qbraid_cli" src="https://qbraid-static.s3.amazonaws.com/logos/qbraid-cli-banner.png">
 
 [![Documentation](https://img.shields.io/badge/Documentation-DF0982)](https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html)
 [![PyPI version](https://img.shields.io/pypi/v/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
 [![Python verions](https://img.shields.io/pypi/pyversions/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
 [![Downloads](https://static.pepy.tech/badge/qbraid-cli)](https://pepy.tech/project/qbraid-cli)
 [![GitHub](https://img.shields.io/badge/issue_tracking-github-blue?logo=github)](https://github.com/qBraid/qBraid-Lab/issues)
+[![Discord](https://img.shields.io/discord/771898982564626445.svg?color=pink)](https://discord.gg/KugF6Cnncm)
 
 Command Line Interface for interacting with all parts of the qBraid platform.
 
 The **qBraid CLI** is a versatile command-line interface tool designed for seamless interaction with qBraid cloud services and quantum software management tools. Initially exclusive to the [qBraid Lab](https://docs.qbraid.com/projects/lab/en/latest/lab/overview.html) platform, the CLI now supports local installations as well. This enhancement broadens access to features like [qBraid Quantum Jobs](https://docs.qbraid.com/projects/lab/en/latest/lab/quantum_jobs.html), enabling direct acess to QPU devices from leading providers like IonQ, Oxford Quantum Circuits, QuEra, and Rigetti, as well as on-demand simulators from AWS, all using qBraid credits, with no additional access keys required.
 
 ## Getting Started
 
@@ -59,35 +67,35 @@
 - [Launch qBraid Lab &rarr;](https://lab.qbraid.com/)
 - [Make an account &rarr;](https://account.qbraid.com/)
 
 For help, see qBraid Lab User Guide: [Getting Started](https://docs.qbraid.com/projects/lab/en/latest/lab/getting_started.html).
 
 You can also install the qBraid-CLI from PyPI with:
 
-```bash
+```shell
 pip install qbraid-cli
 ```
 
 ## Local configuration
 
 After installation, you must configure your account credentials to use the CLI locally:
 
 1. Create a qBraid account or log in to your existing account by visiting
    [account.qbraid.com](https://account.qbraid.com/)
 2. Copy your API Key token from the left side of
     your [account page](https://account.qbraid.com/):
 3. Save your API key from step 2 in local configuration file `~/.qbraid/qbraidrc` using:
 
-```bash
+```shell
 $ qbraid configure
 ```
 
 ## Basic Commands
 
-```bash
+```shell
 $ qbraid
 ----------------------------------
   * Welcome to the qBraid CLI! * 
 ----------------------------------
 
         ____            _     _  
    __ _| __ ) _ __ __ _(_) __| | 
@@ -102,35 +110,35 @@
 - Use 'qbraid --version' to see the current version.
 
 Reference Docs: https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 ```
 
 A qBraid CLI command has the following structure:
 
-```bash
+```shell
 $ qbraid <command> <subcommand> [options and parameters]
 ```
 
 For example, to list installed environments, the command would be:
 
-```bash
+```shell
 $ qbraid envs list
 ```
 
 To view help documentation, use one of the following:
 
-```bash
+```shell
 $ qbraid --help
 $ qbraid <command> --help
 $ qbraid <command> <subcommand> --help
 ```
 
 For example:
 
-```bash
+```shell
 $ qbraid --help
 
 Usage: qbraid [OPTIONS] COMMAND [ARGS]...
 
 The qBraid CLI.
 
 Options
@@ -146,23 +154,23 @@
   envs                          Manage qBraid environments.
   jobs                          Manage qBraid quantum jobs.
   kernels                       Manage qBraid kernels.
 ```
 
 To get the version of the qBraid CLI:
 
-```bash
+```shell
 $ qbraid --version
 ```
 
 ## Magic Commands
 
 You can also access the CLI directly from within [Notebooks](https://docs.qbraid.com/projects/lab/en/latest/lab/notebooks.html) using IPython [magic commands](https://ipython.readthedocs.io/en/stable/interactive/magics.html). First, configure the qBraid magic commands extension using:
 
-```bash
+```shell
 $ qbraid configure magic
 ```
 
 The above command can also be executed from within a Jupyter notebook using the ``!`` operator. Then, from within a notebook cell, load the qBraid magic IPython extension using:
 
 ```python
 In [1]: %load_ext qbraid_magic
```

### Comparing `qbraid_cli-0.8.1/tests/configure/test_configure_prompt_for_config.py` & `qbraid_cli-0.8.1a0/tests/test_configure/test_prompt_for_config.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/configure/test_configure_set.py` & `qbraid_cli-0.8.1a0/tests/test_configure/test_configure_set.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/configure/test_configure_validate_input.py` & `qbraid_cli-0.8.1a0/tests/test_configure/test_validate_input.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/devices/test_devices_list.py` & `qbraid_cli-0.8.1a0/tests/test_devices/test_devices_list.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/devices/test_devices_validations.py` & `qbraid_cli-0.8.1a0/tests/test_devices/test_validations.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/envs/test_envs_activate.py` & `qbraid_cli-0.8.1a0/tests/test_envs/test_app/test_envs_activate.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/envs/test_envs_activate_find_shell_rc.py` & `qbraid_cli-0.8.1a0/tests/test_envs/test_activate/test_find_shell_rc.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/envs/test_envs_activate_print_command.py` & `qbraid_cli-0.8.1a0/tests/test_envs/test_activate/test_print_activate_command.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/envs/test_envs_activate_pyenv.py` & `qbraid_cli-0.8.1a0/tests/test_envs/test_activate/test_activate_pyenv.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/envs/test_envs_create.py` & `qbraid_cli-0.8.1a0/tests/test_envs/test_app/test_envs_create.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/envs/test_envs_create_qbraid_env_assets.py` & `qbraid_cli-0.8.1a0/tests/test_envs/test_create/test_create_qbraid_env_assets.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,29 +36,32 @@
     with (
         patch("os.makedirs"),
         patch("os.path.isfile", return_value=True),
         patch("shutil.copy"),
         patch("json.dump"),
         patch("builtins.open", mock_open()),
         patch("qbraid_cli.envs.create.update_state_json") as mock_update_state_json,
+        patch("qbraid_cli.envs.create.create_venv") as mock_create_venv,
         patch(
             "jupyter_client.kernelspec.KernelSpecManager.get_all_specs",
             return_value=kernel_spec_mock,
         ),
     ):
         create_qbraid_env_assets(slug, alias, kernel_name, slug_path)
 
         # Verify that update_state_json and create_venv are called with correct arguments
         mock_update_state_json.assert_called_once_with(slug_path, 0, 0, env_name=alias)
+        mock_create_venv.assert_called_once_with(slug_path, alias)
 
         # Verify kernel.json creation and contents
         expected_kernel_json_path = os.path.join(
             slug_path, "kernels", f"python3_{slug}", "kernel.json"
         )
         open.assert_any_call(expected_kernel_json_path, "w", encoding="utf-8")
+
         # Prepare the expected data for kernel.json,
         # modifying argv[0] to match the expected python_exec_path
         expected_kernel_data = kernel_spec_mock["python3"]["spec"]
         if os.name == "nt":
             expected_kernel_data["argv"][0] = os.path.join(
                 slug_path, "pyenv", "Scripts", "python.exe"
             )
```

### Comparing `qbraid_cli-0.8.1/tests/envs/test_envs_list.py` & `qbraid_cli-0.8.1a0/tests/test_envs/test_app/test_envs_list.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/envs/test_envs_remove.py` & `qbraid_cli-0.8.1a0/tests/test_envs/test_app/test_envs_remove.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,20 +15,17 @@
 
 runner = typer.testing.CliRunner()
 
 
 @patch("shutil.rmtree", MagicMock())
 def test_envs_remove():
     """Test removing an environment."""
-    test_env_path = Path("/path/to/env")
     with (
+        patch("qbraid_cli.envs.app.request_delete_env"),
         patch(
             "qbraid_cli.envs.app.installed_envs_data",
-            return_value=({"test-slug": test_env_path}, {"Test Env": "test-slug"}),
+            return_value=({"test-slug": Path("/path/to/env")}, {"Test Env": "test-slug"}),
         ),
     ):
         name = "Test Env"
         result = runner.invoke(envs_app, ["remove", "--name", name], input="y\n")
-    assert (
-        f"Warning: You are about to delete the environment 'Test Env' located at '{test_env_path}'"
-        in result.stdout
-    )
+    assert "Environment 'Test Env' successfully removed." in result.stdout
```

### Comparing `qbraid_cli-0.8.1/tests/jobs/test_jobs_disable.py` & `qbraid_cli-0.8.1a0/tests/test_jobs/test_app/test_jobs_disable.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/jobs/test_jobs_enable.py` & `qbraid_cli-0.8.1a0/tests/test_jobs/test_app/test_jobs_enable.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/jobs/test_jobs_list.py` & `qbraid_cli-0.8.1a0/tests/test_jobs/test_app/test_jobs_list.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/jobs/test_jobs_state.py` & `qbraid_cli-0.8.1a0/tests/test_jobs/test_app/test_jobs_state.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/jobs/test_jobs_toggle_braket_confirm.py` & `qbraid_cli-0.8.1a0/tests/test_jobs/test_toggle_braket/test_confirm_updates.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/jobs/test_jobs_toggle_braket_disable.py` & `qbraid_cli-0.8.1a0/tests/test_jobs/test_toggle_braket/test_disable_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/jobs/test_jobs_toggle_braket_enable.py` & `qbraid_cli-0.8.1a0/tests/test_jobs/test_toggle_braket/test_enable_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/jobs/test_jobs_toggle_braket_get_data.py` & `qbraid_cli-0.8.1a0/tests/test_jobs/test_toggle_braket/test_get_package_data.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/jobs/test_jobs_validate_get_state.py` & `qbraid_cli-0.8.1a0/tests/test_jobs/test_validation/test_get_state.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 """
 
 from unittest.mock import patch
 
 import pytest
 
-from qbraid_cli.jobs.validation import get_state, run_progress_get_state
+from qbraid_cli.jobs.validation import get_state
 
 
 @patch("qbraid_core.services.quantum.QuantumClient.qbraid_jobs_state")
 def test_get_state_specific_library(mock_qbraid_jobs_state):
     """Test the get_state function for a specific library."""
     library = "braket"
     python_exe = "/usr/bin/python"
@@ -56,39 +56,7 @@
 
     result = get_state(library)
     mock_qbraid_jobs_state.assert_called_once_with(device_lib=library)
     assert result == (
         "/usr/bin/python",
         {library: expected},
     ), f"Expected state for {library} to be correctly returned"
-
-
-@patch("qbraid_cli.jobs.validation.get_state")
-@patch("qbraid_cli.jobs.validation.run_progress_task")
-def test_run_progress_get_state_with_library(mock_run_progress_task, mock_get_state):
-    """Test run_progress_get_state with braket library."""
-    library = "braket"
-    # Configure the mock for get_state if necessary, e.g., mock_get_state.return_value = {}
-
-    run_progress_get_state(library)
-
-    # Verifying run_progress_task is called correctly
-    mock_run_progress_task.assert_called_once()
-    _, kwargs = mock_run_progress_task.call_args
-    assert kwargs["description"] == "Collecting package metadata..."
-    assert kwargs["error_message"] == f"Failed to collect {library} package metadata."
-    # Verifying get_state is intended to be
-    # called with the correct arguments
-    mock_get_state.assert_not_called()
-
-
-@patch("qbraid_cli.jobs.validation.get_state")
-@patch("qbraid_cli.jobs.validation.run_progress_task")
-def test_run_progress_get_state_no_library(mock_run_progress_task, mock_get_state):
-    """Test run_progress_get_state without a library."""
-    run_progress_get_state()
-
-    mock_run_progress_task.assert_called_once()
-    _, kwargs = mock_run_progress_task.call_args
-    assert kwargs["description"] == "Collecting package metadata..."
-    assert kwargs["error_message"] == "Failed to collect None package metadata."
-    mock_get_state.assert_not_called()  # As above
```

### Comparing `qbraid_cli-0.8.1/tests/jobs/test_jobs_validate_handle_state.py` & `qbraid_cli-0.8.1a0/tests/test_jobs/test_validation/test_handle_jobs_state.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/jobs/test_jobs_validate_library.py` & `qbraid_cli-0.8.1a0/tests/test_jobs/test_validation/test_validate_library.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tests/kernels/test_kernels_list.py` & `qbraid_cli-0.8.1a0/tests/test_kernels/test_kernels_list.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tools/create_dev_build.sh` & `qbraid_cli-0.8.1a0/tools/create_dev_build.sh`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tools/install_wheel_extras.sh` & `qbraid_cli-0.8.1a0/tools/install_wheel_extras.sh`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.1/tools/split_rst.py` & `qbraid_cli-0.8.1a0/tools/split_rst.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,14 @@
 
     # Remove backticks from section titles if the next line is a section line
     content = re.sub(r"^``(.*?)``\n([=+\-^]+)$", r"\1\n\2", content, flags=re.MULTILINE)
 
     content = content.replace("\\ :", ":")
     content = content.replace("\n\n\n", "\n\n")
 
-    # Add a backslash directly before '*args' preceded by any amount of whitespace
-    content = re.sub(r"(^\s*)(\*args)", r"\1\\\2", content, flags=re.MULTILINE)
-
     with open(file_path, "w", encoding="utf-8") as file:
         file.write(content)
 
 
 def split_rst_file_simple(file_path: str) -> None:
     """
     Splits a reStructuredText (rst) file into multiple files based on sections underlined
```

