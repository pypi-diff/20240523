# Comparing `tmp/python-barbicanclient-5.7.0.tar.gz` & `tmp/python-barbicanclient-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-barbicanclient-5.7.0.tar", last modified: Fri Mar  1 13:49:52 2024, max compression
+gzip compressed data, was "python-barbicanclient-6.0.0.tar", last modified: Thu May 23 08:01:56 2024, max compression
```

## Comparing `python-barbicanclient-5.7.0.tar` & `python-barbicanclient-6.0.0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.587508 python-barbicanclient-5.7.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4594 2024-03-01 13:49:52.000000 python-barbicanclient-5.7.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22267 2024-03-01 13:49:52.000000 python-barbicanclient-5.7.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11366 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12966 2024-03-01 13:49:52.587508 python-barbicanclient-5.7.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10338 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.563782 python-barbicanclient-5.7.0/barbicanclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2029 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16618 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/barbican.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.563782 python-barbicanclient-5.7.0/barbicanclient/barbican_cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/barbican_cli/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.567736 python-barbicanclient-5.7.0/barbicanclient/barbican_cli/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/barbican_cli/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10595 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/barbican_cli/v1/acls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2160 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/barbican_cli/v1/cas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5853 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/barbican_cli/v1/containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6117 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/barbican_cli/v1/orders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12385 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/barbican_cli/v1/secrets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2418 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9024 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1426 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1947 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/formatter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1610 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/osc_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.567736 python-barbicanclient-5.7.0/barbicanclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10155 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/tests/keystone_client_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12490 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/tests/test_barbican.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2189 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/tests/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18585 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/tests/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2738 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/tests/test_formatter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4009 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.571690 python-barbicanclient-5.7.0/barbicanclient/tests/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/tests/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22367 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/tests/v1/test_acls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5386 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/tests/v1/test_cas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6815 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/tests/v1/test_consumers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25838 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/tests/v1/test_containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17044 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/tests/v1/test_orders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22825 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/tests/v1/test_secrets.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.571690 python-barbicanclient-5.7.0/barbicanclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18946 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/v1/acls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7347 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/v1/cas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5843 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/v1/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28575 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/v1/containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19523 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/v1/orders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28422 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/v1/secrets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/barbicanclient/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/clientrc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.571690 python-barbicanclient-5.7.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.571690 python-barbicanclient-5.7.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.575645 python-barbicanclient-5.7.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5210 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/doc/source/cli/authentication.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32497 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/doc/source/cli/cli_usage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26948 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/doc/source/cli/details.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13007 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/doc/source/cli/usage.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2837 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.575645 python-barbicanclient-5.7.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5678 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/doc/source/contributor/testing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.575645 python-barbicanclient-5.7.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.575645 python-barbicanclient-5.7.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1323 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.575645 python-barbicanclient-5.7.0/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/etc/barbicanclient.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/etc/functional_tests.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.575645 python-barbicanclient-5.7.0/functionaltests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.575645 python-barbicanclient-5.7.0/functionaltests/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      771 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.575645 python-barbicanclient-5.7.0/functionaltests/cli/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.579599 python-barbicanclient-5.7.0/functionaltests/cli/v1/behaviors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/v1/behaviors/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7547 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/v1/behaviors/acl_behaviors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5101 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/v1/behaviors/base_behaviors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2150 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/v1/behaviors/consumer_behaviors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3271 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/v1/behaviors/container_behaviors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7183 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/v1/behaviors/secret_behaviors.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.579599 python-barbicanclient-5.7.0/functionaltests/cli/v1/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/v1/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.579599 python-barbicanclient-5.7.0/functionaltests/cli/v1/smoke/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/v1/smoke/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10742 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/v1/smoke/test_acl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5805 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/v1/smoke/test_consumer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2892 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/v1/smoke/test_container.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/v1/smoke/test_help.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5891 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/cli/v1/smoke/test_secret.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.579599 python-barbicanclient-5.7.0/functionaltests/client/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/client/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1842 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/client/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6795 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/client/test_client_connectivity.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.579599 python-barbicanclient-5.7.0/functionaltests/client/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/client/v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.583553 python-barbicanclient-5.7.0/functionaltests/client/v1/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/client/v1/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22945 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/client/v1/functional/test_acl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13936 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/client/v1/functional/test_containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16327 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/client/v1/functional/test_orders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45156 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/client/v1/functional/test_secrets.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.583553 python-barbicanclient-5.7.0/functionaltests/client/v1/smoke/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/client/v1/smoke/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7089 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/client/v1/smoke/test_containers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5342 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/client/v1/smoke/test_orders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5734 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/client/v1/smoke/test_secrets.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.583553 python-barbicanclient-5.7.0/functionaltests/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3774 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/common/cleanup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2775 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21149 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/common/keys.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5703 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/functionaltests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.587508 python-barbicanclient-5.7.0/python_barbicanclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12966 2024-03-01 13:49:52.000000 python-barbicanclient-5.7.0/python_barbicanclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3910 2024-03-01 13:49:52.000000 python-barbicanclient-5.7.0/python_barbicanclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-01 13:49:52.000000 python-barbicanclient-5.7.0/python_barbicanclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1726 2024-03-01 13:49:52.000000 python-barbicanclient-5.7.0/python_barbicanclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-01 13:49:52.000000 python-barbicanclient-5.7.0/python_barbicanclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-01 13:49:52.000000 python-barbicanclient-5.7.0/python_barbicanclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-03-01 13:49:52.000000 python-barbicanclient-5.7.0/python_barbicanclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2024-03-01 13:49:52.000000 python-barbicanclient-5.7.0/python_barbicanclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.559827 python-barbicanclient-5.7.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 13:49:52.587508 python-barbicanclient-5.7.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/releasenotes/notes/add-secret-consumers-a65cd6b22d28184d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/releasenotes/notes/drop-py-2-7-50042a0e2227c095.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/releasenotes/notes/use-only-uuid-from-href-81710d1b388dce57.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      679 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2743 2024-03-01 13:49:52.587508 python-barbicanclient-5.7.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1757 2024-03-01 13:49:28.000000 python-barbicanclient-5.7.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.740876 python-barbicanclient-6.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4639 2024-05-23 08:01:56.000000 python-barbicanclient-6.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22427 2024-05-23 08:01:56.000000 python-barbicanclient-6.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11366 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12968 2024-05-23 08:01:56.740876 python-barbicanclient-6.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10338 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.728877 python-barbicanclient-6.0.0/barbicanclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2029 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16618 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/barbican.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.728877 python-barbicanclient-6.0.0/barbicanclient/barbican_cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/barbican_cli/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.728877 python-barbicanclient-6.0.0/barbicanclient/barbican_cli/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/barbican_cli/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10595 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/barbican_cli/v1/acls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2160 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/barbican_cli/v1/cas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5853 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/barbican_cli/v1/containers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6117 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/barbican_cli/v1/orders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12385 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/barbican_cli/v1/secrets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2418 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9024 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1426 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1947 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/formatter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1610 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/osc_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.728877 python-barbicanclient-6.0.0/barbicanclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10155 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/tests/keystone_client_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12490 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/tests/test_barbican.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2189 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/tests/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18585 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/tests/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2738 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/tests/test_formatter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4009 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.732876 python-barbicanclient-6.0.0/barbicanclient/tests/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/tests/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22367 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/tests/v1/test_acls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5386 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/tests/v1/test_cas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6815 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/tests/v1/test_consumers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25838 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/tests/v1/test_containers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17044 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/tests/v1/test_orders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22825 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/tests/v1/test_secrets.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.732876 python-barbicanclient-6.0.0/barbicanclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18946 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/v1/acls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7347 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/v1/cas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5843 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/v1/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28575 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/v1/containers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19523 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/v1/orders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28422 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/v1/secrets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/barbicanclient/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/clientrc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.732876 python-barbicanclient-6.0.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.732876 python-barbicanclient-6.0.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.732876 python-barbicanclient-6.0.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5210 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/doc/source/cli/authentication.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32497 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/doc/source/cli/cli_usage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26948 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/doc/source/cli/details.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13007 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/doc/source/cli/usage.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2837 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.732876 python-barbicanclient-6.0.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5678 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/doc/source/contributor/testing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.732876 python-barbicanclient-6.0.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.732876 python-barbicanclient-6.0.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1323 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.732876 python-barbicanclient-6.0.0/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/etc/barbicanclient.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/etc/functional_tests.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.732876 python-barbicanclient-6.0.0/functionaltests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.736876 python-barbicanclient-6.0.0/functionaltests/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      771 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.736876 python-barbicanclient-6.0.0/functionaltests/cli/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.736876 python-barbicanclient-6.0.0/functionaltests/cli/v1/behaviors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/v1/behaviors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7547 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/v1/behaviors/acl_behaviors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5101 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/v1/behaviors/base_behaviors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2150 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/v1/behaviors/consumer_behaviors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3271 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/v1/behaviors/container_behaviors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7183 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/v1/behaviors/secret_behaviors.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.736876 python-barbicanclient-6.0.0/functionaltests/cli/v1/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/v1/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.736876 python-barbicanclient-6.0.0/functionaltests/cli/v1/smoke/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/v1/smoke/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10742 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/v1/smoke/test_acl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5805 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/v1/smoke/test_consumer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2892 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/v1/smoke/test_container.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/v1/smoke/test_help.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5891 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/cli/v1/smoke/test_secret.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.736876 python-barbicanclient-6.0.0/functionaltests/client/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/client/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1842 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/client/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6795 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/client/test_client_connectivity.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.736876 python-barbicanclient-6.0.0/functionaltests/client/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/client/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.736876 python-barbicanclient-6.0.0/functionaltests/client/v1/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/client/v1/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22945 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/client/v1/functional/test_acl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13936 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/client/v1/functional/test_containers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16344 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/client/v1/functional/test_orders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45156 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/client/v1/functional/test_secrets.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.740876 python-barbicanclient-6.0.0/functionaltests/client/v1/smoke/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/client/v1/smoke/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7089 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/client/v1/smoke/test_containers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5342 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/client/v1/smoke/test_orders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5734 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/client/v1/smoke/test_secrets.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.740876 python-barbicanclient-6.0.0/functionaltests/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3774 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/common/cleanup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2775 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21149 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/common/keys.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5703 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/functionaltests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.740876 python-barbicanclient-6.0.0/python_barbicanclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12968 2024-05-23 08:01:56.000000 python-barbicanclient-6.0.0/python_barbicanclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3910 2024-05-23 08:01:56.000000 python-barbicanclient-6.0.0/python_barbicanclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:01:56.000000 python-barbicanclient-6.0.0/python_barbicanclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1726 2024-05-23 08:01:56.000000 python-barbicanclient-6.0.0/python_barbicanclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:01:56.000000 python-barbicanclient-6.0.0/python_barbicanclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-23 08:01:56.000000 python-barbicanclient-6.0.0/python_barbicanclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-23 08:01:56.000000 python-barbicanclient-6.0.0/python_barbicanclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2024-05-23 08:01:56.000000 python-barbicanclient-6.0.0/python_barbicanclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.724877 python-barbicanclient-6.0.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:56.740876 python-barbicanclient-6.0.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/releasenotes/notes/add-secret-consumers-a65cd6b22d28184d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/releasenotes/notes/drop-py-2-7-50042a0e2227c095.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/releasenotes/notes/use-only-uuid-from-href-81710d1b388dce57.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2745 2024-05-23 08:01:56.740876 python-barbicanclient-6.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1757 2024-05-23 08:01:15.000000 python-barbicanclient-6.0.0/tox.ini
```

### Comparing `python-barbicanclient-5.7.0/.zuul.yaml` & `python-barbicanclient-6.0.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/AUTHORS` & `python-barbicanclient-6.0.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 Sean McGinnis <sean.mcginnis@gmail.com>
 ShangXiao <shangxiaobj@inspur.com>
 Shuquan Huang <huang.shuquan@99cloud.net>
 Stephen Finucane <stephenfin@redhat.com>
 Steve Heyman <steve.heyman@rackspace.com>
 Steven Gonzales <stevendgonzales@gmail.com>
 Swapnil Kulkarni (coolsvap) <me@coolsvap.net>
