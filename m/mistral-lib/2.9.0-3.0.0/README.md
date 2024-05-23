# Comparing `tmp/mistral-lib-2.9.0.tar.gz` & `tmp/mistral-lib-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistral-lib-2.9.0.tar", last modified: Thu Sep  7 10:00:14 2023, max compression
+gzip compressed data, was "mistral-lib-3.0.0.tar", last modified: Thu May 23 08:03:20 2024, max compression
```

## Comparing `mistral-lib-2.9.0.tar` & `mistral-lib-3.0.0.tar`

### file list

```diff
@@ -1,93 +1,96 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.902747 mistral-lib-2.9.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1522 2023-09-07 10:00:14.000000 mistral-lib-2.9.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5698 2023-09-07 10:00:14.000000 mistral-lib-2.9.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2128 2023-09-07 10:00:14.902747 mistral-lib-2.9.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      973 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.894747 mistral-lib-2.9.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.894747 mistral-lib-2.9.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2591 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.894747 mistral-lib-2.9.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1532 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/doc/source/contributor/creating_custom_actions.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.894747 mistral-lib-2.9.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.894747 mistral-lib-2.9.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.894747 mistral-lib-2.9.0/mistral_lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      667 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.898747 mistral-lib-2.9.0/mistral_lib/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/actions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12622 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/actions/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4035 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/actions/context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.898747 mistral-lib-2.9.0/mistral_lib/actions/providers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/actions/providers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3303 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/actions/providers/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1773 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/actions/providers/composite.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2078 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/actions/providers/python.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2503 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/actions/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2853 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6307 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/serialization.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.898747 mistral-lib-2.9.0/mistral_lib/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.898747 mistral-lib-2.9.0/mistral_lib/tests/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/tests/actions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3833 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/tests/actions/test_action_providers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/tests/actions/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3229 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/tests/actions/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2703 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/tests/test_inspect_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3518 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/tests/test_serialization.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10036 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/tests/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.898747 mistral-lib-2.9.0/mistral_lib/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14591 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2344 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/utils/inspect_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.898747 mistral-lib-2.9.0/mistral_lib/yaql/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/yaql/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.898747 mistral-lib-2.9.0/mistral_lib/yaql/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/mistral_lib/yaql/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.898747 mistral-lib-2.9.0/mistral_lib.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2128 2023-09-07 10:00:14.000000 mistral-lib-2.9.0/mistral_lib.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2145 2023-09-07 10:00:14.000000 mistral-lib-2.9.0/mistral_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-09-07 10:00:14.000000 mistral-lib-2.9.0/mistral_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-09-07 10:00:14.000000 mistral-lib-2.9.0/mistral_lib.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-09-07 10:00:14.000000 mistral-lib-2.9.0/mistral_lib.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-09-07 10:00:14.000000 mistral-lib-2.9.0/mistral_lib.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-09-07 10:00:14.000000 mistral-lib-2.9.0/mistral_lib.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.894747 mistral-lib-2.9.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.898747 mistral-lib-2.9.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/notes/action_providers-54a50a4d629016ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/notes/mask-password-6899d868d213f722.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/notes/rename-task-id-to-task-execution-id-f17d671fcef0127a.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.902747 mistral-lib-2.9.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.902747 mistral-lib-2.9.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-07 10:00:14.902747 mistral-lib-2.9.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8966 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1157 2023-09-07 10:00:14.902747 mistral-lib-2.9.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1683 2023-09-07 09:59:46.000000 mistral-lib-2.9.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.048920 mistral-lib-3.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1595 2024-05-23 08:03:19.000000 mistral-lib-3.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6129 2024-05-23 08:03:19.000000 mistral-lib-3.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2130 2024-05-23 08:03:20.048920 mistral-lib-3.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      973 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.036918 mistral-lib-3.0.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.036918 mistral-lib-3.0.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2591 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.036918 mistral-lib-3.0.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1532 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/doc/source/contributor/creating_custom_actions.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.036918 mistral-lib-3.0.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.036918 mistral-lib-3.0.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.036918 mistral-lib-3.0.0/mistral_lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      667 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.036918 mistral-lib-3.0.0/mistral_lib/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/actions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12622 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/actions/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4365 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/actions/context.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.036918 mistral-lib-3.0.0/mistral_lib/actions/providers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/actions/providers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3303 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/actions/providers/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1773 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/actions/providers/composite.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2078 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/actions/providers/python.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2503 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/actions/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2853 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6307 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/serialization.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.044920 mistral-lib-3.0.0/mistral_lib/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.044920 mistral-lib-3.0.0/mistral_lib/tests/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/tests/actions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3833 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/tests/actions/test_action_providers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/tests/actions/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3321 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/tests/actions/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2703 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/tests/test_inspect_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3518 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/tests/test_serialization.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10036 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/tests/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.044920 mistral-lib-3.0.0/mistral_lib/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14591 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2344 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/utils/inspect_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.044920 mistral-lib-3.0.0/mistral_lib/yaql/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/yaql/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.044920 mistral-lib-3.0.0/mistral_lib/yaql/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/mistral_lib/yaql/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.036918 mistral-lib-3.0.0/mistral_lib.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2130 2024-05-23 08:03:19.000000 mistral-lib-3.0.0/mistral_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2238 2024-05-23 08:03:20.000000 mistral-lib-3.0.0/mistral_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:03:19.000000 mistral-lib-3.0.0/mistral_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:03:19.000000 mistral-lib-3.0.0/mistral_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-23 08:03:19.000000 mistral-lib-3.0.0/mistral_lib.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2024-05-23 08:03:19.000000 mistral-lib-3.0.0/mistral_lib.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2024-05-23 08:03:19.000000 mistral-lib-3.0.0/mistral_lib.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.032918 mistral-lib-3.0.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.044920 mistral-lib-3.0.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/notes/action_providers-54a50a4d629016ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/notes/mask-password-6899d868d213f722.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/notes/rename-task-id-to-task-execution-id-f17d671fcef0127a.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.048920 mistral-lib-3.0.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.048920 mistral-lib-3.0.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:20.048920 mistral-lib-3.0.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8966 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1159 2024-05-23 08:03:20.048920 mistral-lib-3.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1683 2024-05-23 08:02:37.000000 mistral-lib-3.0.0/tox.ini
```

### Comparing `mistral-lib-2.9.0/AUTHORS` & `mistral-lib-3.0.0/AUTHORS`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 Eyal <eyal.bar-ilan@nokia.com>
 Flavio Percoco <flaper87@gmail.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Hervé Beraud <hberaud@redhat.com>
 Ifat Afek <ifat.afek@nokia.com>
 Monty Taylor <mordred@inaugust.com>
 Nguyen Hai <nguyentrihai93@gmail.com>
+Oleg Ovcharuk <vgvoleg@gmail.com>
 OpenStack Release Bot <infra-root@openstack.org>
 Renat Akhmerov <renat.akhmerov@gmail.com>
 Ryan Brady <rbrady@redhat.com>
 Sean McGinnis <sean.mcginnis@gmail.com>
 Sharat Sharma <sharat.sharma@nectechnologies.in>
 Takashi Kajinami <tkajinam@redhat.com>
+Vadim Zelenevsky <wortellen@gmail.com>
 Vieri <15050873171@163.com>
 ZhijunWei <wzj334965317@outlook.com>
 ali <maxget7@gmail.com>
 caoyuan <cao.yuan@99cloud.net>
 cuiweibo <cuiweibo@inspur.com>
 guotao <guotao.bj@inspur.com>
 huang.zhiping <huang.zhiping@99cloud.net>
```

