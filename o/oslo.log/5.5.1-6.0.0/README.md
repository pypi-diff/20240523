# Comparing `tmp/oslo.log-5.5.1.tar.gz` & `tmp/oslo.log-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslo.log-5.5.1.tar", last modified: Tue Apr  2 07:48:27 2024, max compression
+gzip compressed data, was "oslo.log-6.0.0.tar", last modified: Thu May 23 08:14:42 2024, max compression
```

## Comparing `oslo.log-5.5.1.tar` & `oslo.log-6.0.0.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.967316 oslo.log-5.5.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-04-02 07:48:05.000000 oslo.log-5.5.1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-04-02 07:48:05.000000 oslo.log-5.5.1/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      974 2024-04-02 07:48:05.000000 oslo.log-5.5.1/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-04-02 07:48:05.000000 oslo.log-5.5.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1254 2024-04-02 07:48:05.000000 oslo.log-5.5.1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7506 2024-04-02 07:48:27.000000 oslo.log-5.5.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2024-04-02 07:48:05.000000 oslo.log-5.5.1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28969 2024-04-02 07:48:27.000000 oslo.log-5.5.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2024-04-02 07:48:05.000000 oslo.log-5.5.1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2024-04-02 07:48:05.000000 oslo.log-5.5.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2024-04-02 07:48:27.967316 oslo.log-5.5.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2024-04-02 07:48:05.000000 oslo.log-5.5.1/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.943314 oslo.log-5.5.1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.943314 oslo.log-5.5.1/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.947314 oslo.log-5.5.1/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/admin/advanced_config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2785 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/admin/example_nova.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5116 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/admin/journal.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/admin/log_rotation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1777 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/admin/nova_sample.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.947314 oslo.log-5.5.1/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4456 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.947314 oslo.log-5.5.1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      694 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.947314 oslo.log-5.5.1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.947314 oslo.log-5.5.1/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/reference/fixtures.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/reference/formatters.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/reference/handlers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/reference/helpers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/reference/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/reference/log.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/reference/versionutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/reference/watchers.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.947314 oslo.log-5.5.1/doc/source/user/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.951315 oslo.log-5.5.1/doc/source/user/examples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1572 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/user/examples/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/user/examples/oslo_logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/user/examples/python_logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/user/examples/usage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/user/examples/usage_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3103 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/user/examples/usage_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/user/examples.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11454 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/user/guidelines.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4721 2024-04-02 07:48:05.000000 oslo.log-5.5.1/doc/source/user/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.951315 oslo.log-5.5.1/oslo.log.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2024-04-02 07:48:27.000000 oslo.log-5.5.1/oslo.log.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4699 2024-04-02 07:48:27.000000 oslo.log-5.5.1/oslo.log.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-02 07:48:27.000000 oslo.log-5.5.1/oslo.log.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-04-02 07:48:27.000000 oslo.log-5.5.1/oslo.log.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-02 07:48:27.000000 oslo.log-5.5.1/oslo.log.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-04-02 07:48:27.000000 oslo.log-5.5.1/oslo.log.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-04-02 07:48:27.000000 oslo.log-5.5.1/oslo.log.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-04-02 07:48:27.000000 oslo.log-5.5.1/oslo.log.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.955315 oslo.log-5.5.1/oslo_log/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11091 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/_options.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.955315 oslo.log-5.5.1/oslo_log/cmds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/cmds/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6858 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/cmds/convert_json.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.955315 oslo.log-5.5.1/oslo_log/fixture/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/fixture/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1177 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/fixture/logging_error.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/fixture/setlevel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21644 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/formatters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4988 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/handlers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2201 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/helpers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.939314 oslo.log-5.5.1/oslo_log/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.939314 oslo.log-5.5.1/oslo_log/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.955315 oslo.log-5.5.1/oslo_log/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1992 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/locale/de/LC_MESSAGES/oslo_log.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.939314 oslo.log-5.5.1/oslo_log/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.955315 oslo.log-5.5.1/oslo_log/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2024 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/locale/en_GB/LC_MESSAGES/oslo_log.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.939314 oslo.log-5.5.1/oslo_log/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.955315 oslo.log-5.5.1/oslo_log/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2157 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/locale/es/LC_MESSAGES/oslo_log.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.939314 oslo.log-5.5.1/oslo_log/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.955315 oslo.log-5.5.1/oslo_log/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/locale/ja/LC_MESSAGES/oslo_log.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19444 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5238 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/pipe_mutex.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4762 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/rate_limit.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.955315 oslo.log-5.5.1/oslo_log/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.959315 oslo.log-5.5.1/oslo_log/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.959315 oslo.log-5.5.1/oslo_log/tests/unit/fixture/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/tests/unit/fixture/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/tests/unit/fixture/test_logging_error.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1449 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/tests/unit/fixture/test_setlevel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2966 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/tests/unit/test_convert_json.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1998 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/tests/unit/test_custom_loghandler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5169 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/tests/unit/test_formatters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2775 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/tests/unit/test_helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    79067 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/tests/unit/test_log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6603 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/tests/unit/test_pipe_mutex.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3767 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/tests/unit/test_rate_limit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14051 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/tests/unit/test_versionutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      688 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10409 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/versionutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3774 2024-04-02 07:48:05.000000 oslo.log-5.5.1/oslo_log/watchers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.939314 oslo.log-5.5.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.963315 oslo.log-5.5.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/add-context-section-0b2f411ec64f42f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/add-facility-to-journal-e10bf7002cc19dd3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/add-reno-e4fedb11ece56f1e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/add-system_scope-to-logging_user_identity_format-0581ce5070740375.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      381 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/always-add-error-text-715022964364ffa0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/deprecate-windows-support-75e6ac72310d5e72.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/drop-python27-support-0fe4909a5468feb3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/info-logging-7b7be9fc7a95aebc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/init-global-request-id-eb2031bc221e5fb7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/is_debug_enabled-d7afee4c811a46df.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/jsonformatter-repr-fd616eb6fa6caeb3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/log-global_request_id-f97e6d663e8a80b3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/log-rotation-595f8232cd987a6d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/native-threads-logging-cc84f7288c4835a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/reload_log_config-743817192b1172b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/remove-log-format-b4b949701cee3315.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/remove-syslog-rfc-format-7a06772c0bb48e9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/remove-verbose-option-d0d1381e182d1be1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/systemd-journal-support-fcbc34b3c5ce93ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/use-json-option-96f71da54a3b9a18.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/use-project-in-user-identity-93fd6e0a2e434a6f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/use_stderr_default_false-50d846b88cf2be90.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/notes/windows-eventlog-2beb0a6010e342eb.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.967316 oslo.log-5.5.1/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.967316 oslo.log-5.5.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.967316 oslo.log-5.5.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/liberty.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.939314 oslo.log-5.5.1/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.939314 oslo.log-5.5.1/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.967316 oslo.log-5.5.1/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10458 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.939314 oslo.log-5.5.1/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-02 07:48:27.967316 oslo.log-5.5.1/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-04-02 07:48:05.000000 oslo.log-5.5.1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2024-04-02 07:48:05.000000 oslo.log-5.5.1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2024-04-02 07:48:27.967316 oslo.log-5.5.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-04-02 07:48:05.000000 oslo.log-5.5.1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2024-04-02 07:48:05.000000 oslo.log-5.5.1/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1574 2024-04-02 07:48:05.000000 oslo.log-5.5.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.467394 oslo.log-6.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-05-23 08:14:12.000000 oslo.log-6.0.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-05-23 08:14:12.000000 oslo.log-6.0.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      974 2024-05-23 08:14:12.000000 oslo.log-6.0.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-05-23 08:14:12.000000 oslo.log-6.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1254 2024-05-23 08:14:12.000000 oslo.log-6.0.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7506 2024-05-23 08:14:42.000000 oslo.log-6.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2024-05-23 08:14:12.000000 oslo.log-6.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29300 2024-05-23 08:14:42.000000 oslo.log-6.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2024-05-23 08:14:12.000000 oslo.log-6.0.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2024-05-23 08:14:12.000000 oslo.log-6.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2024-05-23 08:14:42.467394 oslo.log-6.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2024-05-23 08:14:12.000000 oslo.log-6.0.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.447387 oslo.log-6.0.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.447387 oslo.log-6.0.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.447387 oslo.log-6.0.0/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/admin/advanced_config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2785 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/admin/example_nova.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5116 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/admin/journal.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/admin/log_rotation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1777 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/admin/nova_sample.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.447387 oslo.log-6.0.0/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4456 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.447387 oslo.log-6.0.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      694 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.447387 oslo.log-6.0.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.447387 oslo.log-6.0.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/reference/fixtures.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/reference/formatters.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/reference/handlers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/reference/helpers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/reference/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/reference/log.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/reference/versionutils.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.451388 oslo.log-6.0.0/doc/source/user/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.451388 oslo.log-6.0.0/doc/source/user/examples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1572 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/user/examples/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/user/examples/oslo_logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/user/examples/python_logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/user/examples/usage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/user/examples/usage_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3103 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/user/examples/usage_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/user/examples.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11454 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/user/guidelines.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4721 2024-05-23 08:14:12.000000 oslo.log-6.0.0/doc/source/user/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.451388 oslo.log-6.0.0/oslo.log.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2024-05-23 08:14:42.000000 oslo.log-6.0.0/oslo.log.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4741 2024-05-23 08:14:42.000000 oslo.log-6.0.0/oslo.log.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:14:42.000000 oslo.log-6.0.0/oslo.log.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-05-23 08:14:42.000000 oslo.log-6.0.0/oslo.log.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:14:42.000000 oslo.log-6.0.0/oslo.log.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-23 08:14:42.000000 oslo.log-6.0.0/oslo.log.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2024-05-23 08:14:42.000000 oslo.log-6.0.0/oslo.log.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-05-23 08:14:42.000000 oslo.log-6.0.0/oslo.log.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.455390 oslo.log-6.0.0/oslo_log/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11349 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/_options.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.455390 oslo.log-6.0.0/oslo_log/cmds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/cmds/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6858 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/cmds/convert_json.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.455390 oslo.log-6.0.0/oslo_log/fixture/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/fixture/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1177 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/fixture/logging_error.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/fixture/setlevel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21250 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/formatters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4988 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/handlers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2201 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/helpers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.439384 oslo.log-6.0.0/oslo_log/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.439384 oslo.log-6.0.0/oslo_log/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.455390 oslo.log-6.0.0/oslo_log/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1992 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/locale/de/LC_MESSAGES/oslo_log.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.439384 oslo.log-6.0.0/oslo_log/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.455390 oslo.log-6.0.0/oslo_log/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2024 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/locale/en_GB/LC_MESSAGES/oslo_log.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.439384 oslo.log-6.0.0/oslo_log/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.455390 oslo.log-6.0.0/oslo_log/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2157 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/locale/es/LC_MESSAGES/oslo_log.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.439384 oslo.log-6.0.0/oslo_log/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.455390 oslo.log-6.0.0/oslo_log/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/locale/ja/LC_MESSAGES/oslo_log.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19557 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5238 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/pipe_mutex.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4762 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/rate_limit.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.455390 oslo.log-6.0.0/oslo_log/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.459391 oslo.log-6.0.0/oslo_log/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.459391 oslo.log-6.0.0/oslo_log/tests/unit/fixture/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/tests/unit/fixture/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/tests/unit/fixture/test_logging_error.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1449 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/tests/unit/fixture/test_setlevel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2966 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/tests/unit/test_convert_json.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1998 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/tests/unit/test_custom_loghandler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/tests/unit/test_formatters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2775 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/tests/unit/test_helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    76394 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/tests/unit/test_log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6603 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/tests/unit/test_pipe_mutex.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3767 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/tests/unit/test_rate_limit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14051 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/tests/unit/test_versionutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      688 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10409 2024-05-23 08:14:12.000000 oslo.log-6.0.0/oslo_log/versionutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.443385 oslo.log-6.0.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.463392 oslo.log-6.0.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/add-context-section-0b2f411ec64f42f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/add-facility-to-journal-e10bf7002cc19dd3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/add-reno-e4fedb11ece56f1e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/add-system_scope-to-logging_user_identity_format-0581ce5070740375.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      381 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/always-add-error-text-715022964364ffa0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/deprecate-watch-log-file-ba9524ae872e7c01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/deprecate-windows-support-75e6ac72310d5e72.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/drop-python27-support-0fe4909a5468feb3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/info-logging-7b7be9fc7a95aebc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/init-global-request-id-eb2031bc221e5fb7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/is_debug_enabled-d7afee4c811a46df.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/jsonformatter-repr-fd616eb6fa6caeb3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/log-global_request_id-f97e6d663e8a80b3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/log-rotation-595f8232cd987a6d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/native-threads-logging-cc84f7288c4835a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/reload_log_config-743817192b1172b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/remove-log-format-b4b949701cee3315.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/remove-syslog-rfc-format-7a06772c0bb48e9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/remove-verbose-option-d0d1381e182d1be1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/systemd-journal-support-fcbc34b3c5ce93ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/use-json-option-96f71da54a3b9a18.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/use-project-in-user-identity-93fd6e0a2e434a6f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/use_stderr_default_false-50d846b88cf2be90.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/notes/windows-eventlog-2beb0a6010e342eb.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.467394 oslo.log-6.0.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.467394 oslo.log-6.0.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.467394 oslo.log-6.0.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/liberty.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.443385 oslo.log-6.0.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.443385 oslo.log-6.0.0/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.467394 oslo.log-6.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10738 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.443385 oslo.log-6.0.0/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:14:42.467394 oslo.log-6.0.0/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-23 08:14:12.000000 oslo.log-6.0.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-05-23 08:14:12.000000 oslo.log-6.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2024-05-23 08:14:42.471395 oslo.log-6.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-05-23 08:14:12.000000 oslo.log-6.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2024-05-23 08:14:12.000000 oslo.log-6.0.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1574 2024-05-23 08:14:12.000000 oslo.log-6.0.0/tox.ini
```

### Comparing `oslo.log-5.5.1/.pre-commit-config.yaml` & `oslo.log-6.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/.zuul.yaml` & `oslo.log-6.0.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/AUTHORS` & `oslo.log-6.0.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/CONTRIBUTING.rst` & `oslo.log-6.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/ChangeLog` & `oslo.log-6.0.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 CHANGES
 =======
 
