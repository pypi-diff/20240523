# Comparing `tmp/newrelic-9.9.0.tar.gz` & `tmp/newrelic-9.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newrelic-9.9.0.tar", last modified: Thu Apr 18 22:50:51 2024, max compression
+gzip compressed data, was "newrelic-9.9.1.tar", last modified: Mon May 13 21:39:38 2024, max compression
```

## Comparing `newrelic-9.9.0.tar` & `newrelic-9.9.1.tar`

### file list

```diff
@@ -1,1368 +1,1369 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.735916 newrelic-9.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.535914 newrelic-9.9.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-18 22:50:46.000000 newrelic-9.9.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-18 22:50:46.000000 newrelic-9.9.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.535914 newrelic-9.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.535914 newrelic-9.9.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/ISSUE_TEMPLATE/troubleshooting.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.535914 newrelic-9.9.0/.github/containers/
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/containers/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/containers/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     1528 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/containers/install-python.sh
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/containers/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/mergify.yml
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.535914 newrelic-9.9.0/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1268 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/scripts/retry.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.539914 newrelic-9.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/workflows/build-ci-image.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/workflows/deploy-python.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1186 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/workflows/get-envs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/workflows/mega-linter.yml
--rw-r--r--   0 runner    (1001) docker     (127)    31311 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-18 22:50:46.000000 newrelic-9.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-18 22:50:46.000000 newrelic-9.9.0/.mega-linter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-04-18 22:50:46.000000 newrelic-9.9.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-18 22:50:46.000000 newrelic-9.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-18 22:50:46.000000 newrelic-9.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-04-18 22:50:51.735916 newrelic-9.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7724 2024-04-18 22:50:46.000000 newrelic-9.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-18 22:50:46.000000 newrelic-9.9.0/ROADMAP.md
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-18 22:50:46.000000 newrelic-9.9.0/THIRD_PARTY_NOTICES.md
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-18 22:50:46.000000 newrelic-9.9.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.539914 newrelic-9.9.0/newrelic/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.543914 newrelic-9.9.0/newrelic/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/debug_console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/generate_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/license_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/local_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/network_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/record_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/run_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/run_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/server_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/validate_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22032 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.547914 newrelic-9.9.0/newrelic/api/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/application.py
--rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/asgi_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/background_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/cat_header_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/database_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/datastore_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/error_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/external_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/function_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/function_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/generator_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/graphql_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/html_insertion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/in_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/memcache_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/message_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/message_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/ml_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/object_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/out_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/post_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/pre_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/profile_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/solr_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/supportability.py
--rw-r--r--   0 runner    (1001) docker     (127)    26851 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/time_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    79389 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/transaction_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/web_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    25224 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/wsgi_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.547914 newrelic-9.9.0/newrelic/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/bootstrap/sitecustomize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.551914 newrelic-9.9.0/newrelic/common/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/_monotonic.c
--rw-r--r--   0 runner    (1001) docker     (127)    21725 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/agent_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/async_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/async_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    64813 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/certs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/coroutine.py
--rw-r--r--   0 runner    (1001) docker     (127)    20660 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/encoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/log_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/metric_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/object_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     9993 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/object_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/package_version_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/stopwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/streaming_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13872 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/system_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/utilization.py
--rw-r--r--   0 runner    (1001) docker     (127)   161325 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.555914 newrelic-9.9.0/newrelic/core/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/_thread_utilization.c
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/adaptive_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    32825 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    22340 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/agent_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/agent_streaming.py
--rw-r--r--   0 runner    (1001) docker     (127)    74275 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    46085 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/custom_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     9575 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/data_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/database_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    29349 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/datastore_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/error_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/error_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/external_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/function_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/graphql_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/graphql_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/infinite_tracing_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/infinite_tracing_v3_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/infinite_tracing_v4_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/internal_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/log_event_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/loop_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/memcache_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/message_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/node_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10111 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/otlp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16490 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/profile_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/root_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/rules_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/solr_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/stack_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    75777 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/stats_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/string_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/thread_utilization.py
--rw-r--r--   0 runner    (1001) docker     (127)    15461 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/trace_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/trace_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    23420 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/transaction_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.555914 newrelic-9.9.0/newrelic/extras/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.555914 newrelic-9.9.0/newrelic/extras/framework_django/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/extras/framework_django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.559914 newrelic-9.9.0/newrelic/extras/framework_django/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/extras/framework_django/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/extras/framework_django/templatetags/newrelic_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.571914 newrelic-9.9.0/newrelic/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_asgiref.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_cheroot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_cherrypy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_daphne.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_flup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_gevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_gunicorn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_hypercorn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_meinheld.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_paste.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_uvicorn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_waitress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_wsgiref.py
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/application_celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/application_gearman.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/component_cornice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/component_djangorestframework.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/component_flask_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/component_graphqlserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/component_piston.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/component_sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/component_tastypie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/coroutines_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/coroutines_gevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_asyncpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_cx_oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_dbapi2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_ibm_db_dbi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_mysqldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_oursql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    11103 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_psycopg2cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_psycopg2ct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_pymssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_pymysql.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_pyodbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_aioredis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_aredis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_bmemcached.py
--rw-r--r--   0 runner    (1001) docker     (127)    21862 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)    18601 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_firestore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_memcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_pyelasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_pylibmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_pymemcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_pymongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_pysolr.py
--rw-r--r--   0 runner    (1001) docker     (127)    17315 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_solrpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_umemcache.py
--rw-r--r--   0 runner    (1001) docker     (127)    33824 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_botocore.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_dropbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_facepy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_feedparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_httplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_httplib2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_pywapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_thrift.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_urllib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_urllib2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_xmlrpclib.py
--rw-r--r--   0 runner    (1001) docker     (127)    12197 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_ariadne.py
--rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_bottle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_cherrypy.py
--rw-r--r--   0 runner    (1001) docker     (127)    42156 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_django_py3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    15352 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_graphene.py
--rw-r--r--   0 runner    (1001) docker     (127)    18198 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_graphql_py3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_pylons.py
--rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_sanic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_starlette.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_strawberry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13267 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_tornado.py
--rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_web2py.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_webpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/logger_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/logger_loguru.py
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/logger_structlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/memcache_memcache.py
--rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/messagebroker_confluentkafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/messagebroker_kafkapython.py
--rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/messagebroker_pika.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/middleware_flask_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/middleware_weberror.py
--rw-r--r--   0 runner    (1001) docker     (127)    35454 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/mlmodel_langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    41623 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/mlmodel_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    25129 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/mlmodel_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/template_genshi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/template_jinja2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/template_mako.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.575914 newrelic-9.9.0/newrelic/network/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/network/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/network/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/newrelic.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.575914 newrelic-9.9.0/newrelic/packages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/asgiref_compatibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.575914 newrelic-9.9.0/newrelic/packages/isort/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.575914 newrelic-9.9.0/newrelic/packages/isort/stdlibs/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/all.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py27.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py311.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py36.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py37.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py39.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.575914 newrelic-9.9.0/newrelic/packages/opentelemetry_proto/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/opentelemetry_proto/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/opentelemetry_proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/opentelemetry_proto/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/opentelemetry_proto/logs_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16736 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/opentelemetry_proto/metrics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/opentelemetry_proto/resource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34549 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/six.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.579914 newrelic-9.9.0/newrelic/packages/urllib3/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    40285 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/connectionpool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.579914 newrelic-9.9.0/newrelic/packages/urllib3/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.579914 newrelic-9.9.0/newrelic/packages/urllib3/contrib/_securetransport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17632 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/appengine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 runner    (1001) docker     (127)    17055 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 runner    (1001) docker     (127)    34431 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/securetransport.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/socks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8579 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/filepost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.579914 newrelic-9.9.0/newrelic/packages/urllib3/packages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.579914 newrelic-9.9.0/newrelic/packages/urllib3/packages/backports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/packages/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/packages/backports/makefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/packages/backports/weakref_finalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    34665 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/packages/six.py
--rw-r--r--   0 runner    (1001) docker     (127)    19990 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/poolmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    30761 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.583914 newrelic-9.9.0/newrelic/packages/urllib3/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    22013 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    17165 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/ssl_.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/ssltransport.py
--rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.583914 newrelic-9.9.0/newrelic/packages/wrapt/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/__wrapt__.py
--rw-r--r--   0 runner    (1001) docker     (127)    96990 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/_wrappers.c
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/weakrefs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27137 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/newrelic/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/samplers/cpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/samplers/data_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/samplers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/samplers/gc_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/samplers/memory_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.735916 newrelic-9.9.0/newrelic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    61751 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-18 22:50:46.000000 newrelic-9.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/scripts/newrelic-admin
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-18 22:50:51.735916 newrelic-9.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-04-18 22:50:46.000000 newrelic-9.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.531914 newrelic-9.9.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/tests/adapter_asgiref/
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_asgiref/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_asgiref/test_context_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/tests/adapter_cheroot/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_cheroot/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_cheroot/test_wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/tests/adapter_daphne/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_daphne/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_daphne/test_daphne.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/tests/adapter_gevent/
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gevent/_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gevent/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gevent/test_patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gevent/test_pywsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/tests/adapter_gunicorn/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/asgi_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/async_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/test_aiohttp_app_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/test_asgi_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/test_gaiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/tests/adapter_hypercorn/
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_hypercorn/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_hypercorn/test_hypercorn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/tests/adapter_uvicorn/
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_uvicorn/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_uvicorn/test_uvicorn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.591915 newrelic-9.9.0/tests/adapter_waitress/
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_waitress/_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_waitress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_waitress/test_wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.599915 newrelic-9.9.0/tests/agent_features/
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/_test_async_coroutine_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/_test_async_coroutine_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/_test_async_generator_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/_test_code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_apdex_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    32398 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_asgi_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_asgi_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_asgi_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_asgi_w3c_trace_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_async_context_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_async_generator_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_async_timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_async_wrapper_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    35683 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_attributes_in_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_background_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    34491 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_browser_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_collector_payloads.py
--rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_coroutine_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_coroutine_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_custom_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_custom_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_datastore_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_dead_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_dimensional_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_error_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_error_group_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_event_loop_wait_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    13189 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_exception_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_function_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    29688 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_high_security_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_ignore_expected_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_llm_token_count_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_log_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_logs_in_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_metric_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_ml_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_notice_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_priority_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_profile_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_record_llm_feedback_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_serverless_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    24641 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_span_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_stack_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_supportability_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_synthetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_time_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_transaction_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_transaction_trace_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_w3c_trace_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_web_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_wsgi_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.599915 newrelic-9.9.0/tests/agent_streaming/
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_streaming/_test_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_streaming/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17363 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_streaming/test_infinite_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_streaming/test_span_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_streaming/test_stream_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_streaming/test_streaming_rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.603915 newrelic-9.9.0/tests/agent_unittests/
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/_test_import_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_agent_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)    20250 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_agent_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_check_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_connect_response_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_distributed_tracing_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_encoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_full_uri_payloads.py
--rw-r--r--   0 runner    (1001) docker     (127)    32348 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_harvest_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    21008 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_import_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_infinite_trace_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_package_version_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_region_aware_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_sampler_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_serverless_mode_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_trace_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_utilization_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.607915 newrelic-9.9.0/tests/application_celery/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_celery/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_celery/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_celery/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_celery/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_celery/test_max_tasks_per_child.py
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_celery/test_task_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.607915 newrelic-9.9.0/tests/application_gearman/
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_gearman/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_gearman/test_gearman.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.607915 newrelic-9.9.0/tests/component_djangorestframework/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_djangorestframework/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_djangorestframework/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_djangorestframework/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_djangorestframework/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_djangorestframework/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_djangorestframework/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.607915 newrelic-9.9.0/tests/component_flask_rest/
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_flask_rest/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_flask_rest/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_flask_rest/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.607915 newrelic-9.9.0/tests/component_graphqlserver/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_graphqlserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_graphqlserver/_target_schema_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_graphqlserver/_test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_graphqlserver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    18303 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_graphqlserver/test_graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.611915 newrelic-9.9.0/tests/component_tastypie/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_tastypie/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_tastypie/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_tastypie/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_tastypie/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_tastypie/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_tastypie/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_tastypie/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.611915 newrelic-9.9.0/tests/coroutines_asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/coroutines_asyncio/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/coroutines_asyncio/test_context_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.615915 newrelic-9.9.0/tests/cross_agent/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.615915 newrelic-9.9.0/tests/cross_agent/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/attribute_configuration.json
--rw-r--r--   0 runner    (1001) docker     (127)    15836 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/cat_map.json
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/collector_hostname.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.615915 newrelic-9.9.0/tests/cross_agent/fixtures/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/datastores/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/datastores/datastore_instances.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.615915 newrelic-9.9.0/tests/cross_agent/fixtures/distributed_tracing/
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/distributed_tracing/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    48250 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json
--rw-r--r--   0 runner    (1001) docker     (127)    58950 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/distributed_tracing/trace_context.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.619915 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/cases.json
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-0.9.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/empty.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/heroku.txt
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/invalid-length.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-lxc-container.txt
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-no-container.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.10-no-container.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.619915 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/cases.json
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-20.10.16.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-24.0.2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-too-long.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/empty.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/invalid-characters.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/invalid-length.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/labels.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.627915 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/api_gateway_auth.json
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/batch_get.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/batch_submit.json
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudformation_create.json
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_response.json
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudwatch_logs.json
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/codecommit.json
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cognito_sync.json
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis.json
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_analytics.json
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_apache.json
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_invoke.json
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/lex_appointment.json
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/lex_book_car.json
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/s3_put.json
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/scheduled_event.json
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/ses.json
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/smarthome_discovery.json
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/smarthome_turn_off.json
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/sns.json
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/sqs.json
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.643915 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.query.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.643915 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_1logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_2core_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17027 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)    38341 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/malformed_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.643915 newrelic-9.9.0/tests/cross_agent/fixtures/proc_meminfo/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_meminfo/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_meminfo/malformed_file.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rules.json
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_cookie.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.651915 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/empty_head
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html
--rwxr-xr-x   0 runner    (1001) docker     (127)      852 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html
--rwxr-xr-x   0 runner    (1001) docker     (127)      958 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.659915 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.659915 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.659915 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql
--rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_parsing.json
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/transaction_segment_terms.json
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/url_clean.json
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/url_domain_extraction.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.659915 newrelic-9.9.0/tests/cross_agent/fixtures/utilization/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization/boot_id.json
--rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization/utilization_json.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.663915 newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json
--rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json
--rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_agent_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_aws_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_azure_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_boot_id_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_cat_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_collector_hostname.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_datastore_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_docker_container_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_docker_container_id_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_gcp_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_labels_and_rollups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_lambda_event_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_pcf_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_sql_obfuscation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_system_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_transaction_segment_terms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_utilization_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_w3c_trace_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.663915 newrelic-9.9.0/tests/datastore_aioredis/
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_custom_conn_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_execute_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_get_and_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_uninstrumented_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.663915 newrelic-9.9.0/tests/datastore_aredis/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_custom_conn_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_execute_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_get_and_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_uninstrumented_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.667915 newrelic-9.9.0/tests/datastore_asyncpg/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_asyncpg/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_asyncpg/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_asyncpg/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.667915 newrelic-9.9.0/tests/datastore_bmemcached/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_bmemcached/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_bmemcached/test_memcache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.667915 newrelic-9.9.0/tests/datastore_elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_database_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_instrumented_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_mget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_transport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.671915 newrelic-9.9.0/tests/datastore_firestore/
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_async_batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_async_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_async_documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_async_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_async_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.671915 newrelic-9.9.0/tests/datastore_memcache/
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_memcache/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_memcache/test_all_methods_wrapped.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_memcache/test_memcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_memcache/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_memcache/test_span_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.671915 newrelic-9.9.0/tests/datastore_mysql/
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_mysql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_mysql/test_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.671915 newrelic-9.9.0/tests/datastore_postgresql/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_postgresql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_postgresql/test_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_psycopg2/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_as_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_database_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_explain_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_forward_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_obfuscation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_rollback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_slow_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_psycopg2cffi/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2cffi/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2cffi/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2cffi/test_explain_plans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_pylibmc/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pylibmc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pylibmc/test_memcache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_pymemcache/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymemcache/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymemcache/test_memcache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_pymongo/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymongo/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    15220 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymongo/test_pymongo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_pymssql/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymssql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymssql/test_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_pymysql/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymysql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymysql/test_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_pyodbc/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pyodbc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pyodbc/test_pyodbc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_pysolr/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pysolr/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pysolr/test_solr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.679915 newrelic-9.9.0/tests/datastore_redis/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_custom_conn_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_execute_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_get_and_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_rb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_uninstrumented_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.679915 newrelic-9.9.0/tests/datastore_rediscluster/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_rediscluster/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_rediscluster/test_uninstrumented_rediscluster_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.679915 newrelic-9.9.0/tests/datastore_solrpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_solrpy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_solrpy/test_solr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.679915 newrelic-9.9.0/tests/datastore_sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_sqlite/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_sqlite/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_sqlite/test_obfuscation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.683915 newrelic-9.9.0/tests/external_botocore/
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/_mock_bedrock_encoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   331596 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/_mock_external_bedrock_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    55152 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/_test_bedrock_chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/_test_bedrock_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    36309 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_bedrock_chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_bedrock_chat_completion_via_langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    17722 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_bedrock_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_boto3_iam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_boto3_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_boto3_sns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_botocore_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_botocore_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_botocore_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_botocore_sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.683915 newrelic-9.9.0/tests/external_feedparser/
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_feedparser/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13246 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_feedparser/packages.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_feedparser/test_feedparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.683915 newrelic-9.9.0/tests/external_http/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_http/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_http/test_http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.683915 newrelic-9.9.0/tests/external_httplib/
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httplib/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httplib/test_httplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httplib/test_urllib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httplib/test_urllib2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.683915 newrelic-9.9.0/tests/external_httplib2/
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httplib2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httplib2/test_httplib2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.683915 newrelic-9.9.0/tests/external_httpx/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httpx/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    15878 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httpx/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.687915 newrelic-9.9.0/tests/external_requests/
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_requests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_requests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_requests/test_span_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.687915 newrelic-9.9.0/tests/external_urllib3/
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_urllib3/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9361 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_urllib3/test_urllib3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.687915 newrelic-9.9.0/tests/framework_aiohttp/
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_client_async_await.py
--rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_client_cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_externals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_server_cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_ws.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.687915 newrelic-9.9.0/tests/framework_ariadne/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_ariadne/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_ariadne/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_ariadne/_target_schema_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_ariadne/_target_schema_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_ariadne/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_ariadne/schema.graphql
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_ariadne/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.687915 newrelic-9.9.0/tests/framework_bottle/
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_bottle/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_bottle/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_bottle/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.691915 newrelic-9.9.0/tests/framework_cherrypy/
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_cherrypy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_cherrypy/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_cherrypy/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_cherrypy/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_cherrypy/test_routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.691915 newrelic-9.9.0/tests/framework_django/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.691915 newrelic-9.9.0/tests/framework_django/dummy_app/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/dummy_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.691915 newrelic-9.9.0/tests/framework_django/dummy_app/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/dummy_app/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/dummy_app/templatetags/custom_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.691915 newrelic-9.9.0/tests/framework_django/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/templates/main.html
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/templates/render_exception.html
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/templates/results.html
--rw-r--r--   0 runner    (1001) docker     (127)    22716 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/test_asgi_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.691915 newrelic-9.9.0/tests/framework_falcon/
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_falcon/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_falcon/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_falcon/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.695915 newrelic-9.9.0/tests/framework_fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_fastapi/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_fastapi/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_fastapi/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.695915 newrelic-9.9.0/tests/framework_flask/
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_application_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_blueprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_user_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_views_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/test_blueprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/test_not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/test_user_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.695915 newrelic-9.9.0/tests/framework_graphene/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphene/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphene/_target_schema_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphene/_target_schema_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphene/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphene/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.699915 newrelic-9.9.0/tests/framework_graphql/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphql/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphql/_target_schema_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphql/_target_schema_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    21392 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphql/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphql/test_application_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.699915 newrelic-9.9.0/tests/framework_grpc/
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/_test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.699915 newrelic-9.9.0/tests/framework_grpc/sample_application/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/sample_application/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/sample_application/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/sample_application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/sample_application/sample_application.proto
--rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.699915 newrelic-9.9.0/tests/framework_pyramid/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_pyramid/_test_append_slash_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_pyramid/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_pyramid/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_pyramid/test_append_slash_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_pyramid/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_pyramid/test_cornice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.703915 newrelic-9.9.0/tests/framework_sanic/
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_sanic/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_sanic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13507 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_sanic/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_sanic/test_cross_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.703915 newrelic-9.9.0/tests/framework_starlette/
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_starlette/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_starlette/_test_bg_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_starlette/_test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_starlette/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_starlette/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_starlette/test_bg_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.703915 newrelic-9.9.0/tests/framework_strawberry/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_strawberry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_strawberry/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_strawberry/_target_schema_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_strawberry/_target_schema_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_strawberry/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_strawberry/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.703915 newrelic-9.9.0/tests/framework_tornado/
--rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_tornado/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_tornado/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_tornado/test_custom_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_tornado/test_externals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_tornado/test_inbound_cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_tornado/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.707915 newrelic-9.9.0/tests/logger_logging/
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_logging/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_logging/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_logging/test_local_decorating.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_logging/test_log_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_logging/test_logging_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_logging/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_logging/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.707915 newrelic-9.9.0/tests/logger_loguru/
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_loguru/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_loguru/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_loguru/test_local_decorating.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_loguru/test_log_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_loguru/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_loguru/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.707915 newrelic-9.9.0/tests/logger_structlog/
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_structlog/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_structlog/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_structlog/test_local_decorating.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_structlog/test_log_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_structlog/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.707915 newrelic-9.9.0/tests/messagebroker_confluentkafka/
--rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_confluentkafka/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_confluentkafka/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_confluentkafka/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_confluentkafka/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.711915 newrelic-9.9.0/tests/messagebroker_kafkapython/
--rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_kafkapython/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_kafkapython/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_kafkapython/test_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_kafkapython/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_kafkapython/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.711915 newrelic-9.9.0/tests/messagebroker_pika/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/minversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_memory_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)    17114 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_pika_async_connection_consume.py
--rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_pika_blocking_connection_consume.py
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13879 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_pika_produce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_pika_supportability.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.711915 newrelic-9.9.0/tests/mlmodel_langchain/
--rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_langchain/_mock_external_openai_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_langchain/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_langchain/hello.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_langchain/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    53177 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_langchain/test_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)    16916 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_langchain/test_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)    17598 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_langchain/test_vectorstore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.715915 newrelic-9.9.0/tests/mlmodel_openai/
--rw-r--r--   0 runner    (1001) docker     (127)    55141 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/_mock_external_openai_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    13416 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    16526 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    23654 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    18574 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_error_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    17200 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    28903 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream_error_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    17722 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)    19152 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    15641 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_error_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_stream_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.719915 newrelic-9.9.0/tests/mlmodel_sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_calibration_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_cluster_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_compose_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_covariance_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_cross_decomposition_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_discriminant_analysis_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_dummy_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_ensemble_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_feature_selection_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_gaussian_process_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12412 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_inference_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_kernel_ridge_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14219 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_linear_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_metric_scorers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_mixture_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_ml_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_model_selection_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_multiclass_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_multioutput_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_naive_bayes_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_neighbors_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_neural_network_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_pipeline_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    26289 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_prediction_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_semi_supervised_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_svm_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_tree_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.719915 newrelic-9.9.0/tests/template_genshi/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/template_genshi/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/template_genshi/test_genshi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.719915 newrelic-9.9.0/tests/template_jinja2/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/template_jinja2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/template_jinja2/test_jinja2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.719915 newrelic-9.9.0/tests/template_mako/
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/template_mako/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/template_mako/test_mako.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.723915 newrelic-9.9.0/tests/testing_support/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/asgi_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9612 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/db_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/external_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.723915 newrelic-9.9.0/tests/testing_support/fixture/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/fixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/fixture/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    50802 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/ml_testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/mock_external_grpc_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/mock_external_http_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/mock_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/sample_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/sample_asgi_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.735916 newrelic-9.9.0/tests/testing_support/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_apdex_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_application_error_event_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_application_error_trace_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_application_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_browser_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_cross_process_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_custom_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_custom_event_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_custom_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_custom_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_database_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_database_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_database_trace_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_datastore_trace_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_dimensional_metric_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_dimensional_metrics_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_distributed_trace_accepted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_distributed_tracing_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_error_event_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_error_event_attributes_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_error_event_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_error_trace_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_error_trace_attributes_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_error_trace_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_external_node_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_function_called.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_internal_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_log_event_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_log_event_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_log_event_count_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_log_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_log_events_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_messagebroker_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_metric_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_ml_event_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_ml_event_count_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_ml_event_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_ml_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_ml_events_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_non_transaction_error_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_outbound_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_serverless_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_serverless_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_serverless_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_slow_sql_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_span_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_sql_obfuscation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_synthetics_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_synthetics_transaction_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_time_metrics_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_error_event_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_error_trace_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_event_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_event_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_slow_sql_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_trace_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_tt_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_tt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_tt_segment_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    26571 2024-04-18 22:50:46.000000 newrelic-9.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.643365 newrelic-9.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.451365 newrelic-9.9.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-13 21:39:33.000000 newrelic-9.9.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-13 21:39:33.000000 newrelic-9.9.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.451365 newrelic-9.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.451365 newrelic-9.9.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/ISSUE_TEMPLATE/troubleshooting.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.451365 newrelic-9.9.1/.github/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/containers/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/containers/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1528 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/containers/install-python.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/containers/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.451365 newrelic-9.9.1/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1268 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/scripts/retry.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.451365 newrelic-9.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/workflows/build-ci-image.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/workflows/deploy-python.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1186 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/workflows/get-envs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/workflows/mega-linter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    31311 2024-05-13 21:39:33.000000 newrelic-9.9.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-13 21:39:33.000000 newrelic-9.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-13 21:39:33.000000 newrelic-9.9.1/.mega-linter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-05-13 21:39:33.000000 newrelic-9.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-13 21:39:33.000000 newrelic-9.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-13 21:39:33.000000 newrelic-9.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-05-13 21:39:38.643365 newrelic-9.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7724 2024-05-13 21:39:33.000000 newrelic-9.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-13 21:39:33.000000 newrelic-9.9.1/ROADMAP.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-13 21:39:33.000000 newrelic-9.9.1/THIRD_PARTY_NOTICES.md
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-13 21:39:33.000000 newrelic-9.9.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.455365 newrelic-9.9.1/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.455365 newrelic-9.9.1/newrelic/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/admin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/admin/debug_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/admin/generate_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/admin/license_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/admin/local_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/admin/network_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/admin/record_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/admin/run_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/admin/run_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/admin/server_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/admin/validate_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22032 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.463365 newrelic-9.9.1/newrelic/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/asgi_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/background_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/cat_header_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/database_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/datastore_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/error_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/external_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/function_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/function_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/generator_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/graphql_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/html_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/in_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/memcache_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/message_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/message_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/ml_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/object_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/out_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/post_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/pre_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/profile_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/solr_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/supportability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26851 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/time_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79389 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/transaction_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/web_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25224 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/api/wsgi_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.463365 newrelic-9.9.1/newrelic/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/bootstrap/sitecustomize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.463365 newrelic-9.9.1/newrelic/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/_monotonic.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21725 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/agent_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/async_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/async_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64813 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/certs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/coroutine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20660 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/encoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/log_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/metric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/object_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9993 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/object_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/package_version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/stopwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/streaming_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13872 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/system_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/common/utilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)   162260 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.471365 newrelic-9.9.1/newrelic/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/_thread_utilization.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/adaptive_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32825 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22340 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/agent_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/agent_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74275 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46085 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/custom_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9575 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/database_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29349 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/datastore_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/error_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/error_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/external_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/function_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/graphql_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/graphql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/infinite_tracing_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/infinite_tracing_v3_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/infinite_tracing_v4_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/internal_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/log_event_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/loop_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/memcache_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/message_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/node_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10111 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/otlp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16490 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/profile_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/root_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/rules_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/solr_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/stack_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75777 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/stats_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/string_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/thread_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15461 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/trace_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23420 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/core/transaction_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.471365 newrelic-9.9.1/newrelic/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.471365 newrelic-9.9.1/newrelic/extras/framework_django/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/extras/framework_django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.471365 newrelic-9.9.1/newrelic/extras/framework_django/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/extras/framework_django/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/extras/framework_django/templatetags/newrelic_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.487365 newrelic-9.9.1/newrelic/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/adapter_asgiref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/adapter_cheroot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/adapter_cherrypy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/adapter_daphne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/adapter_flup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/adapter_gevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/adapter_gunicorn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/adapter_hypercorn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/adapter_meinheld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/adapter_paste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/adapter_uvicorn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/adapter_waitress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/adapter_wsgiref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/application_celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/application_gearman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/component_cornice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/component_djangorestframework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/component_flask_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/component_graphqlserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/component_piston.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/component_sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/component_tastypie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/coroutines_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/coroutines_gevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/database_asyncpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/database_cx_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/database_dbapi2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/database_ibm_db_dbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/database_mysqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/database_oursql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11103 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/database_psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/database_psycopg2cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/database_psycopg2ct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/database_pymssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/database_pymysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/database_pyodbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/database_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/datastore_aioredis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/datastore_aredis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/datastore_bmemcached.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21862 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/datastore_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18601 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/datastore_firestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/datastore_memcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/datastore_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/datastore_pyelasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/datastore_pylibmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/datastore_pymemcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/datastore_pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/datastore_pysolr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17315 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/datastore_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/datastore_solrpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/datastore_umemcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33824 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/external_botocore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/external_dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/external_facepy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/external_feedparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/external_httplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/external_httplib2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/external_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/external_pywapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/external_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/external_thrift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/external_urllib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/external_urllib2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/external_urllib3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/external_xmlrpclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12197 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_ariadne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_bottle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_cherrypy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42156 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_django_py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15352 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_graphene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18198 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_graphql_py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_pylons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_sanic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_starlette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_strawberry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13267 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_tornado.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_web2py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/framework_webpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/logger_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/logger_loguru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/logger_structlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/memcache_memcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/messagebroker_confluentkafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/messagebroker_kafkapython.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/messagebroker_pika.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/middleware_flask_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/middleware_weberror.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35695 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/mlmodel_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41623 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/mlmodel_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25129 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/mlmodel_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/template_genshi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/template_jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/hooks/template_mako.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.487365 newrelic-9.9.1/newrelic/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/network/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/network/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/newrelic.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.491365 newrelic-9.9.1/newrelic/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/asgiref_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.491365 newrelic-9.9.1/newrelic/packages/isort/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/isort/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/isort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.491365 newrelic-9.9.1/newrelic/packages/isort/stdlibs/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/isort/stdlibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/isort/stdlibs/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/isort/stdlibs/py2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/isort/stdlibs/py27.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/isort/stdlibs/py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/isort/stdlibs/py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/isort/stdlibs/py311.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/isort/stdlibs/py36.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/isort/stdlibs/py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/isort/stdlibs/py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/isort/stdlibs/py39.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.491365 newrelic-9.9.1/newrelic/packages/opentelemetry_proto/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/opentelemetry_proto/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/opentelemetry_proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/opentelemetry_proto/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/opentelemetry_proto/logs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16736 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/opentelemetry_proto/metrics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/opentelemetry_proto/resource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34549 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/six.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.495365 newrelic-9.9.1/newrelic/packages/urllib3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40285 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/connectionpool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.495365 newrelic-9.9.1/newrelic/packages/urllib3/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.495365 newrelic-9.9.1/newrelic/packages/urllib3/contrib/_securetransport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17632 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/contrib/appengine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17055 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34431 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/contrib/securetransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/contrib/socks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8579 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/filepost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.495365 newrelic-9.9.1/newrelic/packages/urllib3/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.495365 newrelic-9.9.1/newrelic/packages/urllib3/packages/backports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/packages/backports/weakref_finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34665 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/packages/six.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19990 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/poolmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30761 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.499365 newrelic-9.9.1/newrelic/packages/urllib3/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/util/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/util/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/util/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/util/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22013 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17165 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/util/ssl_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/util/ssltransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/util/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/util/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/urllib3/util/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.499365 newrelic-9.9.1/newrelic/packages/wrapt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/wrapt/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/wrapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/wrapt/__wrapt__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96990 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/wrapt/_wrappers.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/wrapt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/wrapt/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/wrapt/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/wrapt/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/wrapt/weakrefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27137 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/packages/wrapt/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.503365 newrelic-9.9.1/newrelic/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/samplers/cpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/samplers/data_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/samplers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/samplers/gc_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-13 21:39:33.000000 newrelic-9.9.1/newrelic/samplers/memory_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 21:39:38.000000 newrelic-9.9.1/newrelic/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.639365 newrelic-9.9.1/newrelic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-05-13 21:39:38.000000 newrelic-9.9.1/newrelic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    61793 2024-05-13 21:39:38.000000 newrelic-9.9.1/newrelic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:39:38.000000 newrelic-9.9.1/newrelic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 21:39:38.000000 newrelic-9.9.1/newrelic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:39:38.000000 newrelic-9.9.1/newrelic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-13 21:39:38.000000 newrelic-9.9.1/newrelic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-13 21:39:38.000000 newrelic-9.9.1/newrelic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-13 21:39:33.000000 newrelic-9.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.503365 newrelic-9.9.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-05-13 21:39:33.000000 newrelic-9.9.1/scripts/newrelic-admin
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-13 21:39:38.643365 newrelic-9.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-05-13 21:39:33.000000 newrelic-9.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.447365 newrelic-9.9.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.503365 newrelic-9.9.1/tests/adapter_asgiref/
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_asgiref/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_asgiref/test_context_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.503365 newrelic-9.9.1/tests/adapter_cheroot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_cheroot/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_cheroot/test_wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.503365 newrelic-9.9.1/tests/adapter_daphne/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_daphne/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_daphne/test_daphne.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.503365 newrelic-9.9.1/tests/adapter_gevent/
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_gevent/_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_gevent/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_gevent/test_patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_gevent/test_pywsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.503365 newrelic-9.9.1/tests/adapter_gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_gunicorn/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_gunicorn/asgi_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_gunicorn/async_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_gunicorn/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_gunicorn/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_gunicorn/test_aiohttp_app_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_gunicorn/test_asgi_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_gunicorn/test_gaiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_gunicorn/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.503365 newrelic-9.9.1/tests/adapter_hypercorn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_hypercorn/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_hypercorn/test_hypercorn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.503365 newrelic-9.9.1/tests/adapter_uvicorn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_uvicorn/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_uvicorn/test_uvicorn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.507365 newrelic-9.9.1/tests/adapter_waitress/
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_waitress/_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_waitress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/adapter_waitress/test_wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.515365 newrelic-9.9.1/tests/agent_features/
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/_test_async_coroutine_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/_test_async_coroutine_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/_test_async_generator_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/_test_code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_apdex_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32398 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_asgi_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_asgi_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_asgi_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_asgi_w3c_trace_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_async_context_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_async_generator_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_async_timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_async_wrapper_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35683 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_attributes_in_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_background_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34491 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_browser_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_collector_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_coroutine_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_coroutine_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_custom_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_custom_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_datastore_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_dead_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_dimensional_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_error_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_error_group_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_event_loop_wait_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13189 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_exception_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_function_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29688 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_high_security_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_ignore_expected_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_llm_token_count_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_log_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_logs_in_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_metric_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_ml_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_notice_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_priority_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_profile_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_record_llm_feedback_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_serverless_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24641 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_span_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_stack_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_supportability_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_synthetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_time_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_transaction_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_transaction_trace_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_w3c_trace_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_web_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_features/test_wsgi_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.515365 newrelic-9.9.1/tests/agent_streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_streaming/_test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_streaming/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17363 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_streaming/test_infinite_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_streaming/test_span_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_streaming/test_stream_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_streaming/test_streaming_rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.519365 newrelic-9.9.1/tests/agent_unittests/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/_test_import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_agent_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20250 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_agent_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_check_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_connect_response_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_distributed_tracing_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_encoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_full_uri_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32348 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_harvest_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21008 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_infinite_trace_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_package_version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_region_aware_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_sampler_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_serverless_mode_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_trace_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_utilization_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/agent_unittests/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.519365 newrelic-9.9.1/tests/application_celery/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/application_celery/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/application_celery/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/application_celery/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/application_celery/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/application_celery/test_max_tasks_per_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/application_celery/test_task_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/application_celery/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.519365 newrelic-9.9.1/tests/application_gearman/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/application_gearman/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/application_gearman/test_gearman.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.523365 newrelic-9.9.1/tests/component_djangorestframework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_djangorestframework/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_djangorestframework/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_djangorestframework/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_djangorestframework/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_djangorestframework/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_djangorestframework/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.523365 newrelic-9.9.1/tests/component_flask_rest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_flask_rest/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_flask_rest/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_flask_rest/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.523365 newrelic-9.9.1/tests/component_graphqlserver/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_graphqlserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_graphqlserver/_target_schema_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_graphqlserver/_test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_graphqlserver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18303 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_graphqlserver/test_graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.523365 newrelic-9.9.1/tests/component_tastypie/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_tastypie/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_tastypie/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_tastypie/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_tastypie/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_tastypie/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_tastypie/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/component_tastypie/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.523365 newrelic-9.9.1/tests/coroutines_asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/coroutines_asyncio/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/coroutines_asyncio/test_context_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.527365 newrelic-9.9.1/tests/cross_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.527365 newrelic-9.9.1/tests/cross_agent/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/attribute_configuration.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15836 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/cat_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/collector_hostname.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.527365 newrelic-9.9.1/tests/cross_agent/fixtures/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/datastores/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/datastores/datastore_instances.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.531365 newrelic-9.9.1/tests/cross_agent/fixtures/distributed_tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/distributed_tracing/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    48250 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json
+-rw-r--r--   0 runner    (1001) docker     (127)    58950 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/distributed_tracing/trace_context.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.531365 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/cases.json
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/docker-0.9.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/heroku.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/invalid-length.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-lxc-container.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-no-container.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.10-no-container.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.531365 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id_v2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id_v2/cases.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id_v2/docker-20.10.16.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id_v2/docker-24.0.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id_v2/docker-too-long.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id_v2/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id_v2/invalid-characters.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id_v2/invalid-length.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/labels.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.539365 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/api_gateway_auth.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/batch_get.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/batch_submit.json
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cloudformation_create.json
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cloudwatch_logs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/codecommit.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cognito_sync.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/kinesis.json
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/kinesis_analytics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_apache.json
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_invoke.json
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/lex_appointment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/lex_book_car.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/s3_put.json
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/scheduled_event.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/ses.json
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/smarthome_discovery.json
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/smarthome_turn_off.json
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/sns.json
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/sqs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.551365 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.query.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.555365 newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_1logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/1pack_2core_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17027 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38341 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/malformed_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.555365 newrelic-9.9.1/tests/cross_agent/fixtures/proc_meminfo/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_meminfo/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_meminfo/malformed_file.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rules.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_cookie.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.559365 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/empty_head
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)      852 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)      958 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.567365 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.567365 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/malformed/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.567365 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/sql_parsing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/transaction_segment_terms.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/url_clean.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/url_domain_extraction.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.567365 newrelic-9.9.1/tests/cross_agent/fixtures/utilization/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/utilization/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/utilization/boot_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/utilization/utilization_json.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.571365 newrelic-9.9.1/tests/cross_agent/fixtures/utilization_vendor_specific/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/utilization_vendor_specific/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_agent_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_aws_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_azure_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_boot_id_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_cat_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_collector_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_datastore_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_docker_container_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_docker_container_id_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_gcp_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_labels_and_rollups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_lambda_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_pcf_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_sql_obfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_system_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_transaction_segment_terms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_utilization_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/cross_agent/test_w3c_trace_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.571365 newrelic-9.9.1/tests/datastore_aioredis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aioredis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aioredis/test_custom_conn_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aioredis/test_execute_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aioredis/test_get_and_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aioredis/test_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aioredis/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aioredis/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aioredis/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aioredis/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aioredis/test_uninstrumented_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.571365 newrelic-9.9.1/tests/datastore_aredis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aredis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aredis/test_custom_conn_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aredis/test_execute_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aredis/test_get_and_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aredis/test_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aredis/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aredis/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aredis/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_aredis/test_uninstrumented_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.575365 newrelic-9.9.1/tests/datastore_asyncpg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_asyncpg/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_asyncpg/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_asyncpg/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.575365 newrelic-9.9.1/tests/datastore_bmemcached/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_bmemcached/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_bmemcached/test_memcache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.575365 newrelic-9.9.1/tests/datastore_elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_elasticsearch/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_elasticsearch/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_elasticsearch/test_database_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_elasticsearch/test_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_elasticsearch/test_instrumented_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_elasticsearch/test_mget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_elasticsearch/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_elasticsearch/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_elasticsearch/test_transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.579365 newrelic-9.9.1/tests/datastore_firestore/
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_firestore/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_firestore/test_async_batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_firestore/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_firestore/test_async_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_firestore/test_async_documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_firestore/test_async_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_firestore/test_async_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_firestore/test_batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_firestore/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_firestore/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_firestore/test_documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_firestore/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_firestore/test_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.579365 newrelic-9.9.1/tests/datastore_memcache/
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_memcache/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_memcache/test_all_methods_wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_memcache/test_memcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_memcache/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_memcache/test_span_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.579365 newrelic-9.9.1/tests/datastore_mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_mysql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_mysql/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.579365 newrelic-9.9.1/tests/datastore_postgresql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_postgresql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_postgresql/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.583365 newrelic-9.9.1/tests/datastore_psycopg2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2/test_as_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2/test_database_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2/test_explain_plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2/test_forward_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2/test_obfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2/test_rollback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2/test_slow_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.583365 newrelic-9.9.1/tests/datastore_psycopg2cffi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2cffi/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2cffi/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_psycopg2cffi/test_explain_plans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.583365 newrelic-9.9.1/tests/datastore_pylibmc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_pylibmc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_pylibmc/test_memcache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.583365 newrelic-9.9.1/tests/datastore_pymemcache/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_pymemcache/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_pymemcache/test_memcache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.583365 newrelic-9.9.1/tests/datastore_pymongo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_pymongo/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15220 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_pymongo/test_pymongo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.583365 newrelic-9.9.1/tests/datastore_pymssql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_pymssql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_pymssql/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.583365 newrelic-9.9.1/tests/datastore_pymysql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_pymysql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_pymysql/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.583365 newrelic-9.9.1/tests/datastore_pyodbc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_pyodbc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_pyodbc/test_pyodbc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.583365 newrelic-9.9.1/tests/datastore_pysolr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_pysolr/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_pysolr/test_solr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.587365 newrelic-9.9.1/tests/datastore_redis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_redis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_redis/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_redis/test_custom_conn_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_redis/test_execute_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_redis/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_redis/test_get_and_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_redis/test_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_redis/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_redis/test_rb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_redis/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_redis/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_redis/test_uninstrumented_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.587365 newrelic-9.9.1/tests/datastore_rediscluster/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_rediscluster/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_rediscluster/test_uninstrumented_rediscluster_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.587365 newrelic-9.9.1/tests/datastore_solrpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_solrpy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_solrpy/test_solr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.587365 newrelic-9.9.1/tests/datastore_sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_sqlite/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_sqlite/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/datastore_sqlite/test_obfuscation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.591365 newrelic-9.9.1/tests/external_botocore/
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_botocore/_mock_bedrock_encoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   331596 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_botocore/_mock_external_bedrock_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55152 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_botocore/_test_bedrock_chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_botocore/_test_bedrock_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_botocore/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36309 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_botocore/test_bedrock_chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_botocore/test_bedrock_chat_completion_via_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17722 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_botocore/test_bedrock_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_botocore/test_boto3_iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_botocore/test_boto3_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_botocore/test_boto3_sns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_botocore/test_botocore_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_botocore/test_botocore_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_botocore/test_botocore_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_botocore/test_botocore_sqs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.591365 newrelic-9.9.1/tests/external_feedparser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_feedparser/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13246 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_feedparser/packages.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_feedparser/test_feedparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.591365 newrelic-9.9.1/tests/external_http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_http/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_http/test_http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.591365 newrelic-9.9.1/tests/external_httplib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_httplib/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_httplib/test_httplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_httplib/test_urllib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_httplib/test_urllib2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.591365 newrelic-9.9.1/tests/external_httplib2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_httplib2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_httplib2/test_httplib2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.591365 newrelic-9.9.1/tests/external_httpx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_httpx/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15878 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_httpx/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.591365 newrelic-9.9.1/tests/external_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_requests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_requests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_requests/test_span_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.595365 newrelic-9.9.1/tests/external_urllib3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_urllib3/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/external_urllib3/test_urllib3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.595365 newrelic-9.9.1/tests/framework_aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_aiohttp/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_aiohttp/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_aiohttp/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_aiohttp/test_client_async_await.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_aiohttp/test_client_cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_aiohttp/test_externals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_aiohttp/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_aiohttp/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_aiohttp/test_server_cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_aiohttp/test_ws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.595365 newrelic-9.9.1/tests/framework_ariadne/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_ariadne/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_ariadne/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_ariadne/_target_schema_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_ariadne/_target_schema_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_ariadne/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_ariadne/schema.graphql
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_ariadne/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.595365 newrelic-9.9.1/tests/framework_bottle/
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_bottle/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_bottle/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_bottle/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.599365 newrelic-9.9.1/tests/framework_cherrypy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_cherrypy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_cherrypy/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_cherrypy/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_cherrypy/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_cherrypy/test_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.599365 newrelic-9.9.1/tests/framework_django/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_django/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_django/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.599365 newrelic-9.9.1/tests/framework_django/dummy_app/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_django/dummy_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.599365 newrelic-9.9.1/tests/framework_django/dummy_app/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_django/dummy_app/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_django/dummy_app/templatetags/custom_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_django/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.599365 newrelic-9.9.1/tests/framework_django/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_django/templates/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_django/templates/render_exception.html
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_django/templates/results.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22716 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_django/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_django/test_asgi_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_django/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_django/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_django/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.599365 newrelic-9.9.1/tests/framework_falcon/
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_falcon/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_falcon/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_falcon/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.599365 newrelic-9.9.1/tests/framework_fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_fastapi/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_fastapi/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_fastapi/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.603365 newrelic-9.9.1/tests/framework_flask/
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/_test_application_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/_test_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/_test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/_test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/_test_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/_test_user_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/_test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/_test_views_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/test_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/test_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/test_user_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_flask/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.603365 newrelic-9.9.1/tests/framework_graphene/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_graphene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_graphene/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_graphene/_target_schema_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_graphene/_target_schema_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_graphene/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_graphene/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.607365 newrelic-9.9.1/tests/framework_graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_graphql/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_graphql/_target_schema_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_graphql/_target_schema_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_graphql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21392 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_graphql/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_graphql/test_application_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.607365 newrelic-9.9.1/tests/framework_grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_grpc/_test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_grpc/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.607365 newrelic-9.9.1/tests/framework_grpc/sample_application/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_grpc/sample_application/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_grpc/sample_application/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_grpc/sample_application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_grpc/sample_application/sample_application.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_grpc/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_grpc/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_grpc/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_grpc/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.607365 newrelic-9.9.1/tests/framework_pyramid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_pyramid/_test_append_slash_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_pyramid/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_pyramid/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_pyramid/test_append_slash_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_pyramid/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_pyramid/test_cornice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.607365 newrelic-9.9.1/tests/framework_sanic/
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_sanic/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_sanic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13507 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_sanic/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_sanic/test_cross_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.611365 newrelic-9.9.1/tests/framework_starlette/
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_starlette/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_starlette/_test_bg_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_starlette/_test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_starlette/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_starlette/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_starlette/test_bg_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.611365 newrelic-9.9.1/tests/framework_strawberry/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_strawberry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_strawberry/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_strawberry/_target_schema_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_strawberry/_target_schema_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_strawberry/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_strawberry/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.611365 newrelic-9.9.1/tests/framework_tornado/
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_tornado/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_tornado/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_tornado/test_custom_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_tornado/test_externals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_tornado/test_inbound_cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/framework_tornado/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.611365 newrelic-9.9.1/tests/logger_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_logging/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_logging/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_logging/test_local_decorating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_logging/test_log_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_logging/test_logging_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_logging/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_logging/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.615365 newrelic-9.9.1/tests/logger_loguru/
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_loguru/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_loguru/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_loguru/test_local_decorating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_loguru/test_log_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_loguru/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_loguru/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.615365 newrelic-9.9.1/tests/logger_structlog/
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_structlog/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_structlog/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_structlog/test_local_decorating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_structlog/test_log_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/logger_structlog/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.615365 newrelic-9.9.1/tests/messagebroker_confluentkafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_confluentkafka/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_confluentkafka/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_confluentkafka/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_confluentkafka/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.615365 newrelic-9.9.1/tests/messagebroker_kafkapython/
+-rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_kafkapython/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_kafkapython/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_kafkapython/test_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_kafkapython/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_kafkapython/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.619365 newrelic-9.9.1/tests/messagebroker_pika/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_pika/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_pika/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_pika/minversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_pika/test_cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_pika/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_pika/test_memory_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17114 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_pika/test_pika_async_connection_consume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_pika/test_pika_blocking_connection_consume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13879 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_pika/test_pika_produce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/messagebroker_pika/test_pika_supportability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.619365 newrelic-9.9.1/tests/mlmodel_langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_langchain/_mock_external_openai_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_langchain/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_langchain/hello.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_langchain/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53200 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_langchain/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16916 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_langchain/test_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17598 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_langchain/test_vectorstore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.623365 newrelic-9.9.1/tests/mlmodel_openai/
+-rw-r--r--   0 runner    (1001) docker     (127)    55141 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_openai/_mock_external_openai_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13416 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_openai/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16526 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23654 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18574 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion_error_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17200 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28903 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion_stream_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion_stream_error_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17722 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion_stream_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_openai/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19152 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_openai/test_embeddings_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15641 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_openai/test_embeddings_error_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_openai/test_embeddings_stream_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_openai/test_embeddings_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.627365 newrelic-9.9.1/tests/mlmodel_sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_calibration_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_cluster_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_compose_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_covariance_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_cross_decomposition_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_discriminant_analysis_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_dummy_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_ensemble_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_feature_selection_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_gaussian_process_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12412 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_inference_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_kernel_ridge_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14219 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_linear_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_metric_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_mixture_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_ml_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_model_selection_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_multiclass_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_multioutput_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_naive_bayes_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_neighbors_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_neural_network_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_pipeline_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26289 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_prediction_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_semi_supervised_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_svm_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/mlmodel_sklearn/test_tree_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.627365 newrelic-9.9.1/tests/template_genshi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/template_genshi/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/template_genshi/test_genshi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.627365 newrelic-9.9.1/tests/template_jinja2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/template_jinja2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/template_jinja2/test_jinja2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.627365 newrelic-9.9.1/tests/template_mako/
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/template_mako/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/template_mako/test_mako.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.631365 newrelic-9.9.1/tests/testing_support/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/asgi_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9612 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/db_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/external_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.631365 newrelic-9.9.1/tests/testing_support/fixture/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/fixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/fixture/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50802 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/ml_testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/mock_external_grpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/mock_external_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/mock_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/sample_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/sample_asgi_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:38.639365 newrelic-9.9.1/tests/testing_support/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_apdex_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_application_error_event_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_application_error_trace_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_application_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_browser_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_cross_process_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_custom_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_custom_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_custom_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_custom_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_database_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_database_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_database_trace_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_datastore_trace_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_dimensional_metric_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_dimensional_metrics_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_distributed_trace_accepted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_distributed_tracing_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_error_event_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_error_event_attributes_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_error_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_error_trace_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_error_trace_attributes_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_error_trace_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_external_node_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_function_called.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_internal_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_log_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_log_event_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_log_event_count_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_log_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_log_events_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_messagebroker_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_metric_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_ml_event_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_ml_event_count_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_ml_event_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_ml_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_ml_events_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_non_transaction_error_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_outbound_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_serverless_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_serverless_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_serverless_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_slow_sql_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_span_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_sql_obfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_synthetics_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_synthetics_transaction_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_time_metrics_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_transaction_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_transaction_error_event_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_transaction_error_trace_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_transaction_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_transaction_event_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_transaction_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_transaction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_transaction_slow_sql_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_transaction_trace_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_tt_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_tt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-13 21:39:33.000000 newrelic-9.9.1/tests/testing_support/validators/validate_tt_segment_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26753 2024-05-13 21:39:33.000000 newrelic-9.9.1/tox.ini
```

### Comparing `newrelic-9.9.0/.devcontainer/Dockerfile` & `newrelic-9.9.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.devcontainer/devcontainer.json` & `newrelic-9.9.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/ISSUE_TEMPLATE/bug_report.md` & `newrelic-9.9.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/ISSUE_TEMPLATE/config.yml` & `newrelic-9.9.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/ISSUE_TEMPLATE/feature_request.md` & `newrelic-9.9.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/containers/Dockerfile` & `newrelic-9.9.1/.github/containers/Dockerfile`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/containers/Makefile` & `newrelic-9.9.1/.github/containers/Makefile`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/containers/install-python.sh` & `newrelic-9.9.1/.github/containers/install-python.sh`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/dependabot.yml` & `newrelic-9.9.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/mergify.yml` & `newrelic-9.9.1/.github/mergify.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/pull_request_template.md` & `newrelic-9.9.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/scripts/retry.sh` & `newrelic-9.9.1/.github/scripts/retry.sh`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/stale.yml` & `newrelic-9.9.1/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/workflows/build-ci-image.yml` & `newrelic-9.9.1/.github/workflows/build-ci-image.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/workflows/deploy-python.yml` & `newrelic-9.9.1/.github/workflows/deploy-python.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/workflows/get-envs.py` & `newrelic-9.9.1/.github/workflows/get-envs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/workflows/mega-linter.yml` & `newrelic-9.9.1/.github/workflows/mega-linter.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.github/workflows/tests.yml` & `newrelic-9.9.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.gitignore` & `newrelic-9.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/.mega-linter.yml` & `newrelic-9.9.1/.mega-linter.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/CONTRIBUTING.rst` & `newrelic-9.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/LICENSE` & `newrelic-9.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/PKG-INFO` & `newrelic-9.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic
-Version: 9.9.0
+Version: 9.9.1
 Summary: New Relic Python Agent
 Home-page: https://docs.newrelic.com/docs/apm/agents/python-agent/
 Author: New Relic
 Author-email: support@newrelic.com
 Maintainer: New Relic
 Maintainer-email: support@newrelic.com
 License: Apache-2.0