+Takashi Kajinami <kajinamit@oss.nttdata.com>
 Takashi Kajinami <tkajinam@redhat.com>
 Thiago da Silva <thiago@redhat.com>
 Thomas Dinkjian <thomas.dinkjian@rackspace.com>
 Thomas Herve <therve@redhat.com>
 Thomas Herve <thomas.herve@enovance.com>
 Tin Lam <tl3438@att.com>
 Tony Breeds <tony@bakeyournoodle.com>
```

### Comparing `python-barbicanclient-5.7.0/CONTRIBUTING.rst` & `python-barbicanclient-6.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/ChangeLog` & `python-barbicanclient-6.0.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 CHANGES
 =======
 
+6.0.0
+-----
+
+* Remove old excludes
+* Replace pytz
+* Bump hacking
+* Bump hacking
+* coveragerc: Remove non-existent path
+* Update python classifier in setup.cfg
+
 5.7.0
 -----
 
 * Migrate back to Launchpad
 
 5.6.1
 -----
```

### Comparing `python-barbicanclient-5.7.0/LICENSE` & `python-barbicanclient-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/PKG-INFO` & `python-barbicanclient-6.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python-barbicanclient
-Version: 5.7.0
+Version: 6.0.0
 Summary: Client Library for OpenStack Barbican Key Management API
 Home-page: https://docs.openstack.org/python-barbicanclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: python-barbicanclient
         =====================