-5.5.1
+6.0.0
 -----
 
+* Remove unused pyinotify
+* Remove old excludes
+* Remove implementation for watch\_log\_file
+* Apply eventlet workaround only once
+* Deprecate watch\_log\_file
+* Remove fallback for old oslo.context
+* Fix broken reference to rate\_limit\_except\_level
+* Validate rate\_limit\_except\_level by choices
+* Imported Translations from Zanata
 * Fix eventlet detection
-* Update TOX\_CONSTRAINTS\_FILE for stable/2024.1
-* Update .gitreview for stable/2024.1
+* Update master for stable/2024.1
+* reno: Update master for unmaintained/victoria
 
 5.5.0
 -----
 
 * pre-commit: Integrate bandit
 * pre-commit: Bump versions
 * Bump hacking
```

### Comparing `oslo.log-5.5.1/LICENSE` & `oslo.log-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/PKG-INFO` & `oslo.log-6.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslo.log
-Version: 5.5.1
+Version: 6.0.0
 Summary: oslo.log library
 Home-page: https://docs.openstack.org/oslo.log/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `oslo.log-5.5.1/README.rst` & `oslo.log-6.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/admin/advanced_config.rst` & `oslo.log-6.0.0/doc/source/admin/advanced_config.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/admin/example_nova.rst` & `oslo.log-6.0.0/doc/source/admin/example_nova.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/admin/journal.rst` & `oslo.log-6.0.0/doc/source/admin/journal.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/admin/log_rotation.rst` & `oslo.log-6.0.0/doc/source/admin/log_rotation.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/admin/nova_sample.conf` & `oslo.log-6.0.0/doc/source/admin/nova_sample.conf`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/conf.py` & `oslo.log-6.0.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/configuration/index.rst` & `oslo.log-6.0.0/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/index.rst` & `oslo.log-6.0.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/user/examples/_i18n.py` & `oslo.log-6.0.0/doc/source/user/examples/_i18n.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/user/examples/oslo_logging.py` & `oslo.log-6.0.0/doc/source/user/examples/oslo_logging.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/user/examples/python_logging.py` & `oslo.log-6.0.0/doc/source/user/examples/python_logging.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/user/examples/usage.py` & `oslo.log-6.0.0/doc/source/user/examples/usage.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/user/examples/usage_context.py` & `oslo.log-6.0.0/doc/source/user/examples/usage_context.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/user/examples/usage_helper.py` & `oslo.log-6.0.0/doc/source/user/examples/usage_helper.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/user/examples.rst` & `oslo.log-6.0.0/doc/source/user/examples.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/user/guidelines.rst` & `oslo.log-6.0.0/doc/source/user/guidelines.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/doc/source/user/usage.rst` & `oslo.log-6.0.0/doc/source/user/usage.rst`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo.log.egg-info/PKG-INFO` & `oslo.log-6.0.0/oslo.log.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslo.log
