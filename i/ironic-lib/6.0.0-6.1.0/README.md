# Comparing `tmp/ironic-lib-6.0.0.tar.gz` & `tmp/ironic-lib-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ironic-lib-6.0.0.tar", last modified: Thu Feb 22 15:07:02 2024, max compression
+gzip compressed data, was "ironic-lib-6.1.0.tar", last modified: Thu May 23 08:03:34 2024, max compression
```

## Comparing `ironic-lib-6.0.0.tar` & `ironic-lib-6.1.0.tar`

### file list

```diff
@@ -1,102 +1,103 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.322915 ironic-lib-6.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9955 2024-02-22 15:07:02.000000 ironic-lib-6.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    83362 2024-02-22 15:07:01.000000 ironic-lib-6.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11325 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1782 2024-02-22 15:07:02.322915 ironic-lib-6.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2601 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/TESTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.306914 ironic-lib-6.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.306914 ironic-lib-6.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.306914 ironic-lib-6.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2860 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.310914 ironic-lib-6.0.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.302914 ironic-lib-6.0.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.302914 ironic-lib-6.0.0/etc/ironic/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.310914 ironic-lib-6.0.0/etc/ironic/rootwrap.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/etc/ironic/rootwrap.d/ironic-lib.filters
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/extra-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.314915 ironic-lib-6.0.0/ironic_lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7090 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/auth_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4960 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/capabilities.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.314915 ironic-lib-6.0.0/ironic_lib/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      750 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/common/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5705 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/disk_partitioner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27540 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/disk_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6995 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/exception.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.314915 ironic-lib-6.0.0/ironic_lib/json_rpc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3269 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/json_rpc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8597 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/json_rpc/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10295 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/json_rpc/server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7751 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12374 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/mdns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9649 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/metrics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4514 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/metrics_collector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3717 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/metrics_statsd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4186 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/metrics_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4428 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/qemu_img.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.318915 ironic-lib-6.0.0/ironic_lib/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3093 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3523 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8545 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/test_basic_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3339 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/test_capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9498 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/test_disk_partitioner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40979 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/test_disk_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2621 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29790 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/test_json_rpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5432 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/test_keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15499 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/test_mdns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7029 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/test_metrics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2546 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/test_metrics_collector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3807 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/test_metrics_statsd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4476 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/test_metrics_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7283 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/test_qemu_img.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35416 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/tests/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26544 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2395 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/ironic_lib/wsgi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.314915 ironic-lib-6.0.0/ironic_lib.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1782 2024-02-22 15:07:02.000000 ironic-lib-6.0.0/ironic_lib.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2863 2024-02-22 15:07:02.000000 ironic-lib-6.0.0/ironic_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:07:02.000000 ironic-lib-6.0.0/ironic_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2024-02-22 15:07:02.000000 ironic-lib-6.0.0/ironic_lib.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:07:02.000000 ironic-lib-6.0.0/ironic_lib.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-22 15:07:02.000000 ironic-lib-6.0.0/ironic_lib.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-02-22 15:07:02.000000 ironic-lib-6.0.0/ironic_lib.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2024-02-22 15:07:02.000000 ironic-lib-6.0.0/ironic_lib.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.302914 ironic-lib-6.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.322915 ironic-lib-6.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/add-additional-disk-conversion-retry-dfff93cbdf779f81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/add-metrics-collection-b9549ec62ce4feda.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/add-port-to-rpc-client-2f2f0cd60547843f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      738 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/basic-auth-middleware-e5af29651b2d7979.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/conver-str-to-bytes-11a665d0fa8828ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/drop-py-2-7-3c01e37309077c06.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/erase-tiny-partitions-c408a3a4afe60d44.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/extend-list-partitions-b71f81c77f6ecfdb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/fix-dd-async-gpt-erasure-bbc6b084b0344d30.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/fix-metadisk-partitioning-32d3fca274290dd6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/increase-efi-partition-size-9479d069b17804ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/json_rpc-allowed_roles-3bee50b5936c2be3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/remove-iscsi-verify-attempts-ff9eb5b7a28e6143.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/rescan-for-partition-write-out-3fbb92ae5c2a33c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/restore-centos7-compatibility-bfbe2bcf1d1fb7f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/releasenotes/notes/wipe-gpt-on-metadata-wipe-ac0a93b16e00893f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1711 2024-02-22 15:07:02.322915 ironic-lib-6.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2610 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:07:02.322915 ironic-lib-6.0.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1308 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/zuul.d/ironic-lib-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2024-02-22 15:06:31.000000 ironic-lib-6.0.0/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.477410 ironic-lib-6.1.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9992 2024-05-23 08:03:34.000000 ironic-lib-6.1.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    83450 2024-05-23 08:03:34.000000 ironic-lib-6.1.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11325 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1782 2024-05-23 08:03:34.477410 ironic-lib-6.1.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2601 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/TESTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.465408 ironic-lib-6.1.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.465408 ironic-lib-6.1.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.465408 ironic-lib-6.1.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2860 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.465408 ironic-lib-6.1.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.461408 ironic-lib-6.1.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.461408 ironic-lib-6.1.0/etc/ironic/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.465408 ironic-lib-6.1.0/etc/ironic/rootwrap.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/etc/ironic/rootwrap.d/ironic-lib.filters
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/extra-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.469409 ironic-lib-6.1.0/ironic_lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7090 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/auth_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4960 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/capabilities.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.469409 ironic-lib-6.1.0/ironic_lib/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      750 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/common/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5705 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/disk_partitioner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28453 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/disk_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6995 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/exception.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.473410 ironic-lib-6.1.0/ironic_lib/json_rpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3269 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/json_rpc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8597 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/json_rpc/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10295 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/json_rpc/server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7751 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12374 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/mdns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9649 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/metrics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4514 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/metrics_collector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3717 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/metrics_statsd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4186 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/metrics_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4428 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/qemu_img.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.473410 ironic-lib-6.1.0/ironic_lib/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3093 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3523 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8545 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/test_basic_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3339 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/test_capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9498 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/test_disk_partitioner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44011 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/test_disk_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2621 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29790 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/test_json_rpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5432 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/test_keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15499 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/test_mdns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7029 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/test_metrics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2546 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/test_metrics_collector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3807 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/test_metrics_statsd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4476 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/test_metrics_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7283 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/test_qemu_img.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35416 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/tests/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26544 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2395 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/ironic_lib/wsgi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.469409 ironic-lib-6.1.0/ironic_lib.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1782 2024-05-23 08:03:34.000000 ironic-lib-6.1.0/ironic_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2929 2024-05-23 08:03:34.000000 ironic-lib-6.1.0/ironic_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:03:34.000000 ironic-lib-6.1.0/ironic_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2024-05-23 08:03:34.000000 ironic-lib-6.1.0/ironic_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:03:34.000000 ironic-lib-6.1.0/ironic_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-23 08:03:34.000000 ironic-lib-6.1.0/ironic_lib.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-23 08:03:34.000000 ironic-lib-6.1.0/ironic_lib.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2024-05-23 08:03:34.000000 ironic-lib-6.1.0/ironic_lib.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.465408 ironic-lib-6.1.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.477410 ironic-lib-6.1.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/add-additional-disk-conversion-retry-dfff93cbdf779f81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/add-metrics-collection-b9549ec62ce4feda.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/add-port-to-rpc-client-2f2f0cd60547843f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      738 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/basic-auth-middleware-e5af29651b2d7979.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/conver-str-to-bytes-11a665d0fa8828ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/drop-py-2-7-3c01e37309077c06.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/erase-tiny-partitions-c408a3a4afe60d44.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/extend-list-partitions-b71f81c77f6ecfdb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/fix-dd-async-gpt-erasure-bbc6b084b0344d30.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/fix-metadisk-partitioning-32d3fca274290dd6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/increase-efi-partition-size-9479d069b17804ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/json_rpc-allowed_roles-3bee50b5936c2be3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/remove-iscsi-verify-attempts-ff9eb5b7a28e6143.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/rescan-for-partition-write-out-3fbb92ae5c2a33c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/restore-centos7-compatibility-bfbe2bcf1d1fb7f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/support-4096-sector-size-aa479b4040399975.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/releasenotes/notes/wipe-gpt-on-metadata-wipe-ac0a93b16e00893f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1711 2024-05-23 08:03:34.477410 ironic-lib-6.1.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2610 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:34.477410 ironic-lib-6.1.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1308 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/zuul.d/ironic-lib-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2024-05-23 08:02:50.000000 ironic-lib-6.1.0/zuul.d/project.yaml
```

### Comparing `ironic-lib-6.0.0/AUTHORS` & `ironic-lib-6.1.0/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,15 @@
 Takashi Kajinami <kajinamit@oss.nttdata.com>
 Takashi Kajinami <tkajinam@redhat.com>
 Tan Lin <tan.lin.good@gmail.com>
 Thierry Carrez <thierry@openstack.org>
 Thomas Bechtold <tbechtold@suse.com>
 Thomas Goirand <zigo@debian.org>
 Tom Fifield <tom@openstack.org>