### Comparing `mistral-lib-2.9.0/CONTRIBUTING.rst` & `mistral-lib-3.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/ChangeLog` & `mistral-lib-3.0.0/ChangeLog`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 CHANGES
 =======
 
+3.0.0
+-----
+
+* reno: Update master for unmaintained/wallaby
+* reno: Update master for unmaintained/victoria
+* Headers propagation from an execution request to actions/notifications
+* New fields added to action execution context
+* Update master for stable/2024.1
+* reno: Update master for unmaintained/yoga
+* Update python classifier in setup.cfg
+
+2.10.0
+------
+
+* Update master for stable/2023.1
+* Update master for stable/2023.2
+
 2.9.0
 -----
 
 * Fix tox4 error
 * Switch to 2023.1 Python3 unit tests and generic template name
 * Update master for stable/zed
```

### Comparing `mistral-lib-2.9.0/LICENSE` & `mistral-lib-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/PKG-INFO` & `mistral-lib-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mistral-lib
-Version: 2.9.0
+Version: 3.0.0
 Summary: Mistral shared routings and utilities (Actions API, YAQL functions API, data types etc.)
 Home-page: https://docs.openstack.org/mistral/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -43,12 +43,12 @@
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
```

### Comparing `mistral-lib-2.9.0/README.rst` & `mistral-lib-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/doc/source/conf.py` & `mistral-lib-3.0.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/doc/source/contributor/creating_custom_actions.rst` & `mistral-lib-3.0.0/doc/source/contributor/creating_custom_actions.rst`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/doc/source/index.rst` & `mistral-lib-3.0.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/__init__.py` & `mistral-lib-3.0.0/mistral_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/actions/__init__.py` & `mistral-lib-3.0.0/mistral_lib/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/actions/base.py` & `mistral-lib-3.0.0/mistral_lib/actions/base.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/actions/context.py` & `mistral-lib-3.0.0/mistral_lib/actions/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,24 +65,29 @@
         self.user_name = user_name
         self.auth_token = auth_token
 
 
 class ExecutionContext(object):
     def __init__(self, workflow_execution_id=None, task_execution_id=None,
                  action_execution_id=None, workflow_name=None,
-                 callback_url=None, task_id=None):
+                 callback_url=None, task_id=None, with_items_index=0,
+                 task_rerun_no=0, task_rerun_id=None,
+                 workflow_propagated_headers=None):
         self.workflow_execution_id = workflow_execution_id
         self.task_execution_id = task_execution_id
         self.action_execution_id = action_execution_id
         self.workflow_name = workflow_name
         self.callback_url = callback_url
+        self.with_items_index = with_items_index
+        self.task_rerun_no = task_rerun_no
+        self.task_rerun_id = task_rerun_id
+        self.workflow_propagated_headers = workflow_propagated_headers
 
         if task_id is not None:
             self.task_execution_id = task_id
-
             self._deprecate_task_id_warning()
 
     def _deprecate_task_id_warning(self):
         warnings.warn(
             "context.execution.task_id was deprecated in the Queens cycle. "
             "Please use context.execution.task_execution_id. It will be "
             "removed in a future release.", DeprecationWarning
```