-Version: 5.5.1
+Version: 6.0.0
 Summary: oslo.log library
 Home-page: https://docs.openstack.org/oslo.log/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `oslo.log-5.5.1/oslo.log.egg-info/SOURCES.txt` & `oslo.log-6.0.0/oslo.log.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 doc/source/reference/fixtures.rst
 doc/source/reference/formatters.rst
 doc/source/reference/handlers.rst
 doc/source/reference/helpers.rst
 doc/source/reference/index.rst
 doc/source/reference/log.rst
 doc/source/reference/versionutils.rst
-doc/source/reference/watchers.rst
 doc/source/user/examples.rst
 doc/source/user/guidelines.rst
 doc/source/user/history.rst
 doc/source/user/index.rst
 doc/source/user/usage.rst
 doc/source/user/examples/_i18n.py
 doc/source/user/examples/oslo_logging.py
@@ -60,15 +59,14 @@
 oslo_log/handlers.py
 oslo_log/helpers.py
 oslo_log/log.py
 oslo_log/pipe_mutex.py
 oslo_log/rate_limit.py
 oslo_log/version.py
 oslo_log/versionutils.py
-oslo_log/watchers.py
 oslo_log/cmds/__init__.py
 oslo_log/cmds/convert_json.py
 oslo_log/fixture/__init__.py
 oslo_log/fixture/logging_error.py
 oslo_log/fixture/setlevel.py
 oslo_log/locale/de/LC_MESSAGES/oslo_log.po
 oslo_log/locale/en_GB/LC_MESSAGES/oslo_log.po