+Tudor Domnescu <tdomnesc@redhat.com>
 Tushar Kalra <tushar@cloudscaling.com>
 Uros Orozel <uros.orozel@gmail.com>
 Vasyl Saienko <vsaienko@mirantis.com>
 Vic Howard <victor.r.howard@gmail.com>
 Victor Lowther <victor.lowther@gmail.com>
 Victor Sergeyev <vsergeyev@mirantis.com>
 Vikas Jain <vikjain@cisco.com>
```

### Comparing `ironic-lib-6.0.0/ChangeLog` & `ironic-lib-6.1.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+6.1.0
+-----
+
+* destroy\_disk\_metadata: support 4096 sector size
+* Remove old excludes
+
 6.0.0
 -----
 
 * Swap partprobe and udev settle
 * Force constraints when installing a package during tox test
 * Bump hacking to 6.1.0
 * Split common qemu-img functions from disk\_utils
```

### Comparing `ironic-lib-6.0.0/LICENSE` & `ironic-lib-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/PKG-INFO` & `ironic-lib-6.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ironic-lib
-Version: 6.0.0
+Version: 6.1.0
 Summary: Ironic common library
 Home-page: https://docs.openstack.org/ironic-lib/
 Author: OpenStack Ironic
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==========
         ironic-lib