@@ -225,11 +225,11 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `python-barbicanclient-5.7.0/README.rst` & `python-barbicanclient-6.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/__init__.py` & `python-barbicanclient-6.0.0/barbicanclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/_i18n.py` & `python-barbicanclient-6.0.0/barbicanclient/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/barbican.py` & `python-barbicanclient-6.0.0/barbicanclient/barbican.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/barbican_cli/v1/acls.py` & `python-barbicanclient-6.0.0/barbicanclient/barbican_cli/v1/acls.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/barbican_cli/v1/cas.py` & `python-barbicanclient-6.0.0/barbicanclient/barbican_cli/v1/cas.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/barbican_cli/v1/containers.py` & `python-barbicanclient-6.0.0/barbicanclient/barbican_cli/v1/containers.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/barbican_cli/v1/orders.py` & `python-barbicanclient-6.0.0/barbicanclient/barbican_cli/v1/orders.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/barbican_cli/v1/secrets.py` & `python-barbicanclient-6.0.0/barbicanclient/barbican_cli/v1/secrets.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/base.py` & `python-barbicanclient-6.0.0/barbicanclient/base.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/client.py` & `python-barbicanclient-6.0.0/barbicanclient/client.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/exceptions.py` & `python-barbicanclient-6.0.0/barbicanclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/formatter.py` & `python-barbicanclient-6.0.0/barbicanclient/formatter.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/osc_plugin.py` & `python-barbicanclient-6.0.0/barbicanclient/osc_plugin.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/tests/keystone_client_fixtures.py` & `python-barbicanclient-6.0.0/barbicanclient/tests/keystone_client_fixtures.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/tests/test_barbican.py` & `python-barbicanclient-6.0.0/barbicanclient/tests/test_barbican.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/tests/test_base.py` & `python-barbicanclient-6.0.0/barbicanclient/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/tests/test_client.py` & `python-barbicanclient-6.0.0/barbicanclient/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/tests/test_formatter.py` & `python-barbicanclient-6.0.0/barbicanclient/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/tests/utils.py` & `python-barbicanclient-6.0.0/barbicanclient/tests/utils.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/tests/v1/test_acls.py` & `python-barbicanclient-6.0.0/barbicanclient/tests/v1/test_acls.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/tests/v1/test_cas.py` & `python-barbicanclient-6.0.0/barbicanclient/tests/v1/test_cas.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/tests/v1/test_consumers.py` & `python-barbicanclient-6.0.0/barbicanclient/tests/v1/test_consumers.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/tests/v1/test_containers.py` & `python-barbicanclient-6.0.0/barbicanclient/tests/v1/test_containers.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/tests/v1/test_orders.py` & `python-barbicanclient-6.0.0/barbicanclient/tests/v1/test_orders.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/tests/v1/test_secrets.py` & `python-barbicanclient-6.0.0/barbicanclient/tests/v1/test_secrets.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/v1/acls.py` & `python-barbicanclient-6.0.0/barbicanclient/v1/acls.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/v1/cas.py` & `python-barbicanclient-6.0.0/barbicanclient/v1/cas.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/v1/client.py` & `python-barbicanclient-6.0.0/barbicanclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/v1/containers.py` & `python-barbicanclient-6.0.0/barbicanclient/v1/containers.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/v1/orders.py` & `python-barbicanclient-6.0.0/barbicanclient/v1/orders.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/v1/secrets.py` & `python-barbicanclient-6.0.0/barbicanclient/v1/secrets.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/barbicanclient/version.py` & `python-barbicanclient-6.0.0/barbicanclient/version.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/clientrc` & `python-barbicanclient-6.0.0/clientrc`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/doc/source/cli/authentication.rst` & `python-barbicanclient-6.0.0/doc/source/cli/authentication.rst`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/doc/source/cli/cli_usage.rst` & `python-barbicanclient-6.0.0/doc/source/cli/cli_usage.rst`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/doc/source/cli/details.rst` & `python-barbicanclient-6.0.0/doc/source/cli/details.rst`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/doc/source/cli/usage.rst` & `python-barbicanclient-6.0.0/doc/source/cli/usage.rst`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/doc/source/conf.py` & `python-barbicanclient-6.0.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/doc/source/contributor/testing.rst` & `python-barbicanclient-6.0.0/doc/source/contributor/testing.rst`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/doc/source/reference/index.rst` & `python-barbicanclient-6.0.0/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/etc/functional_tests.conf` & `python-barbicanclient-6.0.0/etc/functional_tests.conf`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/__init__.py` & `python-barbicanclient-6.0.0/functionaltests/__init__.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/base.py` & `python-barbicanclient-6.0.0/functionaltests/base.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/cli/base.py` & `python-barbicanclient-6.0.0/functionaltests/cli/base.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/cli/v1/behaviors/acl_behaviors.py` & `python-barbicanclient-6.0.0/functionaltests/cli/v1/behaviors/acl_behaviors.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/cli/v1/behaviors/base_behaviors.py` & `python-barbicanclient-6.0.0/functionaltests/cli/v1/behaviors/base_behaviors.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/cli/v1/behaviors/consumer_behaviors.py` & `python-barbicanclient-6.0.0/functionaltests/cli/v1/behaviors/consumer_behaviors.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/cli/v1/behaviors/container_behaviors.py` & `python-barbicanclient-6.0.0/functionaltests/cli/v1/behaviors/container_behaviors.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/cli/v1/behaviors/secret_behaviors.py` & `python-barbicanclient-6.0.0/functionaltests/cli/v1/behaviors/secret_behaviors.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/cli/v1/smoke/test_acl.py` & `python-barbicanclient-6.0.0/functionaltests/cli/v1/smoke/test_acl.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/cli/v1/smoke/test_consumer.py` & `python-barbicanclient-6.0.0/functionaltests/cli/v1/smoke/test_consumer.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/cli/v1/smoke/test_container.py` & `python-barbicanclient-6.0.0/functionaltests/cli/v1/smoke/test_container.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/cli/v1/smoke/test_help.py` & `python-barbicanclient-6.0.0/functionaltests/cli/v1/smoke/test_help.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/cli/v1/smoke/test_secret.py` & `python-barbicanclient-6.0.0/functionaltests/cli/v1/smoke/test_secret.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/client/base.py` & `python-barbicanclient-6.0.0/functionaltests/client/base.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/client/test_client_connectivity.py` & `python-barbicanclient-6.0.0/functionaltests/client/test_client_connectivity.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/client/v1/functional/test_acl.py` & `python-barbicanclient-6.0.0/functionaltests/client/v1/functional/test_acl.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/client/v1/functional/test_containers.py` & `python-barbicanclient-6.0.0/functionaltests/client/v1/functional/test_containers.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/client/v1/functional/test_orders.py` & `python-barbicanclient-6.0.0/functionaltests/client/v1/functional/test_orders.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 # implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import pytz
+import datetime
 import sys
 
 from functionaltests.client import base
 from functionaltests.common import cleanup
 from functionaltests import utils
 from oslo_utils import timeutils
 from testtools import testcase