@@ -89,14 +87,15 @@
 oslo_log/tests/unit/fixture/test_setlevel.py
 releasenotes/notes/.placeholder
 releasenotes/notes/add-context-section-0b2f411ec64f42f6.yaml
 releasenotes/notes/add-facility-to-journal-e10bf7002cc19dd3.yaml
 releasenotes/notes/add-reno-e4fedb11ece56f1e.yaml
 releasenotes/notes/add-system_scope-to-logging_user_identity_format-0581ce5070740375.yaml
 releasenotes/notes/always-add-error-text-715022964364ffa0.yaml
+releasenotes/notes/deprecate-watch-log-file-ba9524ae872e7c01.yaml
 releasenotes/notes/deprecate-windows-support-75e6ac72310d5e72.yaml
 releasenotes/notes/drop-python27-support-0fe4909a5468feb3.yaml
 releasenotes/notes/info-logging-7b7be9fc7a95aebc.yaml
 releasenotes/notes/init-global-request-id-eb2031bc221e5fb7.yaml
 releasenotes/notes/is_debug_enabled-d7afee4c811a46df.yaml
 releasenotes/notes/jsonformatter-repr-fd616eb6fa6caeb3.yaml
 releasenotes/notes/log-global_request_id-f97e6d663e8a80b3.yaml