```

### Comparing `ironic-lib-6.0.0/README.rst` & `ironic-lib-6.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/TESTING.rst` & `ironic-lib-6.1.0/TESTING.rst`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/doc/source/conf.py` & `ironic-lib-6.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/doc/source/contributor/index.rst` & `ironic-lib-6.1.0/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/etc/ironic/rootwrap.d/ironic-lib.filters` & `ironic-lib-6.1.0/etc/ironic/rootwrap.d/ironic-lib.filters`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/__init__.py` & `ironic-lib-6.1.0/ironic_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/auth_basic.py` & `ironic-lib-6.1.0/ironic_lib/auth_basic.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/capabilities.py` & `ironic-lib-6.1.0/ironic_lib/capabilities.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/common/config.py` & `ironic-lib-6.1.0/ironic_lib/common/config.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/common/i18n.py` & `ironic-lib-6.1.0/ironic_lib/common/i18n.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/disk_partitioner.py` & `ironic-lib-6.1.0/ironic_lib/disk_partitioner.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/disk_utils.py` & `ironic-lib-6.1.0/ironic_lib/disk_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,14 @@
                               r"([\d\.]+)MiB:([\d\.]+)MiB:(\w*):(.*):(.*);")
 _PARTED_TABLE_TYPE_RE = re.compile(r'^.*partition\s+table\s*:\s*(gpt|msdos)',
                                    re.IGNORECASE | re.MULTILINE)
 
 CONFIGDRIVE_LABEL = "config-2"
 MAX_CONFIG_DRIVE_SIZE_MB = 64
 