```

### Comparing `newrelic-9.9.0/README.rst` & `newrelic-9.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/ROADMAP.md` & `newrelic-9.9.1/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/THIRD_PARTY_NOTICES.md` & `newrelic-9.9.1/THIRD_PARTY_NOTICES.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/codecov.yml` & `newrelic-9.9.1/codecov.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/__init__.py` & `newrelic-9.9.1/newrelic/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/admin/__init__.py` & `newrelic-9.9.1/newrelic/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/admin/__main__.py` & `newrelic-9.9.1/newrelic/admin/__main__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/admin/debug_console.py` & `newrelic-9.9.1/newrelic/admin/debug_console.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/admin/generate_config.py` & `newrelic-9.9.1/newrelic/admin/generate_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/admin/license_key.py` & `newrelic-9.9.1/newrelic/admin/license_key.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/admin/local_config.py` & `newrelic-9.9.1/newrelic/admin/local_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/admin/network_config.py` & `newrelic-9.9.1/newrelic/admin/network_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/admin/record_deploy.py` & `newrelic-9.9.1/newrelic/admin/record_deploy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/admin/run_program.py` & `newrelic-9.9.1/newrelic/admin/run_program.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/admin/run_python.py` & `newrelic-9.9.1/newrelic/admin/run_python.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/admin/server_config.py` & `newrelic-9.9.1/newrelic/admin/server_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/admin/validate_config.py` & `newrelic-9.9.1/newrelic/admin/validate_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/agent.py` & `newrelic-9.9.1/newrelic/agent.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/__init__.py` & `newrelic-9.9.1/newrelic/api/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/application.py` & `newrelic-9.9.1/newrelic/api/application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/asgi_application.py` & `newrelic-9.9.1/newrelic/api/asgi_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/background_task.py` & `newrelic-9.9.1/newrelic/api/background_task.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/cat_header_mixin.py` & `newrelic-9.9.1/newrelic/api/cat_header_mixin.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/database_trace.py` & `newrelic-9.9.1/newrelic/api/database_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/datastore_trace.py` & `newrelic-9.9.1/newrelic/api/datastore_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/error_trace.py` & `newrelic-9.9.1/newrelic/api/error_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/exceptions.py` & `newrelic-9.9.1/newrelic/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/external_trace.py` & `newrelic-9.9.1/newrelic/api/external_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/function_profile.py` & `newrelic-9.9.1/newrelic/api/function_profile.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/function_trace.py` & `newrelic-9.9.1/newrelic/api/function_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/generator_trace.py` & `newrelic-9.9.1/newrelic/api/generator_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/graphql_trace.py` & `newrelic-9.9.1/newrelic/api/graphql_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/html_insertion.py` & `newrelic-9.9.1/newrelic/api/html_insertion.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/import_hook.py` & `newrelic-9.9.1/newrelic/api/import_hook.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/in_function.py` & `newrelic-9.9.1/newrelic/api/in_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/lambda_handler.py` & `newrelic-9.9.1/newrelic/api/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/log.py` & `newrelic-9.9.1/newrelic/api/log.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/memcache_trace.py` & `newrelic-9.9.1/newrelic/api/memcache_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/message_trace.py` & `newrelic-9.9.1/newrelic/api/message_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/message_transaction.py` & `newrelic-9.9.1/newrelic/api/message_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/ml_model.py` & `newrelic-9.9.1/newrelic/api/ml_model.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/object_wrapper.py` & `newrelic-9.9.1/newrelic/api/object_wrapper.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/out_function.py` & `newrelic-9.9.1/newrelic/api/out_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/post_function.py` & `newrelic-9.9.1/newrelic/api/post_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/pre_function.py` & `newrelic-9.9.1/newrelic/api/pre_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/profile_trace.py` & `newrelic-9.9.1/newrelic/api/profile_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/settings.py` & `newrelic-9.9.1/newrelic/api/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/solr_trace.py` & `newrelic-9.9.1/newrelic/api/solr_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/supportability.py` & `newrelic-9.9.1/newrelic/api/supportability.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/time_trace.py` & `newrelic-9.9.1/newrelic/api/time_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/transaction.py` & `newrelic-9.9.1/newrelic/api/transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/transaction_name.py` & `newrelic-9.9.1/newrelic/api/transaction_name.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/web_transaction.py` & `newrelic-9.9.1/newrelic/api/web_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/api/wsgi_application.py` & `newrelic-9.9.1/newrelic/api/wsgi_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/bootstrap/__init__.py` & `newrelic-9.9.1/newrelic/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/bootstrap/sitecustomize.py` & `newrelic-9.9.1/newrelic/bootstrap/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/__init__.py` & `newrelic-9.9.1/newrelic/common/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/_monotonic.c` & `newrelic-9.9.1/newrelic/common/_monotonic.c`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/agent_http.py` & `newrelic-9.9.1/newrelic/common/agent_http.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/async_proxy.py` & `newrelic-9.9.1/newrelic/common/async_proxy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/async_wrapper.py` & `newrelic-9.9.1/newrelic/common/async_wrapper.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/cacert.pem` & `newrelic-9.9.1/newrelic/common/cacert.pem`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/certs.py` & `newrelic-9.9.1/newrelic/common/certs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/coroutine.py` & `newrelic-9.9.1/newrelic/common/coroutine.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/encoding_utils.py` & `newrelic-9.9.1/newrelic/common/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/log_file.py` & `newrelic-9.9.1/newrelic/common/log_file.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/metric_utils.py` & `newrelic-9.9.1/newrelic/common/metric_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/object_names.py` & `newrelic-9.9.1/newrelic/common/object_names.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/object_wrapper.py` & `newrelic-9.9.1/newrelic/common/object_wrapper.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/package_version_utils.py` & `newrelic-9.9.1/newrelic/common/package_version_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/signature.py` & `newrelic-9.9.1/newrelic/common/signature.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/stopwatch.py` & `newrelic-9.9.1/newrelic/common/stopwatch.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/streaming_utils.py` & `newrelic-9.9.1/newrelic/common/streaming_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/system_info.py` & `newrelic-9.9.1/newrelic/common/system_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/common/utilization.py` & `newrelic-9.9.1/newrelic/common/utilization.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/config.py` & `newrelic-9.9.1/newrelic/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -2405,14 +2405,20 @@
     _process_module_definition(
         "langchain_community.vectorstores.opensearch_vector_search",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
+        "langchain_community.vectorstores.oraclevs",
+        "newrelic.hooks.mlmodel_langchain",
+        "instrument_langchain_vectorstore_similarity_search",
+    )
+
+    _process_module_definition(
         "langchain_community.vectorstores.pathway",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
         "langchain_community.vectorstores.pgembedding",
@@ -2441,14 +2447,20 @@
     _process_module_definition(
         "langchain_community.vectorstores.qdrant",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
+        "langchain_community.vectorstores.relyt",
+        "newrelic.hooks.mlmodel_langchain",
+        "instrument_langchain_vectorstore_similarity_search",
+    )
+
+    _process_module_definition(
         "langchain_community.vectorstores.rocksetdb",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
         "langchain_community.vectorstores.scann",
@@ -2543,14 +2555,20 @@
     _process_module_definition(
         "langchain_community.vectorstores.typesense",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
+        "langchain_community.vectorstores.upstash",
+        "newrelic.hooks.mlmodel_langchain",
+        "instrument_langchain_vectorstore_similarity_search",
+    )
+
+    _process_module_definition(
         "langchain_community.vectorstores.usearch",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
         "langchain_community.vectorstores.vald",
@@ -2579,14 +2597,20 @@
     _process_module_definition(
         "langchain_community.vectorstores.vespa",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
+        "langchain_community.vectorstores.vlite",
+        "newrelic.hooks.mlmodel_langchain",
+        "instrument_langchain_vectorstore_similarity_search",
+    )
+
+    _process_module_definition(
         "langchain_community.vectorstores.weaviate",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
         "langchain_community.vectorstores.xata",
@@ -4346,14 +4370,19 @@
         "instrument_celery_app_task",
     )
     _process_module_definition(
         "celery.app.task",
         "newrelic.hooks.application_celery",
         "instrument_celery_app_task",
     )
+    _process_module_definition(
+        "celery.app.trace",
+        "newrelic.hooks.application_celery",
+        "instrument_celery_app_trace",
+    )
     _process_module_definition("celery.worker", "newrelic.hooks.application_celery", "instrument_celery_worker")
     _process_module_definition(
         "celery.concurrency.processes",
         "newrelic.hooks.application_celery",
         "instrument_celery_worker",
     )
     _process_module_definition(
```

### Comparing `newrelic-9.9.0/newrelic/console.py` & `newrelic-9.9.1/newrelic/console.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/__init__.py` & `newrelic-9.9.1/newrelic/core/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/_thread_utilization.c` & `newrelic-9.9.1/newrelic/core/_thread_utilization.c`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/adaptive_sampler.py` & `newrelic-9.9.1/newrelic/core/adaptive_sampler.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/agent.py` & `newrelic-9.9.1/newrelic/core/agent.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/agent_protocol.py` & `newrelic-9.9.1/newrelic/core/agent_protocol.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/agent_streaming.py` & `newrelic-9.9.1/newrelic/core/agent_streaming.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/application.py` & `newrelic-9.9.1/newrelic/core/application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/attribute.py` & `newrelic-9.9.1/newrelic/core/attribute.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/attribute_filter.py` & `newrelic-9.9.1/newrelic/core/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/code_level_metrics.py` & `newrelic-9.9.1/newrelic/core/code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/config.py` & `newrelic-9.9.1/newrelic/core/config.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/context.py` & `newrelic-9.9.1/newrelic/core/context.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/custom_event.py` & `newrelic-9.9.1/newrelic/core/custom_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/data_collector.py` & `newrelic-9.9.1/newrelic/core/data_collector.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/database_node.py` & `newrelic-9.9.1/newrelic/core/database_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/database_utils.py` & `newrelic-9.9.1/newrelic/core/database_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/datastore_node.py` & `newrelic-9.9.1/newrelic/core/datastore_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/environment.py` & `newrelic-9.9.1/newrelic/core/environment.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/error_collector.py` & `newrelic-9.9.1/newrelic/core/error_collector.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/error_node.py` & `newrelic-9.9.1/newrelic/core/error_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/external_node.py` & `newrelic-9.9.1/newrelic/core/external_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/function_node.py` & `newrelic-9.9.1/newrelic/core/function_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/graphql_node.py` & `newrelic-9.9.1/newrelic/core/graphql_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/graphql_utils.py` & `newrelic-9.9.1/newrelic/core/graphql_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/infinite_tracing_pb2.py` & `newrelic-9.9.1/newrelic/core/infinite_tracing_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/infinite_tracing_v3_pb2.py` & `newrelic-9.9.1/newrelic/core/infinite_tracing_v3_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/infinite_tracing_v4_pb2.py` & `newrelic-9.9.1/newrelic/core/infinite_tracing_v4_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/internal_metrics.py` & `newrelic-9.9.1/newrelic/core/internal_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/log_event_node.py` & `newrelic-9.9.1/newrelic/core/log_event_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/loop_node.py` & `newrelic-9.9.1/newrelic/core/loop_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/memcache_node.py` & `newrelic-9.9.1/newrelic/core/memcache_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/message_node.py` & `newrelic-9.9.1/newrelic/core/message_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/metric.py` & `newrelic-9.9.1/newrelic/core/metric.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/node_mixin.py` & `newrelic-9.9.1/newrelic/core/node_mixin.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/otlp_utils.py` & `newrelic-9.9.1/newrelic/core/otlp_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/profile_sessions.py` & `newrelic-9.9.1/newrelic/core/profile_sessions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/root_node.py` & `newrelic-9.9.1/newrelic/core/root_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/rules_engine.py` & `newrelic-9.9.1/newrelic/core/rules_engine.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/solr_node.py` & `newrelic-9.9.1/newrelic/core/solr_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/stack_trace.py` & `newrelic-9.9.1/newrelic/core/stack_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/stats_engine.py` & `newrelic-9.9.1/newrelic/core/stats_engine.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/string_table.py` & `newrelic-9.9.1/newrelic/core/string_table.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/thread_utilization.py` & `newrelic-9.9.1/newrelic/core/thread_utilization.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/trace_cache.py` & `newrelic-9.9.1/newrelic/core/trace_cache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/trace_node.py` & `newrelic-9.9.1/newrelic/core/trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/core/transaction_node.py` & `newrelic-9.9.1/newrelic/core/transaction_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/extras/__init__.py` & `newrelic-9.9.1/newrelic/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/extras/framework_django/__init__.py` & `newrelic-9.9.1/newrelic/extras/framework_django/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/extras/framework_django/templatetags/__init__.py` & `newrelic-9.9.1/newrelic/extras/framework_django/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/extras/framework_django/templatetags/newrelic_tags.py` & `newrelic-9.9.1/newrelic/extras/framework_django/templatetags/newrelic_tags.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/__init__.py` & `newrelic-9.9.1/newrelic/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/adapter_asgiref.py` & `newrelic-9.9.1/newrelic/hooks/adapter_asgiref.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/adapter_cheroot.py` & `newrelic-9.9.1/newrelic/hooks/adapter_cheroot.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/adapter_cherrypy.py` & `newrelic-9.9.1/newrelic/hooks/adapter_cherrypy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/adapter_daphne.py` & `newrelic-9.9.1/newrelic/hooks/adapter_daphne.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/adapter_flup.py` & `newrelic-9.9.1/newrelic/hooks/adapter_flup.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/adapter_gevent.py` & `newrelic-9.9.1/newrelic/hooks/adapter_gevent.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/adapter_gunicorn.py` & `newrelic-9.9.1/newrelic/hooks/adapter_gunicorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/adapter_hypercorn.py` & `newrelic-9.9.1/newrelic/hooks/adapter_hypercorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/adapter_meinheld.py` & `newrelic-9.9.1/newrelic/hooks/adapter_meinheld.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/adapter_paste.py` & `newrelic-9.9.1/newrelic/hooks/adapter_paste.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/adapter_uvicorn.py` & `newrelic-9.9.1/newrelic/hooks/adapter_uvicorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/adapter_waitress.py` & `newrelic-9.9.1/newrelic/hooks/adapter_waitress.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/adapter_wsgiref.py` & `newrelic-9.9.1/newrelic/hooks/adapter_wsgiref.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/application_celery.py` & `newrelic-9.9.1/newrelic/hooks/application_celery.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,53 +24,55 @@
 
 from newrelic.api.application import application_instance
 from newrelic.api.background_task import BackgroundTask
 from newrelic.api.function_trace import FunctionTrace
 from newrelic.api.message_trace import MessageTrace
 from newrelic.api.pre_function import wrap_pre_function
 from newrelic.api.transaction import current_transaction
-from newrelic.common.object_wrapper import FunctionWrapper, wrap_function_wrapper
+from newrelic.common.object_wrapper import FunctionWrapper, wrap_function_wrapper, _NRBoundFunctionWrapper
 from newrelic.core.agent import shutdown_agent
 
 UNKNOWN_TASK_NAME = "<Unknown Task>"
 MAPPING_TASK_NAMES = {"celery.starmap", "celery.map"}
 
 
-def task_name(*args, **kwargs):
+def task_info(instance, *args, **kwargs):
     # Grab the current task, which can be located in either place
-    if args:
+    if instance:
+        task = instance
+    elif args:
         task = args[0]
     elif "task" in kwargs:
         task = kwargs["task"]
     else:
         return UNKNOWN_TASK_NAME  # Failsafe
 
     # Task can be either a task instance or a signature, which subclasses dict, or an actual dict in some cases.
     task_name = getattr(task, "name", None) or task.get("task", UNKNOWN_TASK_NAME)
+    task_source = task
 
     # Under mapping tasks, the root task name isn't descriptive enough so we append the
     # subtask name to differentiate between different mapping tasks
     if task_name in MAPPING_TASK_NAMES:
         try:
             subtask = kwargs["task"]["task"]
             task_name = "/".join((task_name, subtask))
+            task_source = task.app._tasks[subtask]
         except Exception:
             pass
 
-    return task_name
+    return task_name, task_source
 
 
 def CeleryTaskWrapper(wrapped):
     def wrapper(wrapped, instance, args, kwargs):
         transaction = current_transaction(active_only=False)
 
-        if instance is not None:
-            _name = task_name(instance, *args, **kwargs)
-        else:
-            _name = task_name(*args, **kwargs)
+        # Grab task name and source
+        _name, _source = task_info(instance, *args, **kwargs)
 
         # A Celery Task can be called either outside of a transaction, or
         # within the context of an existing transaction. There are 3
         # possibilities we need to handle:
         #
         #   1. In an inactive transaction
         #
@@ -89,19 +91,19 @@
         #      running inside of an existing transaction, we want to create
         #      a new background transaction for it.
 
         if transaction and (transaction.ignore_transaction or transaction.stopped):
             return wrapped(*args, **kwargs)
 
         elif transaction:
-            with FunctionTrace(_name, source=instance):
+            with FunctionTrace(_name, source=_source):
                 return wrapped(*args, **kwargs)
 
         else:
-            with BackgroundTask(application_instance(), _name, "Celery", source=instance) as transaction:
+            with BackgroundTask(application_instance(), _name, "Celery", source=_source) as transaction:
                 # Attempt to grab distributed tracing headers
                 try:
                     # Headers on earlier versions of Celery may end up as attributes
                     # on the request context instead of as custom headers. Handler this
                     # by defaulting to using vars() if headers is not available
                     request = instance.request
                     headers = getattr(request, "headers", None) or vars(request)
@@ -196,14 +198,34 @@
                 dt_headers.update(dict(original_headers))
     except Exception:
         pass
 
     return wrapped(*args, **kwargs)
 
 
+def wrap_worker_optimizations(wrapped, instance, args, kwargs):
+    # Attempt to uninstrument BaseTask before stack protection is installed or uninstalled
+    try:
+        from celery.app.task import BaseTask
+
+        if isinstance(BaseTask.__call__, _NRBoundFunctionWrapper):
+            BaseTask.__call__ = BaseTask.__call__.__wrapped__
+    except Exception:
+        BaseTask = None
+
+    # Allow metaprogramming to run
+    result = wrapped(*args, **kwargs)
+
+    # Rewrap finalized BaseTask
+    if BaseTask:  # Ensure imports succeeded
+        BaseTask.__call__ = CeleryTaskWrapper(BaseTask.__call__)
+    
+    return result
+
+
 def instrument_celery_app_base(module):
     if hasattr(module, "Celery") and hasattr(module.Celery, "send_task"):
         wrap_function_wrapper(module, "Celery.send_task", wrap_Celery_send_task)
 
 
 def instrument_celery_worker(module):
     # Triggered for 'celery.worker' and 'celery.concurrency.processes'.
@@ -235,7 +257,16 @@
 
 def instrument_billiard_pool(module):
     def force_agent_shutdown(*args, **kwargs):
         shutdown_agent()
 
     if hasattr(module, "Worker"):
         wrap_pre_function(module, "Worker._do_exit", force_agent_shutdown)
+
+
+def instrument_celery_app_trace(module):
+    # Uses same wrapper for setup and reset worker optimizations to prevent patching and unpatching from removing wrappers
+    if hasattr(module, "setup_worker_optimizations"):
+        wrap_function_wrapper(module, "setup_worker_optimizations", wrap_worker_optimizations)
+
+    if hasattr(module, "reset_worker_optimizations"):
+        wrap_function_wrapper(module, "reset_worker_optimizations", wrap_worker_optimizations)
```

### Comparing `newrelic-9.9.0/newrelic/hooks/application_gearman.py` & `newrelic-9.9.1/newrelic/hooks/application_gearman.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/component_cornice.py` & `newrelic-9.9.1/newrelic/hooks/component_cornice.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/component_djangorestframework.py` & `newrelic-9.9.1/newrelic/hooks/component_djangorestframework.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/component_flask_rest.py` & `newrelic-9.9.1/newrelic/hooks/component_flask_rest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/component_graphqlserver.py` & `newrelic-9.9.1/newrelic/hooks/component_graphqlserver.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/component_piston.py` & `newrelic-9.9.1/newrelic/hooks/component_piston.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/component_sentry.py` & `newrelic-9.9.1/newrelic/hooks/component_sentry.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/component_tastypie.py` & `newrelic-9.9.1/newrelic/hooks/component_tastypie.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/coroutines_asyncio.py` & `newrelic-9.9.1/newrelic/hooks/coroutines_asyncio.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/coroutines_gevent.py` & `newrelic-9.9.1/newrelic/hooks/coroutines_gevent.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/database_asyncpg.py` & `newrelic-9.9.1/newrelic/hooks/database_asyncpg.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/database_cx_oracle.py` & `newrelic-9.9.1/newrelic/hooks/database_cx_oracle.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/database_dbapi2.py` & `newrelic-9.9.1/newrelic/hooks/database_dbapi2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/database_ibm_db_dbi.py` & `newrelic-9.9.1/newrelic/hooks/database_ibm_db_dbi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/database_mysql.py` & `newrelic-9.9.1/newrelic/hooks/database_mysql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/database_mysqldb.py` & `newrelic-9.9.1/newrelic/hooks/database_mysqldb.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/database_oursql.py` & `newrelic-9.9.1/newrelic/hooks/database_oursql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/database_postgresql.py` & `newrelic-9.9.1/newrelic/hooks/database_postgresql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/database_psycopg2.py` & `newrelic-9.9.1/newrelic/hooks/database_psycopg2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/database_psycopg2cffi.py` & `newrelic-9.9.1/newrelic/hooks/database_psycopg2cffi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/database_psycopg2ct.py` & `newrelic-9.9.1/newrelic/hooks/database_psycopg2ct.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/database_pymssql.py` & `newrelic-9.9.1/newrelic/hooks/database_pymssql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/database_pymysql.py` & `newrelic-9.9.1/newrelic/hooks/database_pymysql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/database_pyodbc.py` & `newrelic-9.9.1/newrelic/hooks/database_pyodbc.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/database_sqlite.py` & `newrelic-9.9.1/newrelic/hooks/database_sqlite.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/datastore_aioredis.py` & `newrelic-9.9.1/newrelic/hooks/datastore_aioredis.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/datastore_aredis.py` & `newrelic-9.9.1/newrelic/hooks/datastore_aredis.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/datastore_bmemcached.py` & `newrelic-9.9.1/newrelic/hooks/datastore_bmemcached.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/datastore_elasticsearch.py` & `newrelic-9.9.1/newrelic/hooks/datastore_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/datastore_firestore.py` & `newrelic-9.9.1/newrelic/hooks/datastore_firestore.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/datastore_memcache.py` & `newrelic-9.9.1/newrelic/hooks/datastore_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/datastore_motor.py` & `newrelic-9.9.1/newrelic/hooks/datastore_motor.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/datastore_pyelasticsearch.py` & `newrelic-9.9.1/newrelic/hooks/datastore_pyelasticsearch.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/datastore_pylibmc.py` & `newrelic-9.9.1/newrelic/hooks/datastore_pylibmc.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/datastore_pymemcache.py` & `newrelic-9.9.1/newrelic/hooks/datastore_pymemcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/datastore_pymongo.py` & `newrelic-9.9.1/newrelic/hooks/datastore_pymongo.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/datastore_pysolr.py` & `newrelic-9.9.1/newrelic/hooks/datastore_pysolr.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/datastore_redis.py` & `newrelic-9.9.1/newrelic/hooks/datastore_redis.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/datastore_solrpy.py` & `newrelic-9.9.1/newrelic/hooks/datastore_solrpy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/datastore_umemcache.py` & `newrelic-9.9.1/newrelic/hooks/datastore_umemcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/external_botocore.py` & `newrelic-9.9.1/newrelic/hooks/external_botocore.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/external_dropbox.py` & `newrelic-9.9.1/newrelic/hooks/external_dropbox.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/external_facepy.py` & `newrelic-9.9.1/newrelic/hooks/external_facepy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/external_feedparser.py` & `newrelic-9.9.1/newrelic/hooks/external_feedparser.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/external_httplib.py` & `newrelic-9.9.1/newrelic/hooks/external_httplib.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/external_httplib2.py` & `newrelic-9.9.1/newrelic/hooks/external_httplib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/external_httpx.py` & `newrelic-9.9.1/newrelic/hooks/external_httpx.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/external_pywapi.py` & `newrelic-9.9.1/newrelic/hooks/external_pywapi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/external_requests.py` & `newrelic-9.9.1/newrelic/hooks/external_requests.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/external_thrift.py` & `newrelic-9.9.1/newrelic/hooks/external_thrift.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/external_urllib.py` & `newrelic-9.9.1/newrelic/hooks/external_urllib.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/external_urllib2.py` & `newrelic-9.9.1/newrelic/hooks/external_urllib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/external_xmlrpclib.py` & `newrelic-9.9.1/newrelic/hooks/external_xmlrpclib.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_aiohttp.py` & `newrelic-9.9.1/newrelic/hooks/framework_aiohttp.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_ariadne.py` & `newrelic-9.9.1/newrelic/hooks/framework_ariadne.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_bottle.py` & `newrelic-9.9.1/newrelic/hooks/framework_bottle.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_cherrypy.py` & `newrelic-9.9.1/newrelic/hooks/framework_cherrypy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_django.py` & `newrelic-9.9.1/newrelic/hooks/framework_django.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_django_py3.py` & `newrelic-9.9.1/newrelic/hooks/framework_django_py3.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_falcon.py` & `newrelic-9.9.1/newrelic/hooks/framework_falcon.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_fastapi.py` & `newrelic-9.9.1/newrelic/hooks/framework_fastapi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_flask.py` & `newrelic-9.9.1/newrelic/hooks/framework_flask.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_graphene.py` & `newrelic-9.9.1/newrelic/hooks/framework_graphene.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_graphql.py` & `newrelic-9.9.1/newrelic/hooks/framework_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_graphql_py3.py` & `newrelic-9.9.1/newrelic/hooks/framework_graphql_py3.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_grpc.py` & `newrelic-9.9.1/newrelic/hooks/framework_grpc.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,111 +12,105 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import random
 import time
 
 from newrelic.api.external_trace import ExternalTrace
-from newrelic.api.web_transaction import WebTransactionWrapper
-from newrelic.api.transaction import current_transaction
 from newrelic.api.time_trace import notice_error
-from newrelic.common.object_wrapper import wrap_function_wrapper
+from newrelic.api.transaction import current_transaction
+from newrelic.api.web_transaction import WebTransactionWrapper
 from newrelic.common.object_names import callable_name
+from newrelic.common.object_wrapper import wrap_function_wrapper
 
 
 def _get_uri_method(instance, *args, **kwargs):
-    target = instance._channel.target().decode('utf-8')
-    method = instance._method.decode('utf-8').lstrip('/')
-    uri = 'grpc://%s/%s' % (target, method)
+    target = instance._channel.target().decode("utf-8").lstrip("dns:///")
+    method = instance._method.decode("utf-8").lstrip("/")
+    uri = "grpc://%s/%s" % (target, method)
     return (uri, method)
 
 
-def _prepare_request(
-        transaction, guid, request,
-        timeout=None, metadata=None, *args, **kwargs):
+def _prepare_request(transaction, guid, request, timeout=None, metadata=None, *args, **kwargs):
     metadata = metadata and list(metadata) or []
     dt_metadata = transaction._create_distributed_trace_data_with_guid(guid)
-    metadata.extend(
-        transaction._generate_distributed_trace_headers(dt_metadata)
-    )
+    metadata.extend(transaction._generate_distributed_trace_headers(dt_metadata))
     args = (request, timeout, metadata) + args
     return args, kwargs
 
 
-def _prepare_request_stream(
-        transaction, guid, request_iterator, *args, **kwargs):
-    return _prepare_request(
-            transaction, guid, request_iterator, *args, **kwargs)
+def _prepare_request_stream(transaction, guid, request_iterator, *args, **kwargs):
+    return _prepare_request(transaction, guid, request_iterator, *args, **kwargs)
 
 
 def wrap_call(module, object_path, prepare):
 
     def _call_wrapper(wrapped, instance, args, kwargs):
         transaction = current_transaction()
         if transaction is None:
             return wrapped(*args, **kwargs)
 
         uri, method = _get_uri_method(instance)
-        with ExternalTrace('gRPC', uri, method, source=wrapped):
+        with ExternalTrace("gRPC", uri, method, source=wrapped):
             args, kwargs = prepare(transaction, None, *args, **kwargs)
             return wrapped(*args, **kwargs)
 
     wrap_function_wrapper(module, object_path, _call_wrapper)
 
 
 def wrap_future(module, object_path, prepare):
 
     def _future_wrapper(wrapped, instance, args, kwargs):
         transaction = current_transaction()
         if transaction is None:
             return wrapped(*args, **kwargs)
 
-        guid = '%016x' % random.getrandbits(64)
+        guid = "%016x" % random.getrandbits(64)
         uri, method = _get_uri_method(instance)
 
         args, kwargs = prepare(transaction, guid, *args, **kwargs)
         future = wrapped(*args, **kwargs)
         future._nr_guid = guid
-        future._nr_args = {"library": 'gRPC', "url": uri, "method": method, "source": wrapped}
+        future._nr_args = {"library": "gRPC", "url": uri, "method": method, "source": wrapped}
         future._nr_start_time = time.time()
 
         # In non-streaming responses, result is typically called instead of
         # using the iterator. In streaming calls, the iterator is typically
         # used.
 
         return future
 
     wrap_function_wrapper(module, object_path, _future_wrapper)
 
 
 def wrap_next(_wrapped, _instance, _args, _kwargs):
-    _nr_args = getattr(_instance, '_nr_args', None)
+    _nr_args = getattr(_instance, "_nr_args", None)
     if not _nr_args:
         return _wrapped(*_args, **_kwargs)
 
     try:
         return _wrapped(*_args, **_kwargs)
     except Exception:
-        delattr(_instance, '_nr_args')
-        _nr_start_time = getattr(_instance, '_nr_start_time', 0.0)
-        _nr_guid = getattr(_instance, '_nr_guid', None)
+        delattr(_instance, "_nr_args")
+        _nr_start_time = getattr(_instance, "_nr_start_time", 0.0)
+        _nr_guid = getattr(_instance, "_nr_guid", None)
 
         with ExternalTrace(**_nr_args) as t:
             t.start_time = _nr_start_time or t.start_time
             t.guid = _nr_guid or t.guid
             raise
 
 
 def wrap_result(_wrapped, _instance, _args, _kwargs):
-    _nr_args = getattr(_instance, '_nr_args', None)
+    _nr_args = getattr(_instance, "_nr_args", None)
     if not _nr_args:
         return _wrapped(*_args, **_kwargs)
-    delattr(_instance, '_nr_args')
-    _nr_start_time = getattr(_instance, '_nr_start_time', 0.0)
-    _nr_guid = getattr(_instance, '_nr_guid', None)
+    delattr(_instance, "_nr_args")
+    _nr_start_time = getattr(_instance, "_nr_start_time", 0.0)
+    _nr_guid = getattr(_instance, "_nr_guid", None)
 
     try:
         result = _wrapped(*_args, **_kwargs)
     except Exception:
         with ExternalTrace(**_nr_args) as t:
             t.start_time = _nr_start_time or t.start_time
             t.guid = _nr_guid or t.guid
@@ -132,39 +126,30 @@
     return rpc_event, behavior
 
 
 def grpc_web_transaction(wrapped, instance, args, kwargs):
     rpc_event, behavior = _bind_transaction_args(*args, **kwargs)
     behavior_name = callable_name(behavior)
 
-    call_details = (
-            getattr(rpc_event, 'call_details', None) or
-            getattr(rpc_event, 'request_call_details', None))
-
-    metadata = (
-            getattr(rpc_event, 'invocation_metadata', None) or
-            getattr(rpc_event, 'request_metadata', None))
+    call_details = getattr(rpc_event, "call_details", None) or getattr(rpc_event, "request_call_details", None)
+
+    metadata = getattr(rpc_event, "invocation_metadata", None) or getattr(rpc_event, "request_metadata", None)
 
     host = port = None
     if call_details:
         try:
-            host, port = call_details.host.split(b':', 1)
+            host, port = call_details.host.split(b":", 1)
         except Exception:
             pass
 
         request_path = call_details.method
 
     return WebTransactionWrapper(
-            wrapped,
-            name=behavior_name,
-            request_path=request_path,
-            host=host,
-            port=port,
-            headers=metadata,
-            source=behavior)(*args, **kwargs)
+        wrapped, name=behavior_name, request_path=request_path, host=host, port=port, headers=metadata, source=behavior
+    )(*args, **kwargs)
 
 
 def _trailing_metadata(state, *args, **kwargs):
     return state.trailing_metadata
 
 
 def _nr_wrap_status_code(wrapped, instance, args, kwargs):
@@ -181,48 +166,30 @@
 def _nr_wrap_abort(wrapped, instance, args, kwargs):
     notice_error()
 
     return wrapped(*args, **kwargs)
 
 
 def instrument_grpc__channel(module):
-    wrap_call(module, '_UnaryUnaryMultiCallable.__call__',
-            _prepare_request)
-    wrap_call(module, '_UnaryUnaryMultiCallable.with_call',
-            _prepare_request)
-    wrap_future(module, '_UnaryUnaryMultiCallable.future',
-            _prepare_request)
-    wrap_future(module, '_UnaryStreamMultiCallable.__call__',
-            _prepare_request)
-    wrap_call(module, '_StreamUnaryMultiCallable.__call__',
-            _prepare_request_stream)
-    wrap_call(module, '_StreamUnaryMultiCallable.with_call',
-            _prepare_request_stream)
-    wrap_future(module, '_StreamUnaryMultiCallable.future',
-            _prepare_request_stream)
-    wrap_future(module, '_StreamStreamMultiCallable.__call__',
-            _prepare_request_stream)
-    if hasattr(module, '_MultiThreadedRendezvous'):
-        wrap_function_wrapper(module, '_MultiThreadedRendezvous.result',
-                wrap_result)
-        wrap_function_wrapper(module, '_MultiThreadedRendezvous._next',
-                wrap_next)
+    wrap_call(module, "_UnaryUnaryMultiCallable.__call__", _prepare_request)
+    wrap_call(module, "_UnaryUnaryMultiCallable.with_call", _prepare_request)
+    wrap_future(module, "_UnaryUnaryMultiCallable.future", _prepare_request)
+    wrap_future(module, "_UnaryStreamMultiCallable.__call__", _prepare_request)
+    wrap_call(module, "_StreamUnaryMultiCallable.__call__", _prepare_request_stream)
+    wrap_call(module, "_StreamUnaryMultiCallable.with_call", _prepare_request_stream)
+    wrap_future(module, "_StreamUnaryMultiCallable.future", _prepare_request_stream)
+    wrap_future(module, "_StreamStreamMultiCallable.__call__", _prepare_request_stream)
+    if hasattr(module, "_MultiThreadedRendezvous"):
+        wrap_function_wrapper(module, "_MultiThreadedRendezvous.result", wrap_result)
+        wrap_function_wrapper(module, "_MultiThreadedRendezvous._next", wrap_next)
     else:
-        wrap_function_wrapper(module, '_Rendezvous.result',
-                wrap_result)
-        wrap_function_wrapper(module, '_Rendezvous._next',
-                wrap_next)
-    wrap_function_wrapper(module, '_Rendezvous.cancel',
-            wrap_result)
+        wrap_function_wrapper(module, "_Rendezvous.result", wrap_result)
+        wrap_function_wrapper(module, "_Rendezvous._next", wrap_next)
+    wrap_function_wrapper(module, "_Rendezvous.cancel", wrap_result)
 
 
 def instrument_grpc_server(module):
-    wrap_function_wrapper(module, '_unary_response_in_pool',
-            grpc_web_transaction)
-    wrap_function_wrapper(module, '_stream_response_in_pool',
-            grpc_web_transaction)
-    wrap_function_wrapper(module, '_completion_code',
-            _nr_wrap_status_code)
-    wrap_function_wrapper(module, '_abortion_code',
-            _nr_wrap_status_code)
-    wrap_function_wrapper(module, '_abort',
-            _nr_wrap_abort)
+    wrap_function_wrapper(module, "_unary_response_in_pool", grpc_web_transaction)
+    wrap_function_wrapper(module, "_stream_response_in_pool", grpc_web_transaction)
+    wrap_function_wrapper(module, "_completion_code", _nr_wrap_status_code)
+    wrap_function_wrapper(module, "_abortion_code", _nr_wrap_status_code)
+    wrap_function_wrapper(module, "_abort", _nr_wrap_abort)
```

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_pylons.py` & `newrelic-9.9.1/newrelic/hooks/framework_pylons.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_pyramid.py` & `newrelic-9.9.1/newrelic/hooks/framework_pyramid.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_sanic.py` & `newrelic-9.9.1/newrelic/hooks/framework_sanic.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_starlette.py` & `newrelic-9.9.1/newrelic/hooks/framework_starlette.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_strawberry.py` & `newrelic-9.9.1/newrelic/hooks/framework_strawberry.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_tornado.py` & `newrelic-9.9.1/newrelic/hooks/framework_tornado.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_web2py.py` & `newrelic-9.9.1/newrelic/hooks/framework_web2py.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/framework_webpy.py` & `newrelic-9.9.1/newrelic/hooks/framework_webpy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/logger_logging.py` & `newrelic-9.9.1/newrelic/hooks/logger_logging.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/logger_loguru.py` & `newrelic-9.9.1/newrelic/hooks/logger_loguru.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/logger_structlog.py` & `newrelic-9.9.1/newrelic/hooks/logger_structlog.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/memcache_memcache.py` & `newrelic-9.9.1/newrelic/hooks/memcache_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/messagebroker_confluentkafka.py` & `newrelic-9.9.1/newrelic/hooks/messagebroker_confluentkafka.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/messagebroker_kafkapython.py` & `newrelic-9.9.1/newrelic/hooks/messagebroker_kafkapython.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/messagebroker_pika.py` & `newrelic-9.9.1/newrelic/hooks/messagebroker_pika.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/middleware_flask_compress.py` & `newrelic-9.9.1/newrelic/hooks/middleware_flask_compress.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/middleware_weberror.py` & `newrelic-9.9.1/newrelic/hooks/middleware_weberror.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/mlmodel_langchain.py` & `newrelic-9.9.1/newrelic/hooks/mlmodel_langchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,22 +77,24 @@
     "langchain_community.vectorstores.milvus": "Milvus",
     "langchain_community.vectorstores.momento_vector_index": "MomentoVectorIndex",
     "langchain_community.vectorstores.mongodb_atlas": "MongoDBAtlasVectorSearch",
     "langchain_community.vectorstores.myscale": "MyScale",
     "langchain_community.vectorstores.neo4j_vector": "Neo4jVector",
     "langchain_community.vectorstores.thirdai_neuraldb": "NeuralDBVectorStore",
     "langchain_community.vectorstores.nucliadb": "NucliaDB",
+    "langchain_community.vectorstores.oraclevs": "OracleVS",
     "langchain_community.vectorstores.opensearch_vector_search": "OpenSearchVectorSearch",
     "langchain_community.vectorstores.pathway": "PathwayVectorClient",
     "langchain_community.vectorstores.pgembedding": "PGEmbedding",
     "langchain_community.vectorstores.pgvecto_rs": "PGVecto_rs",
     "langchain_community.vectorstores.pgvector": "PGVector",
     "langchain_community.vectorstores.pinecone": "Pinecone",
     "langchain_community.vectorstores.qdrant": "Qdrant",
     "langchain_community.vectorstores.redis.base": "Redis",
+    "langchain_community.vectorstores.relyt": "Relyt",
     "langchain_community.vectorstores.rocksetdb": "Rockset",
     "langchain_community.vectorstores.scann": "ScaNN",
     "langchain_community.vectorstores.semadb": "SemaDB",
     "langchain_community.vectorstores.singlestoredb": "SingleStoreDB",
     "langchain_community.vectorstores.sklearn": "SKLearnVectorStore",
     "langchain_community.vectorstores.sqlitevss": "SQLiteVSS",
     "langchain_community.vectorstores.starrocks": "StarRocks",
@@ -101,20 +103,22 @@
     "langchain_community.vectorstores.tair": "Tair",
     "langchain_community.vectorstores.tencentvectordb": "TencentVectorDB",
     "langchain_community.vectorstores.tidb_vector": "TiDBVectorStore",
     "langchain_community.vectorstores.tigris": "Tigris",
     "langchain_community.vectorstores.tiledb": "TileDB",
     "langchain_community.vectorstores.timescalevector": "TimescaleVector",
     "langchain_community.vectorstores.typesense": "Typesense",
+    "langchain_community.vectorstores.upstash": "UpstashVectorStore",
     "langchain_community.vectorstores.usearch": "USearch",
     "langchain_community.vectorstores.vald": "Vald",
     "langchain_community.vectorstores.vdms": "VDMS",
     "langchain_community.vectorstores.vearch": "Vearch",
     "langchain_community.vectorstores.vectara": "Vectara",
     "langchain_community.vectorstores.vespa": "VespaStore",
+    "langchain_community.vectorstores.vlite": "VLite",
     "langchain_community.vectorstores.weaviate": "Weaviate",
     "langchain_community.vectorstores.xata": "XataVectorStore",
     "langchain_community.vectorstores.yellowbrick": "Yellowbrick",
     "langchain_community.vectorstores.zep": "ZepVectorStore",
     "langchain_community.vectorstores.docarray.hnsw": "DocArrayHnswSearch",
     "langchain_community.vectorstores.docarray.in_memory": "DocArrayInMemorySearch",
 }
```

### Comparing `newrelic-9.9.0/newrelic/hooks/mlmodel_openai.py` & `newrelic-9.9.1/newrelic/hooks/mlmodel_openai.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/mlmodel_sklearn.py` & `newrelic-9.9.1/newrelic/hooks/mlmodel_sklearn.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/template_genshi.py` & `newrelic-9.9.1/newrelic/hooks/template_genshi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/template_jinja2.py` & `newrelic-9.9.1/newrelic/hooks/template_jinja2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/hooks/template_mako.py` & `newrelic-9.9.1/newrelic/hooks/template_mako.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/network/__init__.py` & `newrelic-9.9.1/newrelic/network/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/network/addresses.py` & `newrelic-9.9.1/newrelic/network/addresses.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/network/exceptions.py` & `newrelic-9.9.1/newrelic/network/exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/newrelic.ini` & `newrelic-9.9.1/newrelic/newrelic.ini`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/asgiref_compatibility.py` & `newrelic-9.9.1/newrelic/packages/asgiref_compatibility.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/isort/LICENSE` & `newrelic-9.9.1/newrelic/packages/isort/LICENSE`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/isort/stdlibs/py27.py` & `newrelic-9.9.1/newrelic/packages/isort/stdlibs/py27.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/isort/stdlibs/py310.py` & `newrelic-9.9.1/newrelic/packages/isort/stdlibs/py310.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/isort/stdlibs/py311.py` & `newrelic-9.9.1/newrelic/packages/isort/stdlibs/py311.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/isort/stdlibs/py36.py` & `newrelic-9.9.1/newrelic/packages/isort/stdlibs/py36.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/isort/stdlibs/py37.py` & `newrelic-9.9.1/newrelic/packages/isort/stdlibs/py37.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/isort/stdlibs/py38.py` & `newrelic-9.9.1/newrelic/packages/isort/stdlibs/py38.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/isort/stdlibs/py39.py` & `newrelic-9.9.1/newrelic/packages/isort/stdlibs/py39.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/opentelemetry_proto/LICENSE.txt` & `newrelic-9.9.1/newrelic/packages/opentelemetry_proto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/opentelemetry_proto/common_pb2.py` & `newrelic-9.9.1/newrelic/packages/opentelemetry_proto/common_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/opentelemetry_proto/logs_pb2.py` & `newrelic-9.9.1/newrelic/packages/opentelemetry_proto/logs_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/opentelemetry_proto/metrics_pb2.py` & `newrelic-9.9.1/newrelic/packages/opentelemetry_proto/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/opentelemetry_proto/resource_pb2.py` & `newrelic-9.9.1/newrelic/packages/opentelemetry_proto/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/six.py` & `newrelic-9.9.1/newrelic/packages/six.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/LICENSE.txt` & `newrelic-9.9.1/newrelic/packages/urllib3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/__init__.py` & `newrelic-9.9.1/newrelic/packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/_collections.py` & `newrelic-9.9.1/newrelic/packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/connection.py` & `newrelic-9.9.1/newrelic/packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/connectionpool.py` & `newrelic-9.9.1/newrelic/packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/contrib/_appengine_environ.py` & `newrelic-9.9.1/newrelic/packages/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/contrib/_securetransport/bindings.py` & `newrelic-9.9.1/newrelic/packages/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/contrib/_securetransport/low_level.py` & `newrelic-9.9.1/newrelic/packages/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/contrib/appengine.py` & `newrelic-9.9.1/newrelic/packages/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/contrib/ntlmpool.py` & `newrelic-9.9.1/newrelic/packages/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/contrib/pyopenssl.py` & `newrelic-9.9.1/newrelic/packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/contrib/securetransport.py` & `newrelic-9.9.1/newrelic/packages/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/contrib/socks.py` & `newrelic-9.9.1/newrelic/packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/exceptions.py` & `newrelic-9.9.1/newrelic/packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/fields.py` & `newrelic-9.9.1/newrelic/packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/filepost.py` & `newrelic-9.9.1/newrelic/packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/packages/backports/makefile.py` & `newrelic-9.9.1/newrelic/packages/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/packages/backports/weakref_finalize.py` & `newrelic-9.9.1/newrelic/packages/urllib3/packages/backports/weakref_finalize.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/packages/six.py` & `newrelic-9.9.1/newrelic/packages/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/poolmanager.py` & `newrelic-9.9.1/newrelic/packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/request.py` & `newrelic-9.9.1/newrelic/packages/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/response.py` & `newrelic-9.9.1/newrelic/packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/util/__init__.py` & `newrelic-9.9.1/newrelic/packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/util/connection.py` & `newrelic-9.9.1/newrelic/packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/util/proxy.py` & `newrelic-9.9.1/newrelic/packages/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/util/request.py` & `newrelic-9.9.1/newrelic/packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/util/response.py` & `newrelic-9.9.1/newrelic/packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/util/retry.py` & `newrelic-9.9.1/newrelic/packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/util/ssl_.py` & `newrelic-9.9.1/newrelic/packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/util/ssl_match_hostname.py` & `newrelic-9.9.1/newrelic/packages/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/util/ssltransport.py` & `newrelic-9.9.1/newrelic/packages/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/util/timeout.py` & `newrelic-9.9.1/newrelic/packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/util/url.py` & `newrelic-9.9.1/newrelic/packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/urllib3/util/wait.py` & `newrelic-9.9.1/newrelic/packages/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/wrapt/LICENSE` & `newrelic-9.9.1/newrelic/packages/wrapt/LICENSE`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/wrapt/__init__.py` & `newrelic-9.9.1/newrelic/packages/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/wrapt/_wrappers.c` & `newrelic-9.9.1/newrelic/packages/wrapt/_wrappers.c`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/wrapt/arguments.py` & `newrelic-9.9.1/newrelic/packages/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/wrapt/decorators.py` & `newrelic-9.9.1/newrelic/packages/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/wrapt/importer.py` & `newrelic-9.9.1/newrelic/packages/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/wrapt/patches.py` & `newrelic-9.9.1/newrelic/packages/wrapt/patches.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/wrapt/weakrefs.py` & `newrelic-9.9.1/newrelic/packages/wrapt/weakrefs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/packages/wrapt/wrappers.py` & `newrelic-9.9.1/newrelic/packages/wrapt/wrappers.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/samplers/__init__.py` & `newrelic-9.9.1/newrelic/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/samplers/cpu_usage.py` & `newrelic-9.9.1/newrelic/samplers/cpu_usage.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/samplers/data_sampler.py` & `newrelic-9.9.1/newrelic/samplers/data_sampler.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/samplers/decorators.py` & `newrelic-9.9.1/newrelic/samplers/decorators.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/samplers/gc_data.py` & `newrelic-9.9.1/newrelic/samplers/gc_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic/samplers/memory_usage.py` & `newrelic-9.9.1/newrelic/samplers/memory_usage.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/newrelic.egg-info/PKG-INFO` & `newrelic-9.9.1/newrelic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic
-Version: 9.9.0
+Version: 9.9.1
 Summary: New Relic Python Agent
 Home-page: https://docs.newrelic.com/docs/apm/agents/python-agent/
 Author: New Relic
 Author-email: support@newrelic.com
 Maintainer: New Relic
 Maintainer-email: support@newrelic.com
 License: Apache-2.0
```

### Comparing `newrelic-9.9.0/newrelic.egg-info/SOURCES.txt` & `newrelic-9.9.1/newrelic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -471,14 +471,15 @@
 tests/agent_unittests/test_wrappers.py
 tests/application_celery/_target_application.py
 tests/application_celery/conftest.py
 tests/application_celery/test_application.py
 tests/application_celery/test_distributed_tracing.py
 tests/application_celery/test_max_tasks_per_child.py
 tests/application_celery/test_task_methods.py
+tests/application_celery/test_wrappers.py
 tests/application_gearman/conftest.py
 tests/application_gearman/test_gearman.py
 tests/component_djangorestframework/conftest.py
 tests/component_djangorestframework/settings.py
 tests/component_djangorestframework/test_application.py
 tests/component_djangorestframework/urls.py
 tests/component_djangorestframework/views.py
```

### Comparing `newrelic-9.9.0/setup.py` & `newrelic-9.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_asgiref/conftest.py` & `newrelic-9.9.1/tests/adapter_asgiref/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_asgiref/test_context_propagation.py` & `newrelic-9.9.1/tests/adapter_asgiref/test_context_propagation.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_cheroot/conftest.py` & `newrelic-9.9.1/tests/adapter_cheroot/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_cheroot/test_wsgi.py` & `newrelic-9.9.1/tests/adapter_cheroot/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_daphne/conftest.py` & `newrelic-9.9.1/tests/adapter_daphne/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_daphne/test_daphne.py` & `newrelic-9.9.1/tests/adapter_daphne/test_daphne.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_gevent/_application.py` & `newrelic-9.9.1/tests/adapter_gevent/_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_gevent/conftest.py` & `newrelic-9.9.1/tests/adapter_gevent/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_gevent/test_patching.py` & `newrelic-9.9.1/tests/adapter_gevent/test_patching.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_gevent/test_pywsgi.py` & `newrelic-9.9.1/tests/adapter_gevent/test_pywsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_gunicorn/app.py` & `newrelic-9.9.1/tests/adapter_gunicorn/app.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_gunicorn/asgi_app.py` & `newrelic-9.9.1/tests/adapter_gunicorn/asgi_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_gunicorn/async_app.py` & `newrelic-9.9.1/tests/adapter_gunicorn/async_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_gunicorn/conftest.py` & `newrelic-9.9.1/tests/adapter_gunicorn/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_gunicorn/test_aiohttp_app_factory.py` & `newrelic-9.9.1/tests/adapter_gunicorn/test_aiohttp_app_factory.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_gunicorn/test_asgi_app.py` & `newrelic-9.9.1/tests/adapter_gunicorn/test_asgi_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_gunicorn/test_gaiohttp.py` & `newrelic-9.9.1/tests/adapter_gunicorn/test_gaiohttp.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_gunicorn/worker.py` & `newrelic-9.9.1/tests/adapter_gunicorn/worker.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_hypercorn/conftest.py` & `newrelic-9.9.1/tests/adapter_hypercorn/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_hypercorn/test_hypercorn.py` & `newrelic-9.9.1/tests/adapter_hypercorn/test_hypercorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_uvicorn/conftest.py` & `newrelic-9.9.1/tests/adapter_uvicorn/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_uvicorn/test_uvicorn.py` & `newrelic-9.9.1/tests/adapter_uvicorn/test_uvicorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_waitress/_application.py` & `newrelic-9.9.1/tests/adapter_waitress/_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_waitress/conftest.py` & `newrelic-9.9.1/tests/adapter_waitress/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/adapter_waitress/test_wsgi.py` & `newrelic-9.9.1/tests/adapter_waitress/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/_test_async_coroutine_trace.py` & `newrelic-9.9.1/tests/agent_features/_test_async_coroutine_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/_test_async_coroutine_transaction.py` & `newrelic-9.9.1/tests/agent_features/_test_async_coroutine_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/_test_async_generator_trace.py` & `newrelic-9.9.1/tests/agent_features/_test_async_generator_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/_test_code_level_metrics.py` & `newrelic-9.9.1/tests/agent_features/_test_code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/conftest.py` & `newrelic-9.9.1/tests/agent_features/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_apdex_metrics.py` & `newrelic-9.9.1/tests/agent_features/test_apdex_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_asgi_browser.py` & `newrelic-9.9.1/tests/agent_features/test_asgi_browser.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_asgi_distributed_tracing.py` & `newrelic-9.9.1/tests/agent_features/test_asgi_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_asgi_transaction.py` & `newrelic-9.9.1/tests/agent_features/test_asgi_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_asgi_w3c_trace_context.py` & `newrelic-9.9.1/tests/agent_features/test_asgi_w3c_trace_context.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_async_context_propagation.py` & `newrelic-9.9.1/tests/agent_features/test_async_context_propagation.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_async_generator_trace.py` & `newrelic-9.9.1/tests/agent_features/test_async_generator_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_async_timing.py` & `newrelic-9.9.1/tests/agent_features/test_async_timing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_async_wrapper_detection.py` & `newrelic-9.9.1/tests/agent_features/test_async_wrapper_detection.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_attribute.py` & `newrelic-9.9.1/tests/agent_features/test_attribute.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_attributes_in_action.py` & `newrelic-9.9.1/tests/agent_features/test_attributes_in_action.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_background_task.py` & `newrelic-9.9.1/tests/agent_features/test_background_task.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_browser.py` & `newrelic-9.9.1/tests/agent_features/test_browser.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_browser_middleware.py` & `newrelic-9.9.1/tests/agent_features/test_browser_middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_cat.py` & `newrelic-9.9.1/tests/agent_features/test_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_code_level_metrics.py` & `newrelic-9.9.1/tests/agent_features/test_code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_collector_payloads.py` & `newrelic-9.9.1/tests/agent_features/test_collector_payloads.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_configuration.py` & `newrelic-9.9.1/tests/agent_features/test_configuration.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_coroutine_trace.py` & `newrelic-9.9.1/tests/agent_features/test_coroutine_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_coroutine_transaction.py` & `newrelic-9.9.1/tests/agent_features/test_coroutine_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_custom_events.py` & `newrelic-9.9.1/tests/agent_features/test_custom_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_custom_metrics.py` & `newrelic-9.9.1/tests/agent_features/test_custom_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_datastore_trace.py` & `newrelic-9.9.1/tests/agent_features/test_datastore_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_dead_transactions.py` & `newrelic-9.9.1/tests/agent_features/test_dead_transactions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_dimensional_metrics.py` & `newrelic-9.9.1/tests/agent_features/test_dimensional_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_distributed_tracing.py` & `newrelic-9.9.1/tests/agent_features/test_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_error_events.py` & `newrelic-9.9.1/tests/agent_features/test_error_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_error_group_callback.py` & `newrelic-9.9.1/tests/agent_features/test_error_group_callback.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_event_loop_wait_time.py` & `newrelic-9.9.1/tests/agent_features/test_event_loop_wait_time.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_exception_messages.py` & `newrelic-9.9.1/tests/agent_features/test_exception_messages.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_function_trace.py` & `newrelic-9.9.1/tests/agent_features/test_function_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_high_security_mode.py` & `newrelic-9.9.1/tests/agent_features/test_high_security_mode.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_ignore_expected_errors.py` & `newrelic-9.9.1/tests/agent_features/test_ignore_expected_errors.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_lambda_handler.py` & `newrelic-9.9.1/tests/agent_features/test_lambda_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_llm_token_count_callback.py` & `newrelic-9.9.1/tests/agent_features/test_llm_token_count_callback.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_log_events.py` & `newrelic-9.9.1/tests/agent_features/test_log_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_logs_in_context.py` & `newrelic-9.9.1/tests/agent_features/test_logs_in_context.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_metric_normalization.py` & `newrelic-9.9.1/tests/agent_features/test_metric_normalization.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_ml_events.py` & `newrelic-9.9.1/tests/agent_features/test_ml_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_notice_error.py` & `newrelic-9.9.1/tests/agent_features/test_notice_error.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_priority_sampling.py` & `newrelic-9.9.1/tests/agent_features/test_priority_sampling.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_profile_trace.py` & `newrelic-9.9.1/tests/agent_features/test_profile_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_record_llm_feedback_event.py` & `newrelic-9.9.1/tests/agent_features/test_record_llm_feedback_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_serverless_mode.py` & `newrelic-9.9.1/tests/agent_features/test_serverless_mode.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_span_events.py` & `newrelic-9.9.1/tests/agent_features/test_span_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_stack_trace.py` & `newrelic-9.9.1/tests/agent_features/test_stack_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_supportability_metrics.py` & `newrelic-9.9.1/tests/agent_features/test_supportability_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_synthetics.py` & `newrelic-9.9.1/tests/agent_features/test_synthetics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_time_trace.py` & `newrelic-9.9.1/tests/agent_features/test_time_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py` & `newrelic-9.9.1/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_transaction_name.py` & `newrelic-9.9.1/tests/agent_features/test_transaction_name.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_transaction_trace_segments.py` & `newrelic-9.9.1/tests/agent_features/test_transaction_trace_segments.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_w3c_trace_context.py` & `newrelic-9.9.1/tests/agent_features/test_w3c_trace_context.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_web_transaction.py` & `newrelic-9.9.1/tests/agent_features/test_web_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_features/test_wsgi_attributes.py` & `newrelic-9.9.1/tests/agent_features/test_wsgi_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_streaming/_test_handler.py` & `newrelic-9.9.1/tests/agent_streaming/_test_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_streaming/conftest.py` & `newrelic-9.9.1/tests/agent_streaming/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_streaming/test_infinite_tracing.py` & `newrelic-9.9.1/tests/agent_streaming/test_infinite_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_streaming/test_span_events.py` & `newrelic-9.9.1/tests/agent_streaming/test_span_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_streaming/test_stream_buffer.py` & `newrelic-9.9.1/tests/agent_streaming/test_stream_buffer.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_streaming/test_streaming_rpc.py` & `newrelic-9.9.1/tests/agent_streaming/test_streaming_rpc.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/_test_import_hook.py` & `newrelic-9.9.1/tests/agent_unittests/_test_import_hook.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/cert.pem` & `newrelic-9.9.1/tests/agent_unittests/cert.pem`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/conftest.py` & `newrelic-9.9.1/tests/agent_unittests/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_agent.py` & `newrelic-9.9.1/tests/agent_unittests/test_agent.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_agent_connect.py` & `newrelic-9.9.1/tests/agent_unittests/test_agent_connect.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_agent_protocol.py` & `newrelic-9.9.1/tests/agent_unittests/test_agent_protocol.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_check_environment.py` & `newrelic-9.9.1/tests/agent_unittests/test_check_environment.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_connect_response_fields.py` & `newrelic-9.9.1/tests/agent_unittests/test_connect_response_fields.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_distributed_tracing_settings.py` & `newrelic-9.9.1/tests/agent_unittests/test_distributed_tracing_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_encoding_utils.py` & `newrelic-9.9.1/tests/agent_unittests/test_encoding_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_environment.py` & `newrelic-9.9.1/tests/agent_unittests/test_environment.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_full_uri_payloads.py` & `newrelic-9.9.1/tests/agent_unittests/test_full_uri_payloads.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_harvest_loop.py` & `newrelic-9.9.1/tests/agent_unittests/test_harvest_loop.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_http_client.py` & `newrelic-9.9.1/tests/agent_unittests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_import_hook.py` & `newrelic-9.9.1/tests/agent_unittests/test_import_hook.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_infinite_trace_settings.py` & `newrelic-9.9.1/tests/agent_unittests/test_infinite_trace_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_package_version_utils.py` & `newrelic-9.9.1/tests/agent_unittests/test_package_version_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_region_aware_settings.py` & `newrelic-9.9.1/tests/agent_unittests/test_region_aware_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_sampler_metrics.py` & `newrelic-9.9.1/tests/agent_unittests/test_sampler_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_serverless_mode_settings.py` & `newrelic-9.9.1/tests/agent_unittests/test_serverless_mode_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_signature.py` & `newrelic-9.9.1/tests/agent_unittests/test_signature.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_trace_cache.py` & `newrelic-9.9.1/tests/agent_unittests/test_trace_cache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_utilization_settings.py` & `newrelic-9.9.1/tests/agent_unittests/test_utilization_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/agent_unittests/test_wrappers.py` & `newrelic-9.9.1/tests/agent_unittests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/application_celery/_target_application.py` & `newrelic-9.9.1/tests/application_celery/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/application_celery/conftest.py` & `newrelic-9.9.1/tests/application_celery/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/application_celery/test_application.py` & `newrelic-9.9.1/tests/application_celery/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/application_celery/test_distributed_tracing.py` & `newrelic-9.9.1/tests/application_celery/test_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/application_celery/test_max_tasks_per_child.py` & `newrelic-9.9.1/tests/application_celery/test_max_tasks_per_child.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/application_celery/test_task_methods.py` & `newrelic-9.9.1/tests/application_celery/test_task_methods.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,47 +8,50 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import pytest
 
 from _target_application import add, tsum
-from celery import chain, chord, group
+from testing_support.validators.validate_code_level_metrics import (
+    validate_code_level_metrics,
+)
 from testing_support.validators.validate_transaction_count import (
     validate_transaction_count,
 )
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
 )
 
-FORGONE_TASK_METRICS = [("Function/_target_application.add", None), ("Function/_target_application.tsum", None)]
+import celery
 
 
-def test_task_wrapping_detection():
-    """
-    Ensure celery detects our monkeypatching properly and will run our instrumentation
-    on __call__ and runs that instead of micro-optimizing it away to a run() call.
+FORGONE_TASK_METRICS = [("Function/_target_application.add", None), ("Function/_target_application.tsum", None)]
 
-    If this is not working, most other tests in this file will fail as the different ways
-    of running celery tasks will not all run our instrumentation.
-    """
-    from celery.app.trace import task_has_custom
 
-    assert task_has_custom(add, "__call__")
+@pytest.fixture(scope="module", autouse=True, params=[False, True], ids=["unpatched", "patched"])
+def with_worker_optimizations(request, celery_worker_available):
+    if request.param:
+        celery.app.trace.setup_worker_optimizations(celery_worker_available.app)
+
+    yield request.param
+    celery.app.trace.reset_worker_optimizations()
 
 
 @validate_transaction_metrics(
     name="_target_application.add",
     group="Celery",
     scoped_metrics=FORGONE_TASK_METRICS,
     rollup_metrics=FORGONE_TASK_METRICS,
     background_task=True,
 )
+@validate_code_level_metrics("_target_application", "add")
 @validate_transaction_count(1)
 def test_celery_task_call():
     """
     Executes task in local process and returns the result directly.
     """
     result = add(3, 4)
     assert result == 7
@@ -57,14 +60,15 @@
 @validate_transaction_metrics(
     name="_target_application.add",
     group="Celery",
     scoped_metrics=FORGONE_TASK_METRICS,
     rollup_metrics=FORGONE_TASK_METRICS,
     background_task=True,
 )
+@validate_code_level_metrics("_target_application", "add")
 @validate_transaction_count(1)
 def test_celery_task_apply():
     """
     Executes task in local process and returns an EagerResult.
     """
     result = add.apply((3, 4))
     result = result.get()
@@ -74,14 +78,15 @@
 @validate_transaction_metrics(
     name="_target_application.add",
     group="Celery",
     scoped_metrics=FORGONE_TASK_METRICS,
     rollup_metrics=FORGONE_TASK_METRICS,
     background_task=True,
 )
+@validate_code_level_metrics("_target_application", "add")
 @validate_transaction_count(1)
 def test_celery_task_delay():
     """
     Executes task on worker process and returns an AsyncResult.
     """
     result = add.delay(3, 4)
     result = result.get()
@@ -91,14 +96,15 @@
 @validate_transaction_metrics(
     name="_target_application.add",
     group="Celery",
     scoped_metrics=FORGONE_TASK_METRICS,
     rollup_metrics=FORGONE_TASK_METRICS,
     background_task=True,
 )
+@validate_code_level_metrics("_target_application", "add")
 @validate_transaction_count(1)
 def test_celery_task_apply_async():
     """
     Executes task on worker process and returns an AsyncResult.
     """
     result = add.apply_async((3, 4))
     result = result.get()
@@ -108,14 +114,15 @@
 @validate_transaction_metrics(
     name="_target_application.add",
     group="Celery",
     scoped_metrics=FORGONE_TASK_METRICS,
     rollup_metrics=FORGONE_TASK_METRICS,
     background_task=True,
 )
+@validate_code_level_metrics("_target_application", "add")
 @validate_transaction_count(1)
 def test_celery_app_send_task(celery_session_app):
     """
     Executes task on worker process and returns an AsyncResult.
     """
     result = celery_session_app.send_task("_target_application.add", (3, 4))
     result = result.get()
@@ -125,14 +132,15 @@
 @validate_transaction_metrics(
     name="_target_application.add",
     group="Celery",
     scoped_metrics=FORGONE_TASK_METRICS,
     rollup_metrics=FORGONE_TASK_METRICS,
     background_task=True,
 )
+@validate_code_level_metrics("_target_application", "add")
 @validate_transaction_count(1)
 def test_celery_task_signature():
     """
     Executes task on worker process and returns an AsyncResult.
     """
     result = add.s(3, 4).delay()
     result = result.get()
@@ -150,14 +158,16 @@
     name="_target_application.add",
     group="Celery",
     scoped_metrics=FORGONE_TASK_METRICS,
     rollup_metrics=FORGONE_TASK_METRICS,
     background_task=True,
     index=-2,
 )
+@validate_code_level_metrics("_target_application", "add")
+@validate_code_level_metrics("_target_application", "add", index=-2)
 @validate_transaction_count(2)
 def test_celery_task_link():
     """
     Executes multiple tasks on worker process and returns an AsyncResult.
     """
     result = add.apply_async((3, 4), link=[add.s(5)])
     result = result.get()
@@ -175,20 +185,22 @@
     name="_target_application.add",
     group="Celery",
     scoped_metrics=FORGONE_TASK_METRICS,
     rollup_metrics=FORGONE_TASK_METRICS,
     background_task=True,
     index=-2,
 )
+@validate_code_level_metrics("_target_application", "add")
+@validate_code_level_metrics("_target_application", "add", index=-2)
 @validate_transaction_count(2)
 def test_celery_chain():
     """
     Executes multiple tasks on worker process and returns an AsyncResult.
     """
-    result = chain(add.s(3, 4), add.s(5))()
+    result = celery.chain(add.s(3, 4), add.s(5))()
 
     result = result.get()
     assert result == 12
 
 
 @validate_transaction_metrics(
     name="_target_application.add",
@@ -201,20 +213,22 @@
     name="_target_application.add",
     group="Celery",
     scoped_metrics=FORGONE_TASK_METRICS,
     rollup_metrics=FORGONE_TASK_METRICS,
     background_task=True,
     index=-2,
 )
+@validate_code_level_metrics("_target_application", "add")
+@validate_code_level_metrics("_target_application", "add", index=-2)
 @validate_transaction_count(2)
 def test_celery_group():
     """
     Executes multiple tasks on worker process and returns an AsyncResult.
     """
-    result = group(add.s(3, 4), add.s(1, 2))()
+    result = celery.group(add.s(3, 4), add.s(1, 2))()
     result = result.get()
     assert result == [7, 3]
 
 
 @validate_transaction_metrics(
     name="_target_application.tsum",
     group="Celery",
@@ -234,31 +248,35 @@
     name="_target_application.add",
     group="Celery",
     scoped_metrics=FORGONE_TASK_METRICS,
     rollup_metrics=FORGONE_TASK_METRICS,
     background_task=True,
     index=-3,
 )
+@validate_code_level_metrics("_target_application", "tsum")
+@validate_code_level_metrics("_target_application", "add", index=-2)
+@validate_code_level_metrics("_target_application", "add", index=-3)
 @validate_transaction_count(3)
 def test_celery_chord():
     """
     Executes 2 add tasks, followed by a tsum task on the worker process and returns an AsyncResult.
     """
-    result = chord([add.s(3, 4), add.s(1, 2)])(tsum.s())
+    result = celery.chord([add.s(3, 4), add.s(1, 2)])(tsum.s())
     result = result.get()
     assert result == 10
 
 
 @validate_transaction_metrics(
     name="celery.map/_target_application.tsum",
     group="Celery",
     scoped_metrics=[("Function/_target_application.tsum", 2)],
     rollup_metrics=[("Function/_target_application.tsum", 2)],
     background_task=True,
 )
+@validate_code_level_metrics("_target_application", "tsum", count=3)
 @validate_transaction_count(1)
 def test_celery_task_map():
     """
     Executes map task on worker process with original task as a subtask and returns an AsyncResult.
     """
     result = tsum.map([(3, 4), (1, 2)]).apply()
     result = result.get()
@@ -268,14 +286,15 @@
 @validate_transaction_metrics(
     name="celery.starmap/_target_application.add",
     group="Celery",
     scoped_metrics=[("Function/_target_application.add", 2)],
     rollup_metrics=[("Function/_target_application.add", 2)],
     background_task=True,
 )
+@validate_code_level_metrics("_target_application", "add", count=3)
 @validate_transaction_count(1)
 def test_celery_task_starmap():
     """
     Executes starmap task on worker process with original task as a subtask and returns an AsyncResult.
     """
     result = add.starmap([(3, 4), (1, 2)]).apply_async()
     result = result.get()
@@ -293,14 +312,16 @@
     name="celery.starmap/_target_application.add",
     group="Celery",
     scoped_metrics=[("Function/_target_application.add", 1)],
     rollup_metrics=[("Function/_target_application.add", 1)],
     background_task=True,
     index=-2,
 )
+@validate_code_level_metrics("_target_application", "add", count=2)
+@validate_code_level_metrics("_target_application", "add", count=2, index=-2)
 @validate_transaction_count(2)
 def test_celery_task_chunks():
     """
     Executes multiple tasks on worker process and returns an AsyncResult.
     """
     result = add.chunks([(3, 4), (1, 2)], n=1).apply_async()
     result = result.get()
```

### Comparing `newrelic-9.9.0/tests/application_gearman/conftest.py` & `newrelic-9.9.1/tests/application_gearman/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/application_gearman/test_gearman.py` & `newrelic-9.9.1/tests/application_gearman/test_gearman.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_djangorestframework/conftest.py` & `newrelic-9.9.1/tests/component_djangorestframework/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_djangorestframework/settings.py` & `newrelic-9.9.1/tests/component_djangorestframework/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_djangorestframework/test_application.py` & `newrelic-9.9.1/tests/component_djangorestframework/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_djangorestframework/urls.py` & `newrelic-9.9.1/tests/component_djangorestframework/urls.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_djangorestframework/views.py` & `newrelic-9.9.1/tests/component_djangorestframework/views.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_djangorestframework/wsgi.py` & `newrelic-9.9.1/tests/component_djangorestframework/wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_flask_rest/_test_application.py` & `newrelic-9.9.1/tests/component_flask_rest/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_flask_rest/conftest.py` & `newrelic-9.9.1/tests/component_flask_rest/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_flask_rest/test_application.py` & `newrelic-9.9.1/tests/component_flask_rest/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_graphqlserver/__init__.py` & `newrelic-9.9.1/tests/component_graphqlserver/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_graphqlserver/_target_schema_async.py` & `newrelic-9.9.1/tests/component_graphqlserver/_target_schema_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_graphqlserver/_test_graphql.py` & `newrelic-9.9.1/tests/component_graphqlserver/_test_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_graphqlserver/conftest.py` & `newrelic-9.9.1/tests/component_graphqlserver/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_graphqlserver/test_graphql.py` & `newrelic-9.9.1/tests/component_graphqlserver/test_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_tastypie/api.py` & `newrelic-9.9.1/tests/component_tastypie/api.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_tastypie/conftest.py` & `newrelic-9.9.1/tests/component_tastypie/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_tastypie/settings.py` & `newrelic-9.9.1/tests/component_tastypie/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_tastypie/test_application.py` & `newrelic-9.9.1/tests/component_tastypie/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_tastypie/urls.py` & `newrelic-9.9.1/tests/component_tastypie/urls.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_tastypie/views.py` & `newrelic-9.9.1/tests/component_tastypie/views.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/component_tastypie/wsgi.py` & `newrelic-9.9.1/tests/component_tastypie/wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/coroutines_asyncio/conftest.py` & `newrelic-9.9.1/tests/coroutines_asyncio/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/coroutines_asyncio/test_context_propagation.py` & `newrelic-9.9.1/tests/coroutines_asyncio/test_context_propagation.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/conftest.py` & `newrelic-9.9.1/tests/cross_agent/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/README.md` & `newrelic-9.9.1/tests/cross_agent/fixtures/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/attribute_configuration.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/attribute_configuration.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/cat_map.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/cat_map.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/collector_hostname.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/collector_hostname.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/datastores/README.md` & `newrelic-9.9.1/tests/cross_agent/fixtures/datastores/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/datastores/datastore_instances.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/datastores/datastore_instances.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/distributed_tracing/README.md` & `newrelic-9.9.1/tests/cross_agent/fixtures/distributed_tracing/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/distributed_tracing/trace_context.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/distributed_tracing/trace_context.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/cases.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/cases.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/cases.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id_v2/cases.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-20.10.16.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id_v2/docker-20.10.16.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-24.0.2.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id_v2/docker-24.0.2.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-too-long.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id_v2/docker-too-long.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/invalid-characters.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id_v2/invalid-characters.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/invalid-length.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/docker_container_id_v2/invalid-length.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/labels.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/labels.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/codecommit.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/codecommit.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/kinesis.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/s3_put.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/s3_put.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/ses.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/ses.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/sns.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/sns.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/sqs.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source/sqs.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/lambda_event_source.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md` & `newrelic-9.9.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/README.md` & `newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt` & `newrelic-9.9.1/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rules.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/rules.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_cookie.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_cookie.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html` & `newrelic-9.9.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/README.md` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/sql_parsing.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/sql_parsing.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/transaction_segment_terms.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/transaction_segment_terms.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/url_clean.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/url_clean.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/url_domain_extraction.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/url_domain_extraction.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/utilization/README.md` & `newrelic-9.9.1/tests/cross_agent/fixtures/utilization/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/utilization/boot_id.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/utilization/boot_id.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/utilization/utilization_json.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/utilization/utilization_json.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/README.md` & `newrelic-9.9.1/tests/cross_agent/fixtures/utilization_vendor_specific/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json` & `newrelic-9.9.1/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_agent_attributes.py` & `newrelic-9.9.1/tests/cross_agent/test_agent_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_aws_utilization_data.py` & `newrelic-9.9.1/tests/cross_agent/test_aws_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_azure_utilization_data.py` & `newrelic-9.9.1/tests/cross_agent/test_azure_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_boot_id_utilization_data.py` & `newrelic-9.9.1/tests/cross_agent/test_boot_id_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_cat_map.py` & `newrelic-9.9.1/tests/cross_agent/test_cat_map.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_collector_hostname.py` & `newrelic-9.9.1/tests/cross_agent/test_collector_hostname.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_datastore_instance.py` & `newrelic-9.9.1/tests/cross_agent/test_datastore_instance.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_distributed_tracing.py` & `newrelic-9.9.1/tests/cross_agent/test_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_docker_container_id.py` & `newrelic-9.9.1/tests/cross_agent/test_docker_container_id.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_docker_container_id_v2.py` & `newrelic-9.9.1/tests/cross_agent/test_docker_container_id_v2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_gcp_utilization_data.py` & `newrelic-9.9.1/tests/cross_agent/test_gcp_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_labels_and_rollups.py` & `newrelic-9.9.1/tests/cross_agent/test_labels_and_rollups.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_lambda_event_source.py` & `newrelic-9.9.1/tests/cross_agent/test_lambda_event_source.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_pcf_utilization_data.py` & `newrelic-9.9.1/tests/cross_agent/test_pcf_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_rules.py` & `newrelic-9.9.1/tests/cross_agent/test_rules.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_sql_obfuscation.py` & `newrelic-9.9.1/tests/cross_agent/test_sql_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_system_info.py` & `newrelic-9.9.1/tests/cross_agent/test_system_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_transaction_segment_terms.py` & `newrelic-9.9.1/tests/cross_agent/test_transaction_segment_terms.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_utilization_configs.py` & `newrelic-9.9.1/tests/cross_agent/test_utilization_configs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/cross_agent/test_w3c_trace_context.py` & `newrelic-9.9.1/tests/cross_agent/test_w3c_trace_context.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aioredis/conftest.py` & `newrelic-9.9.1/tests/datastore_aioredis/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aioredis/test_custom_conn_pool.py` & `newrelic-9.9.1/tests/datastore_aioredis/test_custom_conn_pool.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aioredis/test_execute_command.py` & `newrelic-9.9.1/tests/datastore_aioredis/test_execute_command.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aioredis/test_get_and_set.py` & `newrelic-9.9.1/tests/datastore_aioredis/test_get_and_set.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aioredis/test_instance_info.py` & `newrelic-9.9.1/tests/datastore_aioredis/test_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aioredis/test_multiple_dbs.py` & `newrelic-9.9.1/tests/datastore_aioredis/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aioredis/test_span_event.py` & `newrelic-9.9.1/tests/datastore_aioredis/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aioredis/test_trace_node.py` & `newrelic-9.9.1/tests/datastore_aioredis/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aioredis/test_transactions.py` & `newrelic-9.9.1/tests/datastore_aioredis/test_transactions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aioredis/test_uninstrumented_methods.py` & `newrelic-9.9.1/tests/datastore_aioredis/test_uninstrumented_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aredis/conftest.py` & `newrelic-9.9.1/tests/datastore_aredis/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aredis/test_custom_conn_pool.py` & `newrelic-9.9.1/tests/datastore_aredis/test_custom_conn_pool.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aredis/test_execute_command.py` & `newrelic-9.9.1/tests/datastore_aredis/test_execute_command.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aredis/test_get_and_set.py` & `newrelic-9.9.1/tests/datastore_aredis/test_get_and_set.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aredis/test_instance_info.py` & `newrelic-9.9.1/tests/datastore_aredis/test_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aredis/test_multiple_dbs.py` & `newrelic-9.9.1/tests/datastore_aredis/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aredis/test_span_event.py` & `newrelic-9.9.1/tests/datastore_aredis/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aredis/test_trace_node.py` & `newrelic-9.9.1/tests/datastore_aredis/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_aredis/test_uninstrumented_methods.py` & `newrelic-9.9.1/tests/datastore_aredis/test_uninstrumented_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_asyncpg/conftest.py` & `newrelic-9.9.1/tests/datastore_asyncpg/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_asyncpg/test_multiple_dbs.py` & `newrelic-9.9.1/tests/datastore_asyncpg/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_asyncpg/test_query.py` & `newrelic-9.9.1/tests/datastore_asyncpg/test_query.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_bmemcached/conftest.py` & `newrelic-9.9.1/tests/datastore_bmemcached/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_bmemcached/test_memcache.py` & `newrelic-9.9.1/tests/datastore_bmemcached/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_elasticsearch/conftest.py` & `newrelic-9.9.1/tests/datastore_elasticsearch/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_elasticsearch/test_connection.py` & `newrelic-9.9.1/tests/datastore_elasticsearch/test_connection.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_elasticsearch/test_database_duration.py` & `newrelic-9.9.1/tests/datastore_elasticsearch/test_database_duration.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_elasticsearch/test_elasticsearch.py` & `newrelic-9.9.1/tests/datastore_elasticsearch/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_elasticsearch/test_instrumented_methods.py` & `newrelic-9.9.1/tests/datastore_elasticsearch/test_instrumented_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_elasticsearch/test_mget.py` & `newrelic-9.9.1/tests/datastore_elasticsearch/test_mget.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_elasticsearch/test_multiple_dbs.py` & `newrelic-9.9.1/tests/datastore_elasticsearch/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_elasticsearch/test_trace_node.py` & `newrelic-9.9.1/tests/datastore_elasticsearch/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_elasticsearch/test_transport.py` & `newrelic-9.9.1/tests/datastore_elasticsearch/test_transport.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_firestore/conftest.py` & `newrelic-9.9.1/tests/datastore_firestore/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_firestore/test_async_batching.py` & `newrelic-9.9.1/tests/datastore_firestore/test_async_batching.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_firestore/test_async_client.py` & `newrelic-9.9.1/tests/datastore_firestore/test_async_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_firestore/test_async_collections.py` & `newrelic-9.9.1/tests/datastore_firestore/test_async_collections.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_firestore/test_async_documents.py` & `newrelic-9.9.1/tests/datastore_firestore/test_async_documents.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_firestore/test_async_query.py` & `newrelic-9.9.1/tests/datastore_firestore/test_async_query.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_firestore/test_async_transaction.py` & `newrelic-9.9.1/tests/datastore_firestore/test_async_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_firestore/test_batching.py` & `newrelic-9.9.1/tests/datastore_firestore/test_batching.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_firestore/test_client.py` & `newrelic-9.9.1/tests/datastore_firestore/test_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_firestore/test_collections.py` & `newrelic-9.9.1/tests/datastore_firestore/test_collections.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_firestore/test_documents.py` & `newrelic-9.9.1/tests/datastore_firestore/test_documents.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_firestore/test_query.py` & `newrelic-9.9.1/tests/datastore_firestore/test_query.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_firestore/test_transaction.py` & `newrelic-9.9.1/tests/datastore_firestore/test_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_memcache/conftest.py` & `newrelic-9.9.1/tests/datastore_memcache/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_memcache/test_all_methods_wrapped.py` & `newrelic-9.9.1/tests/datastore_memcache/test_all_methods_wrapped.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_memcache/test_memcache.py` & `newrelic-9.9.1/tests/datastore_memcache/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_memcache/test_multiple_dbs.py` & `newrelic-9.9.1/tests/datastore_memcache/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_memcache/test_span_event.py` & `newrelic-9.9.1/tests/datastore_memcache/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_mysql/conftest.py` & `newrelic-9.9.1/tests/datastore_mysql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_mysql/test_database.py` & `newrelic-9.9.1/tests/datastore_mysql/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_postgresql/conftest.py` & `newrelic-9.9.1/tests/datastore_postgresql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_postgresql/test_database.py` & `newrelic-9.9.1/tests/datastore_postgresql/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2/conftest.py` & `newrelic-9.9.1/tests/datastore_psycopg2/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2/test_as_string.py` & `newrelic-9.9.1/tests/datastore_psycopg2/test_as_string.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2/test_async.py` & `newrelic-9.9.1/tests/datastore_psycopg2/test_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2/test_cursor.py` & `newrelic-9.9.1/tests/datastore_psycopg2/test_cursor.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2/test_database_instance_info.py` & `newrelic-9.9.1/tests/datastore_psycopg2/test_database_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2/test_explain_plans.py` & `newrelic-9.9.1/tests/datastore_psycopg2/test_explain_plans.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2/test_forward_compat.py` & `newrelic-9.9.1/tests/datastore_psycopg2/test_forward_compat.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2/test_multiple_dbs.py` & `newrelic-9.9.1/tests/datastore_psycopg2/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2/test_obfuscation.py` & `newrelic-9.9.1/tests/datastore_psycopg2/test_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2/test_register.py` & `newrelic-9.9.1/tests/datastore_psycopg2/test_register.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2/test_rollback.py` & `newrelic-9.9.1/tests/datastore_psycopg2/test_rollback.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2/test_slow_sql.py` & `newrelic-9.9.1/tests/datastore_psycopg2/test_slow_sql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2/test_span_event.py` & `newrelic-9.9.1/tests/datastore_psycopg2/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2/test_trace_node.py` & `newrelic-9.9.1/tests/datastore_psycopg2/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2/utils.py` & `newrelic-9.9.1/tests/datastore_psycopg2/utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2cffi/conftest.py` & `newrelic-9.9.1/tests/datastore_psycopg2cffi/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2cffi/test_database.py` & `newrelic-9.9.1/tests/datastore_psycopg2cffi/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_psycopg2cffi/test_explain_plans.py` & `newrelic-9.9.1/tests/datastore_psycopg2cffi/test_explain_plans.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_pylibmc/conftest.py` & `newrelic-9.9.1/tests/datastore_pylibmc/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_pylibmc/test_memcache.py` & `newrelic-9.9.1/tests/datastore_pylibmc/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_pymemcache/conftest.py` & `newrelic-9.9.1/tests/datastore_pymemcache/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_pymemcache/test_memcache.py` & `newrelic-9.9.1/tests/datastore_pymemcache/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_pymongo/conftest.py` & `newrelic-9.9.1/tests/datastore_pymongo/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_pymongo/test_pymongo.py` & `newrelic-9.9.1/tests/datastore_pymongo/test_pymongo.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_pymssql/conftest.py` & `newrelic-9.9.1/tests/datastore_pymssql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_pymssql/test_database.py` & `newrelic-9.9.1/tests/datastore_pymssql/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_pymysql/conftest.py` & `newrelic-9.9.1/tests/datastore_pymysql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_pymysql/test_database.py` & `newrelic-9.9.1/tests/datastore_pymysql/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_pyodbc/conftest.py` & `newrelic-9.9.1/tests/datastore_pyodbc/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_pyodbc/test_pyodbc.py` & `newrelic-9.9.1/tests/datastore_pyodbc/test_pyodbc.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_pysolr/conftest.py` & `newrelic-9.9.1/tests/datastore_pysolr/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_pysolr/test_solr.py` & `newrelic-9.9.1/tests/datastore_pysolr/test_solr.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_redis/conftest.py` & `newrelic-9.9.1/tests/datastore_redis/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_redis/test_asyncio.py` & `newrelic-9.9.1/tests/datastore_redis/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_redis/test_custom_conn_pool.py` & `newrelic-9.9.1/tests/datastore_redis/test_custom_conn_pool.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_redis/test_execute_command.py` & `newrelic-9.9.1/tests/datastore_redis/test_execute_command.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_redis/test_generators.py` & `newrelic-9.9.1/tests/datastore_redis/test_generators.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_redis/test_get_and_set.py` & `newrelic-9.9.1/tests/datastore_redis/test_get_and_set.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_redis/test_instance_info.py` & `newrelic-9.9.1/tests/datastore_redis/test_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_redis/test_multiple_dbs.py` & `newrelic-9.9.1/tests/datastore_redis/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_redis/test_rb.py` & `newrelic-9.9.1/tests/datastore_redis/test_rb.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_redis/test_span_event.py` & `newrelic-9.9.1/tests/datastore_redis/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_redis/test_trace_node.py` & `newrelic-9.9.1/tests/datastore_redis/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_redis/test_uninstrumented_methods.py` & `newrelic-9.9.1/tests/datastore_redis/test_uninstrumented_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_rediscluster/conftest.py` & `newrelic-9.9.1/tests/datastore_rediscluster/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_rediscluster/test_uninstrumented_rediscluster_methods.py` & `newrelic-9.9.1/tests/datastore_rediscluster/test_uninstrumented_rediscluster_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_solrpy/conftest.py` & `newrelic-9.9.1/tests/datastore_solrpy/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_solrpy/test_solr.py` & `newrelic-9.9.1/tests/datastore_solrpy/test_solr.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_sqlite/conftest.py` & `newrelic-9.9.1/tests/datastore_sqlite/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_sqlite/test_database.py` & `newrelic-9.9.1/tests/datastore_sqlite/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/datastore_sqlite/test_obfuscation.py` & `newrelic-9.9.1/tests/datastore_sqlite/test_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_botocore/_mock_bedrock_encoding_utils.py` & `newrelic-9.9.1/tests/external_botocore/_mock_bedrock_encoding_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_botocore/_mock_external_bedrock_server.py` & `newrelic-9.9.1/tests/external_botocore/_mock_external_bedrock_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_botocore/_test_bedrock_chat_completion.py` & `newrelic-9.9.1/tests/external_botocore/_test_bedrock_chat_completion.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_botocore/_test_bedrock_embeddings.py` & `newrelic-9.9.1/tests/external_botocore/_test_bedrock_embeddings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_botocore/conftest.py` & `newrelic-9.9.1/tests/external_botocore/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_botocore/test_bedrock_chat_completion.py` & `newrelic-9.9.1/tests/external_botocore/test_bedrock_chat_completion.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_botocore/test_bedrock_chat_completion_via_langchain.py` & `newrelic-9.9.1/tests/external_botocore/test_bedrock_chat_completion_via_langchain.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_botocore/test_bedrock_embeddings.py` & `newrelic-9.9.1/tests/external_botocore/test_bedrock_embeddings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_botocore/test_boto3_iam.py` & `newrelic-9.9.1/tests/external_botocore/test_boto3_iam.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_botocore/test_boto3_s3.py` & `newrelic-9.9.1/tests/external_botocore/test_boto3_s3.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_botocore/test_boto3_sns.py` & `newrelic-9.9.1/tests/external_botocore/test_boto3_sns.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_botocore/test_botocore_dynamodb.py` & `newrelic-9.9.1/tests/external_botocore/test_botocore_dynamodb.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_botocore/test_botocore_ec2.py` & `newrelic-9.9.1/tests/external_botocore/test_botocore_ec2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_botocore/test_botocore_s3.py` & `newrelic-9.9.1/tests/external_botocore/test_botocore_s3.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_botocore/test_botocore_sqs.py` & `newrelic-9.9.1/tests/external_botocore/test_botocore_sqs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_feedparser/conftest.py` & `newrelic-9.9.1/tests/external_feedparser/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_feedparser/packages.xml` & `newrelic-9.9.1/tests/external_feedparser/packages.xml`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_feedparser/test_feedparser.py` & `newrelic-9.9.1/tests/external_feedparser/test_feedparser.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_http/conftest.py` & `newrelic-9.9.1/tests/external_http/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_http/test_http.py` & `newrelic-9.9.1/tests/external_http/test_http.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_httplib/conftest.py` & `newrelic-9.9.1/tests/external_httplib/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_httplib/test_httplib.py` & `newrelic-9.9.1/tests/external_httplib/test_httplib.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_httplib/test_urllib.py` & `newrelic-9.9.1/tests/external_httplib/test_urllib.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_httplib/test_urllib2.py` & `newrelic-9.9.1/tests/external_httplib/test_urllib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_httplib2/conftest.py` & `newrelic-9.9.1/tests/external_httplib2/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_httplib2/test_httplib2.py` & `newrelic-9.9.1/tests/external_httplib2/test_httplib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_httpx/conftest.py` & `newrelic-9.9.1/tests/external_httpx/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_httpx/test_client.py` & `newrelic-9.9.1/tests/external_httpx/test_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_requests/conftest.py` & `newrelic-9.9.1/tests/external_requests/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_requests/test_requests.py` & `newrelic-9.9.1/tests/external_requests/test_requests.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_requests/test_span_event.py` & `newrelic-9.9.1/tests/external_requests/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_urllib3/conftest.py` & `newrelic-9.9.1/tests/external_urllib3/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/external_urllib3/test_urllib3.py` & `newrelic-9.9.1/tests/external_urllib3/test_urllib3.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,21 +41,21 @@
 
 from newrelic.api.background_task import background_task
 from newrelic.common.package_version_utils import get_package_version_tuple
 
 
 @pytest.fixture(scope="session")
 def metrics(server):
-    scoped = [("External/localhost:%d/urllib3/" % server.port, 1)]
+    scoped = [("External/localhost:%d/urllib3/GET" % server.port, 1)]
 
     rollup = [
         ("External/all", 1),
         ("External/allOther", 1),
         ("External/localhost:%d/all" % server.port, 1),
-        ("External/localhost:%d/urllib3/" % server.port, 1),
+        ("External/localhost:%d/urllib3/GET" % server.port, 1),
     ]
 
     return scoped, rollup
 
 
 def test_http_request_connection_pool_urlopen(server, metrics):
     @validate_transaction_errors(errors=[])
@@ -158,21 +158,21 @@
         except Exception:
             pass
 
     _test()
 
 
 def test_port_included(server):
-    scoped = [("External/localhost:%d/urllib3/" % server.port, 1)]
+    scoped = [("External/localhost:%d/urllib3/GET" % server.port, 1)]
 
     rollup = [
         ("External/all", 1),
         ("External/allOther", 1),
         ("External/localhost:%d/all" % server.port, 1),
-        ("External/localhost:%d/urllib3/" % server.port, 1),
+        ("External/localhost:%d/urllib3/GET" % server.port, 1),
     ]
 
     @validate_transaction_errors(errors=[])
     @validate_transaction_metrics(
         "test_urllib3:test_port_included", scoped_metrics=scoped, rollup_metrics=rollup, background_task=True
     )
     @background_task(name="test_urllib3:test_port_included")
```

### Comparing `newrelic-9.9.0/tests/framework_aiohttp/_target_application.py` & `newrelic-9.9.1/tests/framework_aiohttp/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_aiohttp/conftest.py` & `newrelic-9.9.1/tests/framework_aiohttp/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_aiohttp/test_client.py` & `newrelic-9.9.1/tests/framework_aiohttp/test_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_aiohttp/test_client_async_await.py` & `newrelic-9.9.1/tests/framework_aiohttp/test_client_async_await.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_aiohttp/test_client_cat.py` & `newrelic-9.9.1/tests/framework_aiohttp/test_client_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_aiohttp/test_externals.py` & `newrelic-9.9.1/tests/framework_aiohttp/test_externals.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_aiohttp/test_middleware.py` & `newrelic-9.9.1/tests/framework_aiohttp/test_middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_aiohttp/test_server.py` & `newrelic-9.9.1/tests/framework_aiohttp/test_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_aiohttp/test_server_cat.py` & `newrelic-9.9.1/tests/framework_aiohttp/test_server_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_aiohttp/test_ws.py` & `newrelic-9.9.1/tests/framework_aiohttp/test_ws.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_ariadne/__init__.py` & `newrelic-9.9.1/tests/framework_ariadne/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_ariadne/_target_application.py` & `newrelic-9.9.1/tests/framework_ariadne/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_ariadne/_target_schema_async.py` & `newrelic-9.9.1/tests/framework_ariadne/_target_schema_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_ariadne/_target_schema_sync.py` & `newrelic-9.9.1/tests/framework_ariadne/_target_schema_sync.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_ariadne/conftest.py` & `newrelic-9.9.1/tests/framework_ariadne/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_ariadne/schema.graphql` & `newrelic-9.9.1/tests/framework_ariadne/schema.graphql`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_ariadne/test_application.py` & `newrelic-9.9.1/tests/framework_ariadne/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_bottle/_target_application.py` & `newrelic-9.9.1/tests/framework_bottle/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_bottle/conftest.py` & `newrelic-9.9.1/tests/framework_bottle/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_bottle/test_application.py` & `newrelic-9.9.1/tests/framework_bottle/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_cherrypy/conftest.py` & `newrelic-9.9.1/tests/framework_cherrypy/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_cherrypy/test_application.py` & `newrelic-9.9.1/tests/framework_cherrypy/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_cherrypy/test_dispatch.py` & `newrelic-9.9.1/tests/framework_cherrypy/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_cherrypy/test_resource.py` & `newrelic-9.9.1/tests/framework_cherrypy/test_resource.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_cherrypy/test_routes.py` & `newrelic-9.9.1/tests/framework_cherrypy/test_routes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_django/_target_application.py` & `newrelic-9.9.1/tests/framework_django/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_django/conftest.py` & `newrelic-9.9.1/tests/framework_django/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_django/dummy_app/__init__.py` & `newrelic-9.9.1/tests/framework_django/dummy_app/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_django/dummy_app/templatetags/__init__.py` & `newrelic-9.9.1/tests/framework_django/dummy_app/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_django/dummy_app/templatetags/custom_tags.py` & `newrelic-9.9.1/tests/framework_django/dummy_app/templatetags/custom_tags.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_django/middleware.py` & `newrelic-9.9.1/tests/framework_django/middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_django/settings.py` & `newrelic-9.9.1/tests/framework_django/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_django/templates/main.html` & `newrelic-9.9.1/tests/framework_django/templates/main.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_django/templates/render_exception.html` & `newrelic-9.9.1/tests/framework_django/templates/render_exception.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_django/templates/results.html` & `newrelic-9.9.1/tests/framework_django/templates/results.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_django/test_application.py` & `newrelic-9.9.1/tests/framework_django/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_django/test_asgi_application.py` & `newrelic-9.9.1/tests/framework_django/test_asgi_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_django/urls.py` & `newrelic-9.9.1/tests/framework_django/urls.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_django/views.py` & `newrelic-9.9.1/tests/framework_django/views.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_django/wsgi.py` & `newrelic-9.9.1/tests/framework_django/wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_falcon/_target_application.py` & `newrelic-9.9.1/tests/framework_falcon/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_falcon/conftest.py` & `newrelic-9.9.1/tests/framework_falcon/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_falcon/test_application.py` & `newrelic-9.9.1/tests/framework_falcon/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_fastapi/_target_application.py` & `newrelic-9.9.1/tests/framework_fastapi/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_fastapi/conftest.py` & `newrelic-9.9.1/tests/framework_fastapi/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_fastapi/test_application.py` & `newrelic-9.9.1/tests/framework_fastapi/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/_test_application.py` & `newrelic-9.9.1/tests/framework_flask/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/_test_application_async.py` & `newrelic-9.9.1/tests/framework_flask/_test_application_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/_test_blueprints.py` & `newrelic-9.9.1/tests/framework_flask/_test_blueprints.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/_test_compress.py` & `newrelic-9.9.1/tests/framework_flask/_test_compress.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/_test_middleware.py` & `newrelic-9.9.1/tests/framework_flask/_test_middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/_test_not_found.py` & `newrelic-9.9.1/tests/framework_flask/_test_not_found.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/_test_user_exceptions.py` & `newrelic-9.9.1/tests/framework_flask/_test_user_exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/_test_views.py` & `newrelic-9.9.1/tests/framework_flask/_test_views.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/_test_views_async.py` & `newrelic-9.9.1/tests/framework_flask/_test_views_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/conftest.py` & `newrelic-9.9.1/tests/framework_flask/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/test_application.py` & `newrelic-9.9.1/tests/framework_flask/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/test_blueprints.py` & `newrelic-9.9.1/tests/framework_flask/test_blueprints.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/test_compress.py` & `newrelic-9.9.1/tests/framework_flask/test_compress.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/test_middleware.py` & `newrelic-9.9.1/tests/framework_flask/test_middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/test_not_found.py` & `newrelic-9.9.1/tests/framework_flask/test_not_found.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/test_user_exceptions.py` & `newrelic-9.9.1/tests/framework_flask/test_user_exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_flask/test_views.py` & `newrelic-9.9.1/tests/framework_flask/test_views.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_graphene/__init__.py` & `newrelic-9.9.1/tests/framework_graphene/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_graphene/_target_application.py` & `newrelic-9.9.1/tests/framework_graphene/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_graphene/_target_schema_async.py` & `newrelic-9.9.1/tests/framework_graphene/_target_schema_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_graphene/_target_schema_sync.py` & `newrelic-9.9.1/tests/framework_graphene/_target_schema_sync.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_graphene/conftest.py` & `newrelic-9.9.1/tests/framework_graphene/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_graphene/test_application.py` & `newrelic-9.9.1/tests/framework_graphene/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_graphql/__init__.py` & `newrelic-9.9.1/tests/framework_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_graphql/_target_application.py` & `newrelic-9.9.1/tests/framework_graphql/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_graphql/_target_schema_async.py` & `newrelic-9.9.1/tests/framework_graphql/_target_schema_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_graphql/_target_schema_sync.py` & `newrelic-9.9.1/tests/framework_graphql/_target_schema_sync.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_graphql/conftest.py` & `newrelic-9.9.1/tests/framework_graphql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_graphql/test_application.py` & `newrelic-9.9.1/tests/framework_graphql/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_graphql/test_application_async.py` & `newrelic-9.9.1/tests/framework_graphql/test_application_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_grpc/_test_common.py` & `newrelic-9.9.1/tests/framework_grpc/_test_common.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_grpc/conftest.py` & `newrelic-9.9.1/tests/framework_grpc/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_grpc/sample_application/__init__.py` & `newrelic-9.9.1/tests/framework_grpc/sample_application/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_grpc/sample_application/sample_application.proto` & `newrelic-9.9.1/tests/framework_grpc/sample_application/sample_application.proto`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_grpc/test_clients.py` & `newrelic-9.9.1/tests/framework_grpc/test_clients.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_grpc/test_distributed_tracing.py` & `newrelic-9.9.1/tests/framework_grpc/test_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_grpc/test_get_url.py` & `newrelic-9.9.1/tests/framework_grpc/test_get_url.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_grpc/test_server.py` & `newrelic-9.9.1/tests/framework_grpc/test_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_pyramid/_test_append_slash_app.py` & `newrelic-9.9.1/tests/framework_pyramid/_test_append_slash_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_pyramid/_test_application.py` & `newrelic-9.9.1/tests/framework_pyramid/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_pyramid/conftest.py` & `newrelic-9.9.1/tests/framework_pyramid/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_pyramid/test_append_slash_app.py` & `newrelic-9.9.1/tests/framework_pyramid/test_append_slash_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_pyramid/test_application.py` & `newrelic-9.9.1/tests/framework_pyramid/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_pyramid/test_cornice.py` & `newrelic-9.9.1/tests/framework_pyramid/test_cornice.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_sanic/_target_application.py` & `newrelic-9.9.1/tests/framework_sanic/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_sanic/conftest.py` & `newrelic-9.9.1/tests/framework_sanic/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_sanic/test_application.py` & `newrelic-9.9.1/tests/framework_sanic/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_sanic/test_cross_application.py` & `newrelic-9.9.1/tests/framework_sanic/test_cross_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_starlette/_test_application.py` & `newrelic-9.9.1/tests/framework_starlette/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_starlette/_test_bg_tasks.py` & `newrelic-9.9.1/tests/framework_starlette/_test_bg_tasks.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_starlette/_test_graphql.py` & `newrelic-9.9.1/tests/framework_starlette/_test_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_starlette/conftest.py` & `newrelic-9.9.1/tests/framework_starlette/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_starlette/test_application.py` & `newrelic-9.9.1/tests/framework_starlette/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_starlette/test_bg_tasks.py` & `newrelic-9.9.1/tests/framework_starlette/test_bg_tasks.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_strawberry/__init__.py` & `newrelic-9.9.1/tests/framework_strawberry/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_strawberry/_target_application.py` & `newrelic-9.9.1/tests/framework_strawberry/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_strawberry/_target_schema_async.py` & `newrelic-9.9.1/tests/framework_strawberry/_target_schema_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_strawberry/_target_schema_sync.py` & `newrelic-9.9.1/tests/framework_strawberry/_target_schema_sync.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_strawberry/conftest.py` & `newrelic-9.9.1/tests/framework_strawberry/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_strawberry/test_application.py` & `newrelic-9.9.1/tests/framework_strawberry/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_tornado/_target_application.py` & `newrelic-9.9.1/tests/framework_tornado/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_tornado/conftest.py` & `newrelic-9.9.1/tests/framework_tornado/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_tornado/test_custom_handler.py` & `newrelic-9.9.1/tests/framework_tornado/test_custom_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_tornado/test_externals.py` & `newrelic-9.9.1/tests/framework_tornado/test_externals.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_tornado/test_inbound_cat.py` & `newrelic-9.9.1/tests/framework_tornado/test_inbound_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/framework_tornado/test_server.py` & `newrelic-9.9.1/tests/framework_tornado/test_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_logging/conftest.py` & `newrelic-9.9.1/tests/logger_logging/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_logging/test_attributes.py` & `newrelic-9.9.1/tests/logger_logging/test_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_logging/test_local_decorating.py` & `newrelic-9.9.1/tests/logger_logging/test_local_decorating.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_logging/test_log_forwarding.py` & `newrelic-9.9.1/tests/logger_logging/test_log_forwarding.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_logging/test_logging_handler.py` & `newrelic-9.9.1/tests/logger_logging/test_logging_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_logging/test_metrics.py` & `newrelic-9.9.1/tests/logger_logging/test_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_logging/test_settings.py` & `newrelic-9.9.1/tests/logger_logging/test_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_loguru/conftest.py` & `newrelic-9.9.1/tests/logger_loguru/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_loguru/test_attributes.py` & `newrelic-9.9.1/tests/logger_loguru/test_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_loguru/test_local_decorating.py` & `newrelic-9.9.1/tests/logger_loguru/test_local_decorating.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_loguru/test_log_forwarding.py` & `newrelic-9.9.1/tests/logger_loguru/test_log_forwarding.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_loguru/test_metrics.py` & `newrelic-9.9.1/tests/logger_loguru/test_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_loguru/test_settings.py` & `newrelic-9.9.1/tests/logger_loguru/test_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_structlog/conftest.py` & `newrelic-9.9.1/tests/logger_structlog/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_structlog/test_attributes.py` & `newrelic-9.9.1/tests/logger_structlog/test_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_structlog/test_local_decorating.py` & `newrelic-9.9.1/tests/logger_structlog/test_local_decorating.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_structlog/test_log_forwarding.py` & `newrelic-9.9.1/tests/logger_structlog/test_log_forwarding.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/logger_structlog/test_metrics.py` & `newrelic-9.9.1/tests/logger_structlog/test_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_confluentkafka/conftest.py` & `newrelic-9.9.1/tests/messagebroker_confluentkafka/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_confluentkafka/test_consumer.py` & `newrelic-9.9.1/tests/messagebroker_confluentkafka/test_consumer.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_confluentkafka/test_producer.py` & `newrelic-9.9.1/tests/messagebroker_confluentkafka/test_producer.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_confluentkafka/test_serialization.py` & `newrelic-9.9.1/tests/messagebroker_confluentkafka/test_serialization.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_kafkapython/conftest.py` & `newrelic-9.9.1/tests/messagebroker_kafkapython/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_kafkapython/test_consumer.py` & `newrelic-9.9.1/tests/messagebroker_kafkapython/test_consumer.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_kafkapython/test_heartbeat.py` & `newrelic-9.9.1/tests/messagebroker_kafkapython/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_kafkapython/test_producer.py` & `newrelic-9.9.1/tests/messagebroker_kafkapython/test_producer.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_kafkapython/test_serialization.py` & `newrelic-9.9.1/tests/messagebroker_kafkapython/test_serialization.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_pika/compat.py` & `newrelic-9.9.1/tests/messagebroker_pika/compat.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_pika/conftest.py` & `newrelic-9.9.1/tests/messagebroker_pika/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_pika/minversion.py` & `newrelic-9.9.1/tests/messagebroker_pika/minversion.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_pika/test_cat.py` & `newrelic-9.9.1/tests/messagebroker_pika/test_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_pika/test_distributed_tracing.py` & `newrelic-9.9.1/tests/messagebroker_pika/test_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_pika/test_memory_leak.py` & `newrelic-9.9.1/tests/messagebroker_pika/test_memory_leak.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_pika/test_pika_async_connection_consume.py` & `newrelic-9.9.1/tests/messagebroker_pika/test_pika_async_connection_consume.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_pika/test_pika_blocking_connection_consume.py` & `newrelic-9.9.1/tests/messagebroker_pika/test_pika_blocking_connection_consume.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py` & `newrelic-9.9.1/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_pika/test_pika_produce.py` & `newrelic-9.9.1/tests/messagebroker_pika/test_pika_produce.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/messagebroker_pika/test_pika_supportability.py` & `newrelic-9.9.1/tests/messagebroker_pika/test_pika_supportability.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_langchain/_mock_external_openai_server.py` & `newrelic-9.9.1/tests/mlmodel_langchain/_mock_external_openai_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_langchain/conftest.py` & `newrelic-9.9.1/tests/mlmodel_langchain/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_langchain/hello.pdf` & `newrelic-9.9.1/tests/mlmodel_langchain/hello.pdf`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_langchain/test_agent.py` & `newrelic-9.9.1/tests/mlmodel_langchain/test_agent.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_langchain/test_chain.py` & `newrelic-9.9.1/tests/mlmodel_langchain/test_chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1460,15 +1460,15 @@
     _test()
 
 
 @pytest.mark.parametrize(
     "create_function,call_function,input_",
     (
         (create_structured_output_runnable, "ainvoke", {"input": "Sally is 13"}),
-        (create_structured_output_chain, "arun", "Sally is 13"),
+        (create_structured_output_chain, "arun", "Sally is 13"),  # Deprecated in 0.2.0
     ),
 )
 @reset_core_stats_engine()
 @validate_custom_event_count(count=0)
 def test_async_langchain_chain_outside_transaction(
     set_trace_info, chat_openai_client, json_schema, prompt, create_function, call_function, input_, loop
 ):
```

### Comparing `newrelic-9.9.0/tests/mlmodel_langchain/test_tool.py` & `newrelic-9.9.1/tests/mlmodel_langchain/test_tool.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_langchain/test_vectorstore.py` & `newrelic-9.9.1/tests/mlmodel_langchain/test_vectorstore.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_openai/_mock_external_openai_server.py` & `newrelic-9.9.1/tests/mlmodel_openai/_mock_external_openai_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_openai/conftest.py` & `newrelic-9.9.1/tests/mlmodel_openai/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion.py` & `newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_error.py` & `newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion_error.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_error_v1.py` & `newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion_error_v1.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream.py` & `newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion_stream.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream_error.py` & `newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion_stream_error.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream_error_v1.py` & `newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion_stream_error_v1.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream_v1.py` & `newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion_stream_v1.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_v1.py` & `newrelic-9.9.1/tests/mlmodel_openai/test_chat_completion_v1.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_openai/test_embeddings.py` & `newrelic-9.9.1/tests/mlmodel_openai/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_error.py` & `newrelic-9.9.1/tests/mlmodel_openai/test_embeddings_error.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_error_v1.py` & `newrelic-9.9.1/tests/mlmodel_openai/test_embeddings_error_v1.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_stream_v1.py` & `newrelic-9.9.1/tests/mlmodel_openai/test_embeddings_stream_v1.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_v1.py` & `newrelic-9.9.1/tests/mlmodel_openai/test_embeddings_v1.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/conftest.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_calibration_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_calibration_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_cluster_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_cluster_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_compose_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_compose_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_covariance_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_covariance_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_cross_decomposition_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_cross_decomposition_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_discriminant_analysis_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_discriminant_analysis_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_dummy_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_dummy_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_ensemble_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_ensemble_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_feature_selection_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_feature_selection_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_gaussian_process_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_gaussian_process_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_inference_events.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_inference_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_kernel_ridge_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_kernel_ridge_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_linear_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_linear_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_metric_scorers.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_metric_scorers.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_mixture_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_mixture_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_ml_model.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_ml_model.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_model_selection_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_model_selection_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_multiclass_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_multiclass_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_multioutput_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_multioutput_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_naive_bayes_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_naive_bayes_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_neighbors_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_neighbors_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_neural_network_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_neural_network_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_pipeline_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_pipeline_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_prediction_stats.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_prediction_stats.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_semi_supervised_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_semi_supervised_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_svm_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_svm_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/mlmodel_sklearn/test_tree_models.py` & `newrelic-9.9.1/tests/mlmodel_sklearn/test_tree_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/template_genshi/conftest.py` & `newrelic-9.9.1/tests/template_genshi/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/template_genshi/test_genshi.py` & `newrelic-9.9.1/tests/template_genshi/test_genshi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/template_jinja2/conftest.py` & `newrelic-9.9.1/tests/template_jinja2/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/template_jinja2/test_jinja2.py` & `newrelic-9.9.1/tests/template_jinja2/test_jinja2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/template_mako/conftest.py` & `newrelic-9.9.1/tests/template_mako/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/template_mako/test_mako.py` & `newrelic-9.9.1/tests/template_mako/test_mako.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/__init__.py` & `newrelic-9.9.1/tests/testing_support/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/asgi_testing.py` & `newrelic-9.9.1/tests/testing_support/asgi_testing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/db_settings.py` & `newrelic-9.9.1/tests/testing_support/db_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/external_fixtures.py` & `newrelic-9.9.1/tests/testing_support/external_fixtures.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/fixture/__init__.py` & `newrelic-9.9.1/tests/testing_support/fixture/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/fixture/event_loop.py` & `newrelic-9.9.1/tests/testing_support/fixture/event_loop.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/fixtures.py` & `newrelic-9.9.1/tests/testing_support/fixtures.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/ml_testing_utils.py` & `newrelic-9.9.1/tests/testing_support/ml_testing_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/mock_external_grpc_server.py` & `newrelic-9.9.1/tests/testing_support/mock_external_grpc_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/mock_external_http_server.py` & `newrelic-9.9.1/tests/testing_support/mock_external_http_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/mock_http_client.py` & `newrelic-9.9.1/tests/testing_support/mock_http_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/sample_applications.py` & `newrelic-9.9.1/tests/testing_support/sample_applications.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/sample_asgi_applications.py` & `newrelic-9.9.1/tests/testing_support/sample_asgi_applications.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/util.py` & `newrelic-9.9.1/tests/testing_support/util.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/__init__.py` & `newrelic-9.9.1/tests/testing_support/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_apdex_metrics.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_apdex_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_application_error_event_count.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_application_error_event_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_application_error_trace_count.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_application_error_trace_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_application_errors.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_application_errors.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_browser_attributes.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_browser_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_code_level_metrics.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_cross_process_headers.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_cross_process_headers.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_custom_event.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_custom_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_custom_event_collector_json.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_custom_event_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_custom_events.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_custom_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_custom_parameters.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_custom_parameters.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_database_duration.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_database_duration.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_database_node.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_database_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_database_trace_inputs.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_database_trace_inputs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_datastore_trace_inputs.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_datastore_trace_inputs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_dimensional_metric_payload.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_dimensional_metric_payload.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_dimensional_metrics_outside_transaction.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_dimensional_metrics_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_distributed_trace_accepted.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_distributed_trace_accepted.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_distributed_tracing_header.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_distributed_tracing_header.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_error_event_attributes.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_error_event_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_error_event_attributes_outside_transaction.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_error_event_attributes_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_error_event_collector_json.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_error_event_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_error_trace_attributes.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_error_trace_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_error_trace_attributes_outside_transaction.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_error_trace_attributes_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_error_trace_collector_json.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_error_trace_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_external_node_params.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_external_node_params.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_function_called.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_function_called.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_internal_metrics.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_internal_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_log_event_collector_json.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_log_event_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_log_event_count.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_log_event_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_log_event_count_outside_transaction.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_log_event_count_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_log_events.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_log_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_log_events_outside_transaction.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_log_events_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_messagebroker_headers.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_messagebroker_headers.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_metric_payload.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_metric_payload.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_ml_event_count.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_ml_event_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_ml_event_count_outside_transaction.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_ml_event_count_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_ml_event_payload.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_ml_event_payload.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_ml_events.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_ml_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_ml_events_outside_transaction.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_ml_events_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_non_transaction_error_event.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_non_transaction_error_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_outbound_headers.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_outbound_headers.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_serverless_data.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_serverless_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_serverless_metadata.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_serverless_metadata.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_serverless_payload.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_serverless_payload.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_slow_sql_collector_json.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_slow_sql_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_span_events.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_span_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_sql_obfuscation.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_sql_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_synthetics_event.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_synthetics_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_synthetics_transaction_trace.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_synthetics_transaction_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_time_metrics_outside_transaction.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_time_metrics_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_count.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_transaction_count.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,24 +13,28 @@
 # limitations under the License.
 
 from newrelic.common.object_wrapper import (transient_function_wrapper,
         function_wrapper)
 
 
 def validate_transaction_count(count):
-    _transactions = []
+    transactions = []
 
     @transient_function_wrapper('newrelic.core.stats_engine',
             'StatsEngine.record_transaction')
     def _increment_count(wrapped, instance, args, kwargs):
-        _transactions.append(getattr(args[0], "name", True))
+        transactions.append(getattr(args[0], "name", True))
         return wrapped(*args, **kwargs)
 
     @function_wrapper
     def _validate_transaction_count(wrapped, instance, args, kwargs):
         _new_wrapped = _increment_count(wrapped)
         result = _new_wrapped(*args, **kwargs)
+
+        _transactions = list(transactions)
+        del transactions[:]  # Clear list for subsequent test runs
+
         assert count == len(_transactions), (count, len(_transactions), _transactions)
 
         return result
 
     return _validate_transaction_count
```

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_error_event_count.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_transaction_error_event_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_error_trace_attributes.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_transaction_error_trace_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_errors.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_transaction_errors.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_event_attributes.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_transaction_event_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_event_collector_json.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_transaction_event_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_metrics.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_transaction_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_slow_sql_count.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_transaction_slow_sql_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_trace_attributes.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_transaction_trace_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_tt_collector_json.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_tt_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_tt_parameters.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_tt_parameters.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tests/testing_support/validators/validate_tt_segment_params.py` & `newrelic-9.9.1/tests/testing_support/validators/validate_tt_segment_params.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.9.0/tox.ini` & `newrelic-9.9.1/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,16 @@
     python-mlmodel_openai-openai107-py312,
     python-mlmodel_openai-openailatest-{py37,py38,py39,py310,py311,py312},
     ; langchain dependency faiss-cpu isn't compatible with 3.12 yet.
     python-mlmodel_langchain-{py38,py39,py310,py311},
     python-mlmodel_sklearn-{py37}-scikitlearn0101,
     python-mlmodel_sklearn-{py38,py39,py310,py311,py312}-scikitlearnlatest,
     python-template_genshi-{py27,py37,py38,py39,py310,py311,py312}-genshilatest,
-    python-template_jinja2-{py37,py38,py39,py310,py311,py312}-jinja2latest,
+    python-template_jinja2-py37-jinja2030103,
+    python-template_jinja2-{py38,py39,py310,py311,py312}-jinja2latest,
     python-template_mako-{py27,py37,py38,py39,py310,py311,py312},
     rabbitmq-messagebroker_pika-{py37,py38,py39,py310,py311,py312,pypy310}-pikalatest,
     redis-datastore_redis-{py37,py38,py39,py310,py311,py312,pypy310}-redis{0400,latest},
     rediscluster-datastore_rediscluster-{py37,py311,py312,pypy310}-redislatest,
     solr-datastore_pysolr-{py27,py37,py38,py39,py310,py311,py312,pypy27,pypy310},
 
 [testenv]
@@ -350,15 +351,16 @@
     framework_tornado-tornadolatest: tornado
     framework_tornado-tornadomaster: https://github.com/tornadoweb/tornado/archive/master.zip
     mlmodel_openai-openai0: openai[datalib]<1.0
     mlmodel_openai-openai107: openai[datalib]<1.8
     mlmodel_openai-openailatest: openai[datalib]
     ; Required for openai testing
     mlmodel_openai: protobuf
-    mlmodel_langchain: langchain
+    ; Pinning to 0.1.16 while adding support for with_structured_output in chain tests
+    mlmodel_langchain: langchain<0.1.17
     mlmodel_langchain: langchain-community
     mlmodel_langchain: openai[datalib]
     ; Required for langchain testing
     mlmodel_langchain: pypdf
     mlmodel_langchain: tiktoken
     mlmodel_langchain: faiss-cpu
     mlmodel_langchain: mock
@@ -376,14 +378,15 @@
     messagebroker_confluentkafka-confluentkafka0107: confluent-kafka<1.8
     messagebroker_confluentkafka-confluentkafka0106: confluent-kafka<1.7
     messagebroker_kafkapython-kafkapythonlatest: kafka-python
     messagebroker_kafkapython-kafkapython020001: kafka-python<2.0.2
     messagebroker_kafkapython-kafkapython020000: kafka-python<2.0.1
     template_genshi-genshilatest: genshi
     template_jinja2-jinja2latest: Jinja2
+    template_jinja2-jinja2030103: Jinja2<3.1.4
     template_mako: mako
 
 setenv =
     PYTHONPATH={toxinidir}/tests
     TOX_ENV_DIR={envdir}
     COVERAGE_FILE={envdir}/.coverage.{envname}
     COVERAGE_RCFILE={toxinidir}/tox.ini
```