@@ -109,14 +108,15 @@
 releasenotes/notes/systemd-journal-support-fcbc34b3c5ce93ec.yaml
 releasenotes/notes/use-json-option-96f71da54a3b9a18.yaml
 releasenotes/notes/use-project-in-user-identity-93fd6e0a2e434a6f.yaml
 releasenotes/notes/use_stderr_default_false-50d846b88cf2be90.yaml
 releasenotes/notes/windows-eventlog-2beb0a6010e342eb.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/liberty.rst
 releasenotes/source/mitaka.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
```

### Comparing `oslo.log-5.5.1/oslo_log/_i18n.py` & `oslo.log-6.0.0/oslo_log/_i18n.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/_options.py` & `oslo.log-6.0.0/oslo_log/_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,18 @@
     cfg.StrOpt('log-dir',
                deprecated_name='logdir',
                help='(Optional) The base directory used for relative log_file '
                     ' paths. '
                     + _IGNORE_MESSAGE),
     cfg.BoolOpt('watch-log-file',
                 default=False,
+                deprecated_for_removal=True,
+                deprecated_reason=('This function is known to have bene '
+                                   'broken for long time, and depends on '
+                                   'the unmaintained library'),
                 help='Uses logging handler designed to watch file '
                      'system. When log file is moved or removed this handler '
                      'will open a new log file with specified path '
                      'instantaneously. It makes sense only if log_file option '
                      'is specified and Linux platform is used. '
                      + _IGNORE_MESSAGE),
     cfg.BoolOpt('use-syslog',
@@ -199,16 +203,16 @@
                help='Interval, number of seconds, of log rate limiting.'),
     cfg.IntOpt('rate_limit_burst',
                default=0,
                help='Maximum number of logged messages per '
                     'rate_limit_interval.'),
     cfg.StrOpt('rate_limit_except_level',
                default='CRITICAL',
-               help='Log level name used by rate limiting: CRITICAL, ERROR, '
-                    'INFO, WARNING, DEBUG or empty string. Logs with level '
+               choices=['CRITICAL', 'ERROR', 'INFO', 'WARNING', 'DEBUG', ''],
+               help='Log level name used by rate limiting. Logs with level '
                     'greater or equal to rate_limit_except_level are not '
                     'filtered. An empty string means that all levels are '
                     'filtered.'),
 ]
 
 
 def list_opts():
```

### Comparing `oslo.log-5.5.1/oslo_log/cmds/convert_json.py` & `oslo.log-6.0.0/oslo_log/cmds/convert_json.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/fixture/__init__.py` & `oslo.log-6.0.0/oslo_log/fixture/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/fixture/logging_error.py` & `oslo.log-6.0.0/oslo_log/fixture/logging_error.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/fixture/setlevel.py` & `oslo.log-6.0.0/oslo_log/fixture/setlevel.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/formatters.py` & `oslo.log-6.0.0/oslo_log/formatters.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import datetime
-import debtcollector
 import functools
 import io
 import itertools
 import logging
 import logging.config
 import logging.handlers
 import re
@@ -29,21 +28,14 @@
 from oslo_serialization import jsonutils
 from oslo_utils import encodeutils
 
 
 def _dictify_context(context):
     if getattr(context, 'get_logging_values', None):
         return context.get_logging_values()
-    elif getattr(context, 'to_dict', None):
-        debtcollector.deprecate(
-            'The RequestContext.get_logging_values() '
-            'method should be defined for logging context specific '
-            'information.  The to_dict() method is deprecated '
-            'for oslo.log use.', version='3.8.0', removal_version='5.0.0')
-        return context.to_dict()
     # This dict only style logging format will become deprecated
     # when projects using a dictionary object for context are updated
     elif isinstance(context, dict):
         return context
 
     return {}