@@ -428,15 +428,15 @@
     })
     @testcase.attr('positive')
     def test_create_order_defaults_valid_expiration(self, **kwargs):
         """Covers creating orders with various valid expiration data."""
         timestamp = utils.create_timestamp_w_tz_and_offset(**kwargs)
 
         date = timeutils.parse_isotime(timestamp)
-        date = date.astimezone(pytz.utc)
+        date = date.astimezone(datetime.timezone.utc)
 
         order = self.barbicanclient.orders.create_key(**order_create_key_data)
         order.expiration = timestamp
 
         order_ref = self.cleanup.add_entity(order)
         self.assertIsNotNone(order_ref)
```

### Comparing `python-barbicanclient-5.7.0/functionaltests/client/v1/functional/test_secrets.py` & `python-barbicanclient-6.0.0/functionaltests/client/v1/functional/test_secrets.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/client/v1/smoke/test_containers.py` & `python-barbicanclient-6.0.0/functionaltests/client/v1/smoke/test_containers.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/client/v1/smoke/test_orders.py` & `python-barbicanclient-6.0.0/functionaltests/client/v1/smoke/test_orders.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/client/v1/smoke/test_secrets.py` & `python-barbicanclient-6.0.0/functionaltests/client/v1/smoke/test_secrets.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/common/cleanup.py` & `python-barbicanclient-6.0.0/functionaltests/common/cleanup.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/common/config.py` & `python-barbicanclient-6.0.0/functionaltests/common/config.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/common/keys.py` & `python-barbicanclient-6.0.0/functionaltests/common/keys.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/functionaltests/utils.py` & `python-barbicanclient-6.0.0/functionaltests/utils.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/python_barbicanclient.egg-info/PKG-INFO` & `python-barbicanclient-6.0.0/python_barbicanclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python-barbicanclient
-Version: 5.7.0
+Version: 6.0.0
 Summary: Client Library for OpenStack Barbican Key Management API
 Home-page: https://docs.openstack.org/python-barbicanclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: python-barbicanclient
         =====================
@@ -225,11 +225,11 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `python-barbicanclient-5.7.0/python_barbicanclient.egg-info/SOURCES.txt` & `python-barbicanclient-6.0.0/python_barbicanclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/python_barbicanclient.egg-info/entry_points.txt` & `python-barbicanclient-6.0.0/python_barbicanclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/releasenotes/notes/add-secret-consumers-a65cd6b22d28184d.yaml` & `python-barbicanclient-6.0.0/releasenotes/notes/add-secret-consumers-a65cd6b22d28184d.yaml`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/setup.cfg` & `python-barbicanclient-6.0.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [files]
 packages = 
 	barbicanclient
 
 [entry_points]
 console_scripts =
```

### Comparing `python-barbicanclient-5.7.0/setup.py` & `python-barbicanclient-6.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-barbicanclient-5.7.0/tox.ini` & `python-barbicanclient-6.0.0/tox.ini`

 * *Files identical despite different names*