### Comparing `mistral-lib-2.9.0/mistral_lib/actions/providers/base.py` & `mistral-lib-3.0.0/mistral_lib/actions/providers/base.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/actions/providers/composite.py` & `mistral-lib-3.0.0/mistral_lib/actions/providers/composite.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/actions/providers/python.py` & `mistral-lib-3.0.0/mistral_lib/actions/providers/python.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/actions/types.py` & `mistral-lib-3.0.0/mistral_lib/actions/types.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/exceptions.py` & `mistral-lib-3.0.0/mistral_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/serialization.py` & `mistral-lib-3.0.0/mistral_lib/serialization.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/tests/actions/test_action_providers.py` & `mistral-lib-3.0.0/mistral_lib/tests/actions/test_action_providers.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/tests/actions/test_base.py` & `mistral-lib-3.0.0/mistral_lib/tests/actions/test_base.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/tests/actions/test_context.py` & `mistral-lib-3.0.0/mistral_lib/tests/actions/test_context.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,15 +29,18 @@
         project_id='project_id')
 
     execution_ctx = context.ExecutionContext(
         workflow_execution_id='workflow_execution_id',
         task_execution_id='task_execution_id',
         action_execution_id='action_execution_id',
         workflow_name='workflow_name',
-        callback_url='callback_url')
+        callback_url='callback_url',
+        with_items_index=0,
+        task_rerun_no=0,
+        task_rerun_id='task_rerun_id')
 
     return context.ActionContext(security_ctx, execution_ctx)
 
 
 class TestActionsBase(tests_base.TestCase):
 
     def test_empty_context(self):
```

### Comparing `mistral-lib-2.9.0/mistral_lib/tests/base.py` & `mistral-lib-3.0.0/mistral_lib/tests/base.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/tests/test_inspect_utils.py` & `mistral-lib-3.0.0/mistral_lib/tests/test_inspect_utils.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/tests/test_serialization.py` & `mistral-lib-3.0.0/mistral_lib/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/tests/test_utils.py` & `mistral-lib-3.0.0/mistral_lib/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/utils/__init__.py` & `mistral-lib-3.0.0/mistral_lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib/utils/inspect_utils.py` & `mistral-lib-3.0.0/mistral_lib/utils/inspect_utils.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/mistral_lib.egg-info/PKG-INFO` & `mistral-lib-3.0.0/mistral_lib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mistral-lib
-Version: 2.9.0
+Version: 3.0.0
 Summary: Mistral shared routings and utilities (Actions API, YAQL functions API, data types etc.)
 Home-page: https://docs.openstack.org/mistral/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -43,12 +43,12 @@
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
```

### Comparing `mistral-lib-2.9.0/mistral_lib.egg-info/SOURCES.txt` & `mistral-lib-3.0.0/mistral_lib.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,17 @@
 mistral_lib/utils/inspect_utils.py
 mistral_lib/yaql/__init__.py
 mistral_lib/yaql/api/__init__.py
 releasenotes/notes/.placeholder
 releasenotes/notes/action_providers-54a50a4d629016ce.yaml
 releasenotes/notes/mask-password-6899d868d213f722.yaml
 releasenotes/notes/rename-task-id-to-task-execution-id-f17d671fcef0127a.yaml
+releasenotes/source/2023.1.rst
+releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
 releasenotes/source/train.rst
```

### Comparing `mistral-lib-2.9.0/releasenotes/notes/action_providers-54a50a4d629016ce.yaml` & `mistral-lib-3.0.0/releasenotes/notes/action_providers-54a50a4d629016ce.yaml`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/releasenotes/source/conf.py` & `mistral-lib-3.0.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/setup.cfg` & `mistral-lib-3.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 name = mistral-lib
 summary = Mistral shared routings and utilities (Actions API, YAQL functions API, data types etc.)
 description_file = 
 	README.rst
 author = OpenStack
 author_email = openstack-discuss@lists.openstack.org
 home_page = https://docs.openstack.org/mistral/latest/
-python_requires = >=3.6
+python_requires = >=3.8
 classifier = 
 	Environment :: OpenStack
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [files]
 packages = 
 	mistral_lib
 
 [compile_catalog]
 directory = mistral-lib/locale
```

### Comparing `mistral-lib-2.9.0/setup.py` & `mistral-lib-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `mistral-lib-2.9.0/tox.ini` & `mistral-lib-3.0.0/tox.ini`

 * *Files identical despite different names*