```

### Comparing `oslo.log-5.5.1/oslo_log/handlers.py` & `oslo.log-6.0.0/oslo_log/handlers.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/helpers.py` & `oslo.log-6.0.0/oslo_log/helpers.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/locale/de/LC_MESSAGES/oslo_log.po` & `oslo.log-6.0.0/oslo_log/locale/de/LC_MESSAGES/oslo_log.po`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/locale/en_GB/LC_MESSAGES/oslo_log.po` & `oslo.log-6.0.0/oslo_log/locale/en_GB/LC_MESSAGES/oslo_log.po`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/locale/es/LC_MESSAGES/oslo_log.po` & `oslo.log-6.0.0/oslo_log/locale/es/LC_MESSAGES/oslo_log.po`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/locale/ja/LC_MESSAGES/oslo_log.po` & `oslo.log-6.0.0/oslo_log/locale/ja/LC_MESSAGES/oslo_log.po`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/log.py` & `oslo.log-6.0.0/oslo_log/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,16 @@
     'minutes': 'm',
     'hours': 'h',
     'days': 'd',
     'weekday': 'w',
     'midnight': 'midnight'
 }
 
+_EVENTLET_FIX_APPLIED = False
+
 
 def _get_log_file_path(conf, binary=None):
     logfile = conf.log_file
     logdir = conf.log_dir
 
     if logfile and not logdir:
         return logfile
@@ -268,21 +270,24 @@
 
 def _fix_eventlet_logging():
     """Properly setup logging with eventlet on native threads.
 
     Workaround for: https://github.com/eventlet/eventlet/issues/432
     """
 
+    global _EVENTLET_FIX_APPLIED
+
     # If eventlet was not loaded before call to setup assume it's not used.
-    if eventletutils.is_monkey_patched('thread'):
+    if eventletutils.is_monkey_patched('thread') and not _EVENTLET_FIX_APPLIED:
         import eventlet.green.threading
         from oslo_log import pipe_mutex
         logging.threading = eventlet.green.threading
         logging._lock = logging.threading.RLock()
         logging.Handler.createLock = pipe_mutex.pipe_createLock
+        _EVENTLET_FIX_APPLIED = True
 
 
 def setup(conf, product_name, version='unknown', *, fix_eventlet=True):
     """Setup logging for the current application."""
     if fix_eventlet:
         _fix_eventlet_logging()
     if conf.log_config_append:
@@ -368,18 +373,17 @@
     # Remove all handlers
     for handler in list(log_root.handlers):
         log_root.removeHandler(handler)
 
     logpath = _get_log_file_path(conf)
     if logpath:
         # On Windows, in-use files cannot be moved or deleted.
-        if conf.watch_log_file and platform.system() == 'Linux':
-            from oslo_log import watchers
-            file_handler = watchers.FastWatchedFileHandler
-            filelog = file_handler(logpath)
+        if conf.watch_log_file:
+            raise RuntimeError('watch_log_file feature was removed because '
+                               'it has been broken for multiple releases.')
         elif conf.log_rotation_type.lower() == "interval":
             file_handler = logging.handlers.TimedRotatingFileHandler
             when = conf.log_rotate_interval_type.lower()
             interval_type = LOG_ROTATE_INTERVAL_MAPPING[when]
             # When weekday is configured, "when" has to be a value between
             # 'w0'-'w6' (w0 for Monday, w1 for Tuesday, and so on)'
             if interval_type == 'w':
@@ -468,15 +472,15 @@
         else:
             logger.setLevel(level_name)
 
     if conf.rate_limit_burst >= 1 and conf.rate_limit_interval >= 1:
         from oslo_log import rate_limit
         rate_limit.install_filter(conf.rate_limit_burst,
                                   conf.rate_limit_interval,
-                                  conf.rate_limit_except)
+                                  conf.rate_limit_except_level)
 
 
 _loggers = {}
 
 
 def get_loggers():
     """Return a copy of the oslo loggers dictionary."""
```

### Comparing `oslo.log-5.5.1/oslo_log/pipe_mutex.py` & `oslo.log-6.0.0/oslo_log/pipe_mutex.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/rate_limit.py` & `oslo.log-6.0.0/oslo_log/rate_limit.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/tests/unit/__init__.py` & `oslo.log-6.0.0/oslo_log/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/tests/unit/fixture/__init__.py` & `oslo.log-6.0.0/oslo_log/tests/unit/fixture/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/tests/unit/fixture/test_logging_error.py` & `oslo.log-6.0.0/oslo_log/tests/unit/fixture/test_logging_error.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/tests/unit/fixture/test_setlevel.py` & `oslo.log-6.0.0/oslo_log/tests/unit/fixture/test_setlevel.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/tests/unit/test_convert_json.py` & `oslo.log-6.0.0/oslo_log/tests/unit/test_convert_json.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/tests/unit/test_custom_loghandler.py` & `oslo.log-6.0.0/oslo_log/tests/unit/test_custom_loghandler.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/tests/unit/test_formatters.py` & `oslo.log-6.0.0/oslo_log/tests/unit/test_formatters.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 
 """Unit Tests for oslo.log formatter"""
 
 import logging
 import sys
-from unittest import mock
 
 from oslo_config import cfg
 from oslo_config import fixture as config_fixture
 from oslo_context import context
 from oslotest import base as test_base
 
 from oslo_log import formatters