-GPT_SIZE_SECTORS = 33
-
 # Maximum disk size supported by MBR is 2TB (2 * 1024 * 1024 MB)
 MAX_DISK_SIZE_MB_SUPPORTED_BY_MBR = 2097152
 
 # Backward compatibility, do not use
 qemu_img_info = qemu_img.image_info
 convert_image = qemu_img.convert_image
 
@@ -508,14 +506,28 @@
 def get_dev_block_size(dev):
     """Get the device size in 512 byte sectors."""
     block_sz, cmderr = utils.execute('blockdev', '--getsz', dev,
                                      run_as_root=True)
     return int(block_sz)
 
 
+def get_dev_byte_size(dev):
+    """Get the device size in bytes."""
+    byte_sz, cmderr = utils.execute('blockdev', '--getsize64', dev,
+                                    run_as_root=True)
+    return int(byte_sz)
+
+
+def get_dev_sector_size(dev):
+    """Get the device logical sector size in bytes."""
+    sect_sz, cmderr = utils.execute('blockdev', '--getss', dev,
+                                    run_as_root=True)
+    return int(sect_sz)
+
+
 def destroy_disk_metadata(dev, node_uuid):
     """Destroy metadata structures on node's disk.
 
     Ensure that node's disk magic strings are wiped without zeroing the
     entire drive. To do this we use the wipefs tool from util-linux.
 
     :param dev: Path for the device to work on.
@@ -541,29 +553,40 @@
     # NOTE(TheJulia): sgdisk attempts to load and make sense of the
     # partition tables in advance of wiping the partition data.
     # This means when a CRC error is found, sgdisk fails before
     # erasing partition data.
     # This is the same bug as
     # https://bugs.launchpad.net/ironic-python-agent/+bug/1737556
 
+    sector_size = get_dev_sector_size(dev)
+    # https://uefi.org/specs/UEFI/2.10/05_GUID_Partition_Table_Format.html If
+    # the block size is 512, the First Usable LBA must be greater than or equal
+    # to 34 [...] if the logical block size is 4096, the First Usable LBA must
+    # be greater than or equal to 6
+    if sector_size == 512:
+        gpt_sectors = 33
+    elif sector_size == 4096:
+        gpt_sectors = 5
+
     # Overwrite the Primary GPT, catch very small partitions (like EBRs)
+    dd_bs = 'bs=%s' % sector_size
     dd_device = 'of=%s' % dev
-    dd_count = 'count=%s' % GPT_SIZE_SECTORS
-    dev_size = get_dev_block_size(dev)
-    if dev_size < GPT_SIZE_SECTORS:
-        dd_count = 'count=%s' % dev_size
-    utils.execute('dd', 'bs=512', 'if=/dev/zero', dd_device, dd_count,
+    dd_count = 'count=%s' % gpt_sectors
+    dev_size = get_dev_byte_size(dev)
+    if dev_size < gpt_sectors * sector_size:
+        dd_count = 'count=%s' % int(dev_size / sector_size)
+    utils.execute('dd', dd_bs, 'if=/dev/zero', dd_device, dd_count,
                   'oflag=direct', run_as_root=True, use_standard_locale=True)
 
     # Overwrite the Secondary GPT, do this only if there could be one
-    if dev_size > GPT_SIZE_SECTORS:
-        gpt_backup = dev_size - GPT_SIZE_SECTORS
+    if dev_size > gpt_sectors * sector_size:
+        gpt_backup = int(dev_size / sector_size - gpt_sectors)
         dd_seek = 'seek=%i' % gpt_backup
-        dd_count = 'count=%s' % GPT_SIZE_SECTORS
-        utils.execute('dd', 'bs=512', 'if=/dev/zero', dd_device, dd_count,
+        dd_count = 'count=%s' % gpt_sectors
+        utils.execute('dd', dd_bs, 'if=/dev/zero', dd_device, dd_count,
                       'oflag=direct', dd_seek, run_as_root=True,
                       use_standard_locale=True)
 
     # Go ahead and let sgdisk run as well.
     utils.execute('sgdisk', '-Z', dev, run_as_root=True,
                   use_standard_locale=True)
```

### Comparing `ironic-lib-6.0.0/ironic_lib/exception.py` & `ironic-lib-6.1.0/ironic_lib/exception.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/json_rpc/__init__.py` & `ironic-lib-6.1.0/ironic_lib/json_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/json_rpc/client.py` & `ironic-lib-6.1.0/ironic_lib/json_rpc/client.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/json_rpc/server.py` & `ironic-lib-6.1.0/ironic_lib/json_rpc/server.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/keystone.py` & `ironic-lib-6.1.0/ironic_lib/keystone.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/mdns.py` & `ironic-lib-6.1.0/ironic_lib/mdns.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/metrics.py` & `ironic-lib-6.1.0/ironic_lib/metrics.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/metrics_collector.py` & `ironic-lib-6.1.0/ironic_lib/metrics_collector.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/metrics_statsd.py` & `ironic-lib-6.1.0/ironic_lib/metrics_statsd.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/metrics_utils.py` & `ironic-lib-6.1.0/ironic_lib/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/qemu_img.py` & `ironic-lib-6.1.0/ironic_lib/qemu_img.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/base.py` & `ironic-lib-6.1.0/ironic_lib/tests/base.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/test_base.py` & `ironic-lib-6.1.0/ironic_lib/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/test_basic_auth.py` & `ironic-lib-6.1.0/ironic_lib/tests/test_basic_auth.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/test_capabilities.py` & `ironic-lib-6.1.0/ironic_lib/tests/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/test_disk_partitioner.py` & `ironic-lib-6.1.0/ironic_lib/tests/test_disk_partitioner.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/test_disk_utils.py` & `ironic-lib-6.1.0/ironic_lib/tests/test_disk_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,30 +380,67 @@
 class DestroyMetaDataTestCase(base.IronicLibTestCase):
 
     def setUp(self):
         super(DestroyMetaDataTestCase, self).setUp()
         self.dev = 'fake-dev'
         self.node_uuid = "12345678-1234-1234-1234-1234567890abcxyz"
 
+    def test_destroy_disk_metadata_4096(self, mock_exec):
+        mock_exec.side_effect = iter([
+            (None, None),
+            ('4096\n', None),
+            ('524288\n', None),
+            (None, None),
+            (None, None),
+            (None, None),
+            (None, None)])
+
+        expected_calls = [mock.call('wipefs', '--force', '--all', 'fake-dev',
+                                    run_as_root=True,
+                                    use_standard_locale=True),
+                          mock.call('blockdev', '--getss', 'fake-dev',
+                                    run_as_root=True),
+                          mock.call('blockdev', '--getsize64', 'fake-dev',
+                                    run_as_root=True),
+                          mock.call('dd', 'bs=4096', 'if=/dev/zero',
+                                    'of=fake-dev', 'count=5', 'oflag=direct',
+                                    run_as_root=True,
+                                    use_standard_locale=True),
+                          mock.call('dd', 'bs=4096', 'if=/dev/zero',
+                                    'of=fake-dev', 'count=5', 'oflag=direct',
+                                    'seek=123',
+                                    run_as_root=True,
+                                    use_standard_locale=True),
+                          mock.call('sgdisk', '-Z', 'fake-dev',
+                                    run_as_root=True,
+                                    use_standard_locale=True),
+                          mock.call('fuser', self.dev, check_exit_code=[0, 1],
+                                    run_as_root=True)]
+        disk_utils.destroy_disk_metadata(self.dev, self.node_uuid)
+        mock_exec.assert_has_calls(expected_calls)
+
     def test_destroy_disk_metadata(self, mock_exec):
         # Note(TheJulia): This list will get-reused, but only the second
         # execution returning a string is needed for the test as otherwise
         # command output is not used.
         mock_exec.side_effect = iter([
             (None, None),
-            ('1024\n', None),
+            ('512\n', None),
+            ('524288\n', None),
             (None, None),
             (None, None),
             (None, None),
             (None, None)])
 
         expected_calls = [mock.call('wipefs', '--force', '--all', 'fake-dev',
                                     run_as_root=True,
                                     use_standard_locale=True),
-                          mock.call('blockdev', '--getsz', 'fake-dev',
+                          mock.call('blockdev', '--getss', 'fake-dev',
+                                    run_as_root=True),
+                          mock.call('blockdev', '--getsize64', 'fake-dev',
                                     run_as_root=True),
                           mock.call('dd', 'bs=512', 'if=/dev/zero',
                                     'of=fake-dev', 'count=33', 'oflag=direct',
                                     run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('dd', 'bs=512', 'if=/dev/zero',
                                     'of=fake-dev', 'count=33', 'oflag=direct',
@@ -430,44 +467,48 @@
                           self.node_uuid)
         mock_exec.assert_has_calls(expected_call)
 
     def test_destroy_disk_metadata_sgdisk_fail(self, mock_exec):
         expected_calls = [mock.call('wipefs', '--force', '--all', 'fake-dev',
                                     run_as_root=True,
                                     use_standard_locale=True),
-                          mock.call('blockdev', '--getsz', 'fake-dev',
+                          mock.call('blockdev', '--getss', 'fake-dev',
+                                    run_as_root=True),
+                          mock.call('blockdev', '--getsize64', 'fake-dev',
                                     run_as_root=True),
                           mock.call('dd', 'bs=512', 'if=/dev/zero',
                                     'of=fake-dev', 'count=33', 'oflag=direct',
                                     run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('dd', 'bs=512', 'if=/dev/zero',
                                     'of=fake-dev', 'count=33', 'oflag=direct',
                                     'seek=991', run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('sgdisk', '-Z', 'fake-dev',
                                     run_as_root=True,
                                     use_standard_locale=True)]
         mock_exec.side_effect = iter([
             (None, None),
-            ('1024\n', None),
+            ('512\n', None),
+            ('524288\n', None),
             (None, None),
             (None, None),
             processutils.ProcessExecutionError()])
         self.assertRaises(processutils.ProcessExecutionError,
                           disk_utils.destroy_disk_metadata,
                           self.dev,
                           self.node_uuid)
         mock_exec.assert_has_calls(expected_calls)
 
     def test_destroy_disk_metadata_wipefs_not_support_force(self, mock_exec):
         mock_exec.side_effect = iter([
             processutils.ProcessExecutionError(description='--force'),
             (None, None),
-            ('1024\n', None),
+            ('512\n', None),
+            ('524288\n', None),
             (None, None),
             (None, None),
             (None, None),
             (None, None)])
 
         expected_call = [mock.call('wipefs', '--force', '--all', 'fake-dev',
                                    run_as_root=True,
@@ -478,53 +519,59 @@
         disk_utils.destroy_disk_metadata(self.dev, self.node_uuid)
         mock_exec.assert_has_calls(expected_call)
 
     def test_destroy_disk_metadata_ebr(self, mock_exec):
         expected_calls = [mock.call('wipefs', '--force', '--all', 'fake-dev',
                                     run_as_root=True,
                                     use_standard_locale=True),
-                          mock.call('blockdev', '--getsz', 'fake-dev',
+                          mock.call('blockdev', '--getss', 'fake-dev',
+                                    run_as_root=True),
+                          mock.call('blockdev', '--getsize64', 'fake-dev',
                                     run_as_root=True),
                           mock.call('dd', 'bs=512', 'if=/dev/zero',
                                     'of=fake-dev', 'count=2', 'oflag=direct',
                                     run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('sgdisk', '-Z', 'fake-dev',
                                     run_as_root=True,
                                     use_standard_locale=True)]
         mock_exec.side_effect = iter([
             (None, None),
-            ('2\n', None),  # an EBR is 2 sectors
+            ('512\n', None),
+            ('1024\n', None),  # an EBR is 2 sectors
             (None, None),
             (None, None),
             (None, None),
             (None, None)])
         disk_utils.destroy_disk_metadata(self.dev, self.node_uuid)
         mock_exec.assert_has_calls(expected_calls)
 
     def test_destroy_disk_metadata_tiny_partition(self, mock_exec):
         expected_calls = [mock.call('wipefs', '--force', '--all', 'fake-dev',
                                     run_as_root=True,
                                     use_standard_locale=True),
-                          mock.call('blockdev', '--getsz', 'fake-dev',
+                          mock.call('blockdev', '--getss', 'fake-dev',
+                                    run_as_root=True),
+                          mock.call('blockdev', '--getsize64', 'fake-dev',
                                     run_as_root=True),
                           mock.call('dd', 'bs=512', 'if=/dev/zero',
                                     'of=fake-dev', 'count=33', 'oflag=direct',
                                     run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('dd', 'bs=512', 'if=/dev/zero',
                                     'of=fake-dev', 'count=33', 'oflag=direct',
                                     'seek=9', run_as_root=True,
                                     use_standard_locale=True),
                           mock.call('sgdisk', '-Z', 'fake-dev',
                                     run_as_root=True,
                                     use_standard_locale=True)]
         mock_exec.side_effect = iter([
             (None, None),
-            ('42\n', None),
+            ('512\n', None),
+            ('21504\n', None),
             (None, None),
             (None, None),
             (None, None),
             (None, None)])
         disk_utils.destroy_disk_metadata(self.dev, self.node_uuid)
         mock_exec.assert_has_calls(expected_calls)
 
@@ -541,14 +588,30 @@
         mock_exec.return_value = ("64", "")
         expected_call = [mock.call('blockdev', '--getsz', self.dev,
                                    run_as_root=True)]
         disk_utils.get_dev_block_size(self.dev)
         mock_exec.assert_has_calls(expected_call)
 
 
+@mock.patch.object(utils, 'execute', autospec=True)
+class GetDeviceByteSizeTestCase(base.IronicLibTestCase):
+
+    def setUp(self):
+        super(GetDeviceByteSizeTestCase, self).setUp()
+        self.dev = 'fake-dev'
+        self.node_uuid = "12345678-1234-1234-1234-1234567890abcxyz"
+
+    def test_get_dev_byte_size(self, mock_exec):
+        mock_exec.return_value = ("64", "")
+        expected_call = [mock.call('blockdev', '--getsize64', self.dev,
+                                   run_as_root=True)]
+        disk_utils.get_dev_byte_size(self.dev)
+        mock_exec.assert_has_calls(expected_call)
+
+
 @mock.patch.object(disk_utils, 'dd', autospec=True)
 @mock.patch.object(qemu_img, 'image_info', autospec=True)
 @mock.patch.object(qemu_img, 'convert_image', autospec=True)
 class PopulateImageTestCase(base.IronicLibTestCase):
 
     def test_populate_raw_image(self, mock_cg, mock_qinfo, mock_dd):
         type(mock_qinfo.return_value).file_format = mock.PropertyMock(
```

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/test_exception.py` & `ironic-lib-6.1.0/ironic_lib/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/test_json_rpc.py` & `ironic-lib-6.1.0/ironic_lib/tests/test_json_rpc.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/test_keystone.py` & `ironic-lib-6.1.0/ironic_lib/tests/test_keystone.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/test_mdns.py` & `ironic-lib-6.1.0/ironic_lib/tests/test_mdns.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/test_metrics.py` & `ironic-lib-6.1.0/ironic_lib/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/test_metrics_collector.py` & `ironic-lib-6.1.0/ironic_lib/tests/test_metrics_collector.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/test_metrics_statsd.py` & `ironic-lib-6.1.0/ironic_lib/tests/test_metrics_statsd.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/test_metrics_utils.py` & `ironic-lib-6.1.0/ironic_lib/tests/test_metrics_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/test_qemu_img.py` & `ironic-lib-6.1.0/ironic_lib/tests/test_qemu_img.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/tests/test_utils.py` & `ironic-lib-6.1.0/ironic_lib/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/utils.py` & `ironic-lib-6.1.0/ironic_lib/utils.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib/wsgi.py` & `ironic-lib-6.1.0/ironic_lib/wsgi.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/ironic_lib.egg-info/PKG-INFO` & `ironic-lib-6.1.0/ironic_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ironic-lib
-Version: 6.0.0
+Version: 6.1.0
 Summary: Ironic common library
 Home-page: https://docs.openstack.org/ironic-lib/
 Author: OpenStack Ironic
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==========
         ironic-lib
```

### Comparing `ironic-lib-6.0.0/ironic_lib.egg-info/SOURCES.txt` & `ironic-lib-6.1.0/ironic_lib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -76,10 +76,11 @@
 releasenotes/notes/fix-dd-async-gpt-erasure-bbc6b084b0344d30.yaml
 releasenotes/notes/fix-metadisk-partitioning-32d3fca274290dd6.yaml
 releasenotes/notes/increase-efi-partition-size-9479d069b17804ce.yaml
 releasenotes/notes/json_rpc-allowed_roles-3bee50b5936c2be3.yaml
 releasenotes/notes/remove-iscsi-verify-attempts-ff9eb5b7a28e6143.yaml
 releasenotes/notes/rescan-for-partition-write-out-3fbb92ae5c2a33c6.yaml
 releasenotes/notes/restore-centos7-compatibility-bfbe2bcf1d1fb7f0.yaml
+releasenotes/notes/support-4096-sector-size-aa479b4040399975.yaml
 releasenotes/notes/wipe-gpt-on-metadata-wipe-ac0a93b16e00893f.yaml
 zuul.d/ironic-lib-jobs.yaml
 zuul.d/project.yaml
```

### Comparing `ironic-lib-6.0.0/ironic_lib.egg-info/entry_points.txt` & `ironic-lib-6.1.0/ironic_lib.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/releasenotes/notes/add-additional-disk-conversion-retry-dfff93cbdf779f81.yaml` & `ironic-lib-6.1.0/releasenotes/notes/add-additional-disk-conversion-retry-dfff93cbdf779f81.yaml`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/releasenotes/notes/basic-auth-middleware-e5af29651b2d7979.yaml` & `ironic-lib-6.1.0/releasenotes/notes/basic-auth-middleware-e5af29651b2d7979.yaml`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/releasenotes/notes/increase-efi-partition-size-9479d069b17804ce.yaml` & `ironic-lib-6.1.0/releasenotes/notes/increase-efi-partition-size-9479d069b17804ce.yaml`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/setup.cfg` & `ironic-lib-6.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/setup.py` & `ironic-lib-6.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/tox.ini` & `ironic-lib-6.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `ironic-lib-6.0.0/zuul.d/ironic-lib-jobs.yaml` & `ironic-lib-6.1.0/zuul.d/ironic-lib-jobs.yaml`

 * *Files identical despite different names*