@@ -33,25 +32,14 @@
                                   project_domain_id="pdomain",
                                   user_domain_id="udomain",
                                   overwrite=True)
 
     return ctxt
 
 
-class AlternativeRequestContext(object):
-
-    def __init__(self, user=None, tenant=None):
-        self.user = user
-        self.tenant = tenant
-
-    def to_dict(self):
-        return {'user': self.user,
-                'tenant': self.tenant}
-
-
 class FormatterTest(test_base.BaseTestCase):
 
     def setUp(self):
         super(FormatterTest, self).setUp()
 
     def test_replace_false_value_exists(self):
         d = {"user": "user1"}
@@ -62,37 +50,22 @@
         d = {"user": "user1"}
         s = "%(project)s" % formatters._ReplaceFalseValue(d)
         self.assertEqual("-", s)
 
     def test_dictify_context_empty(self):
         self.assertEqual({}, formatters._dictify_context(None))
 
-    @mock.patch("debtcollector.deprecate")
-    def test_dictify_context_with_dict(self, mock_deprecate):
+    def test_dictify_context_with_dict(self):
         d = {"user": "user"}
         self.assertEqual(d, formatters._dictify_context(d))
-        mock_deprecate.assert_not_called()
 
-    @mock.patch("debtcollector.deprecate")
-    def test_dictify_context_with_context(self, mock_deprecate):
+    def test_dictify_context_with_context(self):
         ctxt = _fake_context()
         self.assertEqual(ctxt.get_logging_values(),
                          formatters._dictify_context(ctxt))
-        mock_deprecate.assert_not_called()
-
-    @mock.patch("debtcollector.deprecate")
-    def test_dictify_context_without_get_logging_values(self, mock_deprecate):
-        ctxt = AlternativeRequestContext(user="user", tenant="tenant")
-        d = {"user": "user", "tenant": "tenant"}
-        self.assertEqual(d, formatters._dictify_context(ctxt))
-        mock_deprecate.assert_called_with(
-            'The RequestContext.get_logging_values() '
-            'method should be defined for logging context specific '
-            'information.  The to_dict() method is deprecated '
-            'for oslo.log use.', removal_version='5.0.0', version='3.8.0')
 
 
 # Test for https://bugs.python.org/issue28603
 class FormatUnhashableExceptionTest(test_base.BaseTestCase):
     def setUp(self):
         super(FormatUnhashableExceptionTest, self).setUp()
         self.config_fixture = self.useFixture(
```

### Comparing `oslo.log-5.5.1/oslo_log/tests/unit/test_helpers.py` & `oslo.log-6.0.0/oslo_log/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/tests/unit/test_log.py` & `oslo.log-6.0.0/oslo_log/tests/unit/test_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 from contextlib import contextmanager
 import copy
 import datetime
 import io
 import logging
 import os
-import platform
 import shutil
 import sys
 try:
     import syslog
 except ImportError:
     syslog = None
 try:
@@ -150,32 +149,14 @@
     def test_eventlog(self, loggers_mock, handler_mock, platform_mock):
         self.config(use_eventlog=True)
         log._setup_logging_from_conf(self.CONF, 'test', 'test')
         handler_mock.assert_called_once_with('test')
         mock_logger = loggers_mock.return_value.logger
         mock_logger.addHandler.assert_any_call(handler_mock.return_value)
 
-    @mock.patch('oslo_log.watchers.FastWatchedFileHandler')
-    @mock.patch('oslo_log.log._get_log_file_path', return_value='test.conf')
-    @mock.patch('platform.system', return_value='Linux')
-    def test_watchlog_on_linux(self, platfotm_mock, path_mock, handler_mock):
-        self.config(watch_log_file=True)
-        log._setup_logging_from_conf(self.CONF, 'test', 'test')
-        handler_mock.assert_called_once_with(path_mock.return_value)
-        self.assertEqual(self.log_handlers[0], handler_mock.return_value)
-
-    @mock.patch('logging.handlers.WatchedFileHandler')
-    @mock.patch('oslo_log.log._get_log_file_path', return_value='test.conf')
-    @mock.patch('platform.system', return_value='Windows')
-    def test_watchlog_on_windows(self, platform_mock, path_mock, handler_mock):
-        self.config(watch_log_file=True)
-        log._setup_logging_from_conf(self.CONF, 'test', 'test')
-        handler_mock.assert_called_once_with(path_mock.return_value)
-        self.assertEqual(self.log_handlers[0], handler_mock.return_value)
-
     @mock.patch('logging.handlers.TimedRotatingFileHandler')
     @mock.patch('oslo_log.log._get_log_file_path', return_value='test.conf')
     def test_timed_rotate_log(self, path_mock, handler_mock):
         rotation_type = 'interval'
         when = 'weekday'
         interval = 2
         backup_count = 2
@@ -1359,62 +1340,14 @@
 
     def test_log_file_defaults_to_none(self):
         log.set_defaults()
         self.conf([])
         self.assertIsNone(self.conf.log_file)
 
 
-@testtools.skipIf(platform.system() != 'Linux',
-                  'pyinotify library works on Linux platform only.')
-class FastWatchedFileHandlerTestCase(BaseTestCase):
-
-    def setUp(self):
-        super(FastWatchedFileHandlerTestCase, self).setUp()
-
-    def _config(self):
-        os_level, log_path = tempfile.mkstemp()
-        log_dir_path = os.path.dirname(log_path)
-        log_file_path = os.path.basename(log_path)
-        self.CONF(['--log-dir', log_dir_path, '--log-file', log_file_path])
-        self.config(use_stderr=False)
-        self.config(watch_log_file=True)
-        log.setup(self.CONF, 'test', 'test')
-        return log_path
-
-    def test_instantiate(self):
-        self._config()
-        logger = log._loggers[None].logger
-        self.assertEqual(1, len(logger.handlers))
-        from oslo_log import watchers
-        self.assertIsInstance(logger.handlers[0],
-                              watchers.FastWatchedFileHandler)
-
-    def test_log(self):
-        log_path = self._config()
-        logger = log._loggers[None].logger
-        text = 'Hello World!'
-        logger.info(text)
-        with open(log_path, 'r') as f:
-            file_content = f.read()
-        self.assertIn(text, file_content)
-
-    def test_move(self):
-        log_path = self._config()
-        os_level_dst, log_path_dst = tempfile.mkstemp()
-        os.rename(log_path, log_path_dst)
-        time.sleep(6)
-        self.assertTrue(os.path.exists(log_path))
-
-    def test_remove(self):
-        log_path = self._config()
-        os.remove(log_path)
-        time.sleep(6)
-        self.assertTrue(os.path.exists(log_path))
-
-
 class MutateTestCase(BaseTestCase):
     def setUp(self):
         super(MutateTestCase, self).setUp()
         if hasattr(log._load_log_config, 'old_time'):
             del log._load_log_config.old_time
 
     def setup_confs(self, *confs):
```

### Comparing `oslo.log-5.5.1/oslo_log/tests/unit/test_pipe_mutex.py` & `oslo.log-6.0.0/oslo_log/tests/unit/test_pipe_mutex.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/tests/unit/test_rate_limit.py` & `oslo.log-6.0.0/oslo_log/tests/unit/test_rate_limit.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/tests/unit/test_versionutils.py` & `oslo.log-6.0.0/oslo_log/tests/unit/test_versionutils.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/version.py` & `oslo.log-6.0.0/oslo_log/version.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/oslo_log/versionutils.py` & `oslo.log-6.0.0/oslo_log/versionutils.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/releasenotes/source/conf.py` & `oslo.log-6.0.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `oslo.log-6.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Andi Chandler <andi@gowling.com>, 2020. #zanata
 # Andi Chandler <andi@gowling.com>, 2022. #zanata
 # Andi Chandler <andi@gowling.com>, 2023. #zanata
 msgid ""
 msgstr ""
 "Project-Id-Version: oslo.log\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-05-05 13:36+0000\n"
+"POT-Creation-Date: 2024-03-26 18:32+0000\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "PO-Revision-Date: 2023-05-09 12:01+0000\n"
 "Last-Translator: Andi Chandler <andi@gowling.com>\n"
 "Language-Team: English (United Kingdom)\n"
 "Language: en_GB\n"
@@ -84,14 +84,17 @@
 
 msgid "4.8.0"
 msgstr "4.8.0"
 
 msgid "5.0.0"
 msgstr "5.0.0"
 
+msgid "5.0.1"
+msgstr "5.0.1"
+
 msgid "5.2.0"
 msgstr "5.2.0"
 
 msgid ""
 "A new ``oslo_log.log.is_debug_enabled`` helper function is added that allows "
 "to determine whether debug mode is enabled for logging."
 msgstr ""
@@ -308,9 +311,16 @@
 msgid ""
 "When removing the \"verbose\" option, the default logging level was set to "
 "\"WARNING\" by mistake. Fixed it back to \"INFO\"."
 msgstr ""
 "When removing the \"verbose\" option, the default logging level was set to "
 "\"WARNING\" by mistake. Fixed it back to \"INFO\"."
 
+msgid ""
+"`Bug #1983863 <https://bugs.launchpad.net/oslo.log/+bug/1983863>`_: Fixed "
+"logging in eventlet native threads."
+msgstr ""
+"`Bug #1983863 <https://bugs.launchpad.net/oslo.log/+bug/1983863>`_: Fixed "
+"logging in eventlet native threads."
+
 msgid "oslo.log Release Notes"
 msgstr "oslo.log Release Notes"
```

### Comparing `oslo.log-5.5.1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `oslo.log-6.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/setup.cfg` & `oslo.log-6.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `oslo.log-5.5.1/setup.py` & `oslo.log-6.0.0/setup.py`

 * *Files identical despite different names*

