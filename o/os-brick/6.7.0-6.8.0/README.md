# Comparing `tmp/os-brick-6.7.0.tar.gz` & `tmp/os-brick-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os-brick-6.7.0.tar", last modified: Fri Feb 23 08:48:41 2024, max compression
+gzip compressed data, was "os-brick-6.8.0.tar", last modified: Thu May 23 08:02:56 2024, max compression
```

## Comparing `os-brick-6.7.0.tar` & `os-brick-6.8.0.tar`

### file list

```diff
@@ -1,314 +1,316 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.203929 os-brick-6.7.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-02-23 08:48:10.000000 os-brick-6.7.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-02-23 08:48:10.000000 os-brick-6.7.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6807 2024-02-23 08:48:10.000000 os-brick-6.7.0/.pylintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-02-23 08:48:10.000000 os-brick-6.7.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3039 2024-02-23 08:48:10.000000 os-brick-6.7.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6933 2024-02-23 08:48:40.000000 os-brick-6.7.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2024-02-23 08:48:10.000000 os-brick-6.7.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31754 2024-02-23 08:48:40.000000 os-brick-6.7.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-02-23 08:48:10.000000 os-brick-6.7.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-02-23 08:48:10.000000 os-brick-6.7.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1061 2024-02-23 08:48:41.203929 os-brick-6.7.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2024-02-23 08:48:10.000000 os-brick-6.7.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1884 2024-02-23 08:48:10.000000 os-brick-6.7.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.167929 os-brick-6.7.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2024-02-23 08:48:10.000000 os-brick-6.7.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.167929 os-brick-6.7.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3140 2024-02-23 08:48:10.000000 os-brick-6.7.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.167929 os-brick-6.7.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2024-02-23 08:48:10.000000 os-brick-6.7.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-02-23 08:48:10.000000 os-brick-6.7.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.167929 os-brick-6.7.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2024-02-23 08:48:10.000000 os-brick-6.7.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.167929 os-brick-6.7.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2024-02-23 08:48:10.000000 os-brick-6.7.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.167929 os-brick-6.7.0/doc/source/reference/os_brick/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2024-02-23 08:48:10.000000 os-brick-6.7.0/doc/source/reference/os_brick/exception.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-02-23 08:48:10.000000 os-brick-6.7.0/doc/source/reference/os_brick/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.167929 os-brick-6.7.0/doc/source/reference/os_brick/initiator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2024-02-23 08:48:10.000000 os-brick-6.7.0/doc/source/reference/os_brick/initiator/connector.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-02-23 08:48:10.000000 os-brick-6.7.0/doc/source/reference/os_brick/initiator/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.167929 os-brick-6.7.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2283 2024-02-23 08:48:10.000000 os-brick-6.7.0/doc/source/user/tutorial.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.159929 os-brick-6.7.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.163929 os-brick-6.7.0/etc/os-brick/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.167929 os-brick-6.7.0/etc/os-brick/rootwrap.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2024-02-23 08:48:10.000000 os-brick-6.7.0/etc/os-brick/rootwrap.d/os-brick.filters
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2024-02-23 08:48:10.000000 os-brick-6.7.0/mypy-files.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.167929 os-brick-6.7.0/os_brick/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.171929 os-brick-6.7.0/os_brick/caches/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3377 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/caches/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4197 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/caches/opencas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1126 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.171929 os-brick-6.7.0/os_brick/encryptors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5487 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/encryptors/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2326 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/encryptors/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7531 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/encryptors/cryptsetup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11379 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/encryptors/luks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1605 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/encryptors/nop.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7546 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3123 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.171929 os-brick-6.7.0/os_brick/initiator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1595 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11636 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connector.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.175929 os-brick-6.7.0/os_brick/initiator/connectors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7406 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2288 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/base_iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2036 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/base_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/fake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19333 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/fibre_channel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1979 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/fibre_channel_ppc64.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4324 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/fibre_channel_s390x.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/gpfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7750 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/huawei.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    58227 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13060 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/lightos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3018 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/local.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    59686 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/nvmeof.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18651 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5154 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/remotefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20688 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/scaleio.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10364 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/storpool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14485 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/connectors/vmware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/host_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9607 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/initiator_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16456 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/linuxfc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8269 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/linuxrbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36112 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/linuxscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.175929 os-brick-6.7.0/os_brick/initiator/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4720 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/windows/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8427 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/windows/fibre_channel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7399 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/windows/iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6727 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/windows/rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5195 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/initiator/windows/smbfs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.175929 os-brick-6.7.0/os_brick/local_dev/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/local_dev/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31721 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/local_dev/lvm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.175929 os-brick-6.7.0/os_brick/privileged/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/privileged/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/privileged/lightos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4892 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/privileged/nvmeof.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2059 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/privileged/rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9466 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/privileged/rootwrap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2948 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/privileged/scaleio.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.179929 os-brick-6.7.0/os_brick/remotefs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/remotefs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11191 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/remotefs/remotefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5663 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/remotefs/windows_remotefs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.179929 os-brick-6.7.0/os_brick/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4800 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.179929 os-brick-6.7.0/os_brick/tests/caches/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/caches/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4883 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/caches/test_init.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6700 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/caches/test_opencas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.179929 os-brick-6.7.0/os_brick/tests/encryptors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/encryptors/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8054 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/encryptors/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6846 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/encryptors/test_cryptsetup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15068 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/encryptors/test_luks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1611 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/encryptors/test_nop.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.179929 os-brick-6.7.0/os_brick/tests/initiator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.183929 os-brick-6.7.0/os_brick/tests/initiator/connectors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3984 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_base_iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3137 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_base_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47198 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_fibre_channel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2323 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_fibre_channel_ppc64.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5036 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_fibre_channel_s390x.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_gpfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10535 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_huawei.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    86282 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3430 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_iser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10989 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_lightos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2284 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_local.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   105206 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_nvmeof.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25104 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3323 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_remotefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14838 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_scaleio.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6831 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_storpool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18260 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/connectors/test_vmware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13487 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/test_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1718 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/test_host_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29891 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/test_linuxfc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10186 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/test_linuxrbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    69689 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/test_linuxscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3348 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/initiator/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.183929 os-brick-6.7.0/os_brick/tests/local_dev/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/local_dev/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/local_dev/fake_lvm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16313 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/local_dev/test_brick_lvm.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.183929 os-brick-6.7.0/os_brick/tests/privileged/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/privileged/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10526 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/privileged/test_nvmeof.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3528 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/privileged/test_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9226 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/privileged/test_rootwrap.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.183929 os-brick-6.7.0/os_brick/tests/remotefs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/remotefs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11848 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/remotefs/test_remotefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6632 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/remotefs/test_windows_remotefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/test_brick.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6655 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/test_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28531 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.187929 os-brick-6.7.0/os_brick/tests/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/windows/fake_win_conn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/windows/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5795 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/windows/test_base_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1562 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/windows/test_factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11642 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/windows/test_fibre_channel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9125 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/windows/test_iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5340 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/windows/test_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7736 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/tests/windows/test_smbfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16327 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2024-02-23 08:48:10.000000 os-brick-6.7.0/os_brick/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.171929 os-brick-6.7.0/os_brick.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1061 2024-02-23 08:48:40.000000 os-brick-6.7.0/os_brick.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11976 2024-02-23 08:48:41.000000 os-brick-6.7.0/os_brick.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-23 08:48:40.000000 os-brick-6.7.0/os_brick.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-23 08:48:40.000000 os-brick-6.7.0/os_brick.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-23 08:48:40.000000 os-brick-6.7.0/os_brick.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-23 08:48:40.000000 os-brick-6.7.0/os_brick.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-02-23 08:48:40.000000 os-brick-6.7.0/os_brick.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-02-23 08:48:40.000000 os-brick-6.7.0/os_brick.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2024-02-23 08:48:10.000000 os-brick-6.7.0/pylintrc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.163929 os-brick-6.7.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.199929 os-brick-6.7.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/add-luks2-support-13563cfe83aba69c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/add-vstorage-protocol-b536f4e21d764801.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/add-windows-fibre-channel-030c095c149da321.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/add-windows-iscsi-15d6b1392695f978.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/add-windows-smbfs-d86edaa003130a31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/add_custom_keyring_for_rbd_connection-eccbaae9ee5f3491.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bp-lightbits-lightos-clustered-nvmetcp-connector-fd8dfd73330973e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-1609753-16eace7f2b48d805.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-1722432-2408dab55c903c5b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-1823200-scaleio-upgrade-3e83b5c9dd148714.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-1823200-victoria-b414a1806cba3998.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-1862443-e87ef38b60f9b979.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-1865754-ceph-octopus-compatibility-0aa9b8bc1b028301.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-1884052-798094496dccf23c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-1888675-mpath-resize-6013ce39fa2b8401.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-1915678-901a6bd24ecede72.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-1924652-2323f905f62ef8ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-1929223-powerflex-connector-certificate-validation-cf9ffc98391115d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-1938870-af85c420d1a108a9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-1944474-55c5ebb3a37801aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-1945323-4140f5aff3558082.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-2004630-e94616509a51258c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-2013749-3de9f827b82116a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/bug-nvmeof-connector-support-multipath-kernels-ff6f1f27fdea2c8e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/default-timeout-26c838af8b7af9fc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/delay-legacy-encryption-provider-name-deprecation-c0d07be3f0d92afd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/dell-powerflex-bug-2046810-c16ba2bd8dde06d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/deprecate-plain-cryptsetup-encryptor-0a279abc0b0d718c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/deprecate-windows-support-bdc643525e9bb132.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/disconnect-multipath-cfg-changed-637abc5ecf44fb10.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/drop-py2-7dcde3ccd0e167b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/drop-python-3-6-and-3-7-1e7190189d415492.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/encryption-a642889a82ff9207.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/extend-encrypted-in-use-ac3f7a1994ec3a38.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/external-locks-9f015988ebdc37d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/fc-always-check-single-wwnn-1595689da0eb673b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/fc-flush-single-path-22ed6cc7b56a6d9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/fc-force-disconnect-1a33cf46c233dd04.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      381 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/fix-extend-multipath-a308d333061665fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/fix-fc-scan-too-broad-3c576e1846b7f05f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/fix-fc-scanning-9164da9eb42aaed0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/fix-generate-hostnqn-in-case-old-nvmecli.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/fix-multipath-disconnect-819d01e6e981883e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/fix-nvme-issues-8dfc15cb691389fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/improve-get_sysfs_wwn-df38ea88cdcdcc94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/improve-iscsi-multipath-detection-f36f28a993f61936.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/introduce-encryption-provider-constants-a7cd0ce58da2bae8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/iscsi_manual_scan_support-d64a1c3c8e1986b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/local-attach-in-rbd-connector-c06347fb164b084a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/lock_path-c1c58a253391b41c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/lvm-delete-error-76f2cc9d8dc91f01.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/multipath-improvements-596c2c6eadfba6ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/multipath-nvme-f77a53eb2717a44c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/no-systool-use-b7bc430de1033670.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/nvme-flush-f31ab337224e5d3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/nvme-hostnqn-c2611dc56729183b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/nvme-rsd-support-d487afd77c534fa1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/nvmeof-connecting-788f77a42fe7dd3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1740 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/nvmeof-consolidate-004dbe3a98f6f815.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/nvmeof-create-hostid-15bf84ec00726fad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/nvmeof-disconnect-83f9aaf17f8c8988.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/nvmeof-faster-create-hostnqn-81a63844142858bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/nvmeof-findmnt-args-b2c966af83bd3bf3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/nvmeof-hide-traceback-a968ab71352684e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/nvmeof-multiple-volumes-within-subsystem-support-05879c1c3bdf52c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/nvmeof-new-address-56044523cf8fc203.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/nvmeof-old-shownqn-c8cc2820b9c1418e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/nvmeof-support-v2-0d3a423c26eee003.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/privsep-logs-9e938e5a2aee042e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/rbd-disconnect-failure-9efa6932df40271b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/rbd-non-openstack-support-28ee093d7d3a700e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/rbd-windows-support-ef6e8184842409dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/rbd_check_valid_device-2f50c0639adb8e7c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/rbd_extend_volume-5bc6adc08f662c5b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/refactor_iscsi_connect-dfbb24305a954783.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/refactor_iscsi_disconnect-557f4173bc1ae4ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/remove-aoe-7a97315a73c7b24f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/remove-bug-1633518-workaround-75c2e26843660696.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/remove-disco-0809537ffb8c50eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/remove-drbd-21872230fcac1138.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/remove-hgst-daa7f07c307974d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/remove-hyperscale-468f1b61bf4dadf8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/remove-old-constants-20021f5b30bde890.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/remove-sheepdog-611257b28bc88934.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/scaleio-extend-attached-ec44d3a72395882c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/scsi-addressing-modes-7674ea30d4ff4c49.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/start-using-reno-23e8d5f1a30851a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/unsupported-lvm-versions-cbaeabce3ace1805.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/update-nvmeof-connector-6260a658c15a9a6e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/ussuri-release-979d709dfa7df068.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/veritas-hyperscale-connector-fe56cec68b1947cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/vmware-vmdk-connector-19e6999e6cae43cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/notes/yoga-known-issues-f1248af0e328d63e.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.203929 os-brick-6.7.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.203929 os-brick-6.7.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.203929 os-brick-6.7.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1732 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-23 08:48:10.000000 os-brick-6.7.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2024-02-23 08:48:10.000000 os-brick-6.7.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1379 2024-02-23 08:48:41.203929 os-brick-6.7.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-02-23 08:48:10.000000 os-brick-6.7.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2024-02-23 08:48:10.000000 os-brick-6.7.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:48:41.203929 os-brick-6.7.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1189 2024-02-23 08:48:10.000000 os-brick-6.7.0/tools/coding-checks.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      299 2024-02-23 08:48:10.000000 os-brick-6.7.0/tools/fast8.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6189 2024-02-23 08:48:10.000000 os-brick-6.7.0/tools/generate_connector_list.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6793 2024-02-23 08:48:10.000000 os-brick-6.7.0/tools/lintstack.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2182 2024-02-23 08:48:10.000000 os-brick-6.7.0/tools/lintstack.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2024-02-23 08:48:10.000000 os-brick-6.7.0/tools/mypywrap.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4674 2024-02-23 08:48:10.000000 os-brick-6.7.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.231999 os-brick-6.8.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-05-23 08:02:29.000000 os-brick-6.8.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-05-23 08:02:29.000000 os-brick-6.8.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6807 2024-05-23 08:02:29.000000 os-brick-6.8.0/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-05-23 08:02:29.000000 os-brick-6.8.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3039 2024-05-23 08:02:29.000000 os-brick-6.8.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6966 2024-05-23 08:02:55.000000 os-brick-6.8.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2024-05-23 08:02:29.000000 os-brick-6.8.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32131 2024-05-23 08:02:55.000000 os-brick-6.8.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-05-23 08:02:29.000000 os-brick-6.8.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-23 08:02:29.000000 os-brick-6.8.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2024-05-23 08:02:56.231999 os-brick-6.8.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2024-05-23 08:02:29.000000 os-brick-6.8.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1884 2024-05-23 08:02:29.000000 os-brick-6.8.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.171982 os-brick-6.8.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2024-05-23 08:02:29.000000 os-brick-6.8.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.171982 os-brick-6.8.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3140 2024-05-23 08:02:29.000000 os-brick-6.8.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.171982 os-brick-6.8.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2024-05-23 08:02:29.000000 os-brick-6.8.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-05-23 08:02:29.000000 os-brick-6.8.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.171982 os-brick-6.8.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2024-05-23 08:02:29.000000 os-brick-6.8.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.171982 os-brick-6.8.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2024-05-23 08:02:29.000000 os-brick-6.8.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.171982 os-brick-6.8.0/doc/source/reference/os_brick/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2024-05-23 08:02:29.000000 os-brick-6.8.0/doc/source/reference/os_brick/exception.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-05-23 08:02:29.000000 os-brick-6.8.0/doc/source/reference/os_brick/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.171982 os-brick-6.8.0/doc/source/reference/os_brick/initiator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2024-05-23 08:02:29.000000 os-brick-6.8.0/doc/source/reference/os_brick/initiator/connector.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-05-23 08:02:29.000000 os-brick-6.8.0/doc/source/reference/os_brick/initiator/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.171982 os-brick-6.8.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2283 2024-05-23 08:02:29.000000 os-brick-6.8.0/doc/source/user/tutorial.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.159978 os-brick-6.8.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.159978 os-brick-6.8.0/etc/os-brick/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.175983 os-brick-6.8.0/etc/os-brick/rootwrap.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2024-05-23 08:02:29.000000 os-brick-6.8.0/etc/os-brick/rootwrap.d/os-brick.filters
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2024-05-23 08:02:29.000000 os-brick-6.8.0/mypy-files.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.175983 os-brick-6.8.0/os_brick/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.179984 os-brick-6.8.0/os_brick/caches/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3377 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/caches/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4197 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/caches/opencas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1126 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.179984 os-brick-6.8.0/os_brick/encryptors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5487 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/encryptors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2326 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/encryptors/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7531 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/encryptors/cryptsetup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11379 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/encryptors/luks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1605 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/encryptors/nop.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7546 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3123 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.179984 os-brick-6.8.0/os_brick/initiator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1595 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11636 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connector.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.187986 os-brick-6.8.0/os_brick/initiator/connectors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7406 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2288 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/base_iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2036 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/base_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/fake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19333 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/fibre_channel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1979 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/fibre_channel_ppc64.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4324 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/fibre_channel_s390x.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/gpfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7750 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/huawei.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    58227 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13060 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/lightos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3018 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/local.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    59886 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/nvmeof.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18651 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5154 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/remotefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20688 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/scaleio.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10364 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/storpool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14485 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/connectors/vmware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/host_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9607 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/initiator_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16456 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/linuxfc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8269 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/linuxrbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36112 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/linuxscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.187986 os-brick-6.8.0/os_brick/initiator/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4720 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/windows/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8427 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/windows/fibre_channel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7399 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/windows/iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6727 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/windows/rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5195 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/initiator/windows/smbfs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.187986 os-brick-6.8.0/os_brick/local_dev/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/local_dev/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31721 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/local_dev/lvm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.187986 os-brick-6.8.0/os_brick/privileged/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/privileged/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/privileged/lightos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4892 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/privileged/nvmeof.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2059 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/privileged/rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9466 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/privileged/rootwrap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2948 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/privileged/scaleio.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.191988 os-brick-6.8.0/os_brick/remotefs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/remotefs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11191 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/remotefs/remotefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5663 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/remotefs/windows_remotefs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.191988 os-brick-6.8.0/os_brick/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4800 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.191988 os-brick-6.8.0/os_brick/tests/caches/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/caches/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4883 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/caches/test_init.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6700 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/caches/test_opencas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.191988 os-brick-6.8.0/os_brick/tests/encryptors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/encryptors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8054 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/encryptors/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6846 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/encryptors/test_cryptsetup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15068 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/encryptors/test_luks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1611 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/encryptors/test_nop.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.195989 os-brick-6.8.0/os_brick/tests/initiator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.199990 os-brick-6.8.0/os_brick/tests/initiator/connectors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3984 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_base_iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3137 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_base_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47198 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_fibre_channel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2323 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_fibre_channel_ppc64.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5036 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_fibre_channel_s390x.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_gpfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10535 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_huawei.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    86282 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3430 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_iser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10989 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_lightos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2284 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_local.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   105509 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_nvmeof.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25104 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3323 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_remotefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14838 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_scaleio.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6831 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_storpool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18260 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/connectors/test_vmware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13487 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/test_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1718 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/test_host_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29891 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/test_linuxfc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10186 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/test_linuxrbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    69689 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/test_linuxscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3348 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/initiator/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.199990 os-brick-6.8.0/os_brick/tests/local_dev/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/local_dev/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/local_dev/fake_lvm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16313 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/local_dev/test_brick_lvm.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.199990 os-brick-6.8.0/os_brick/tests/privileged/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/privileged/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10526 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/privileged/test_nvmeof.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3528 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/privileged/test_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9226 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/privileged/test_rootwrap.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.203991 os-brick-6.8.0/os_brick/tests/remotefs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/remotefs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11848 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/remotefs/test_remotefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6632 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/remotefs/test_windows_remotefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/test_brick.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6655 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/test_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28531 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.203991 os-brick-6.8.0/os_brick/tests/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/windows/fake_win_conn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/windows/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5795 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/windows/test_base_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1562 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/windows/test_factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11642 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/windows/test_fibre_channel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9125 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/windows/test_iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5340 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/windows/test_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7736 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/tests/windows/test_smbfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16327 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2024-05-23 08:02:29.000000 os-brick-6.8.0/os_brick/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.175983 os-brick-6.8.0/os_brick.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2024-05-23 08:02:55.000000 os-brick-6.8.0/os_brick.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12070 2024-05-23 08:02:56.000000 os-brick-6.8.0/os_brick.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:02:55.000000 os-brick-6.8.0/os_brick.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-05-23 08:02:55.000000 os-brick-6.8.0/os_brick.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:02:55.000000 os-brick-6.8.0/os_brick.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-23 08:02:55.000000 os-brick-6.8.0/os_brick.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-05-23 08:02:55.000000 os-brick-6.8.0/os_brick.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-05-23 08:02:55.000000 os-brick-6.8.0/os_brick.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2024-05-23 08:02:29.000000 os-brick-6.8.0/pylintrc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.163979 os-brick-6.8.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.223997 os-brick-6.8.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/add-luks2-support-13563cfe83aba69c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/add-vstorage-protocol-b536f4e21d764801.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/add-windows-fibre-channel-030c095c149da321.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/add-windows-iscsi-15d6b1392695f978.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/add-windows-smbfs-d86edaa003130a31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/add_custom_keyring_for_rbd_connection-eccbaae9ee5f3491.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bp-lightbits-lightos-clustered-nvmetcp-connector-fd8dfd73330973e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-1609753-16eace7f2b48d805.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-1722432-2408dab55c903c5b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-1823200-scaleio-upgrade-3e83b5c9dd148714.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-1823200-victoria-b414a1806cba3998.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-1862443-e87ef38b60f9b979.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-1865754-ceph-octopus-compatibility-0aa9b8bc1b028301.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-1884052-798094496dccf23c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-1888675-mpath-resize-6013ce39fa2b8401.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-1915678-901a6bd24ecede72.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-1924652-2323f905f62ef8ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-1929223-powerflex-connector-certificate-validation-cf9ffc98391115d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-1938870-af85c420d1a108a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-1944474-55c5ebb3a37801aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-1945323-4140f5aff3558082.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-2004630-e94616509a51258c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-2013749-3de9f827b82116a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/bug-nvmeof-connector-support-multipath-kernels-ff6f1f27fdea2c8e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/default-timeout-26c838af8b7af9fc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/delay-legacy-encryption-provider-name-deprecation-c0d07be3f0d92afd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/dell-powerflex-bug-2046810-c16ba2bd8dde06d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/deprecate-plain-cryptsetup-encryptor-0a279abc0b0d718c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/deprecate-windows-support-bdc643525e9bb132.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/disconnect-multipath-cfg-changed-637abc5ecf44fb10.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/drop-py2-7dcde3ccd0e167b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/drop-python-3-6-and-3-7-1e7190189d415492.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/encryption-a642889a82ff9207.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/extend-encrypted-in-use-ac3f7a1994ec3a38.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/external-locks-9f015988ebdc37d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/fc-always-check-single-wwnn-1595689da0eb673b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/fc-flush-single-path-22ed6cc7b56a6d9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/fc-force-disconnect-1a33cf46c233dd04.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      381 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/fix-extend-multipath-a308d333061665fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/fix-fc-scan-too-broad-3c576e1846b7f05f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/fix-fc-scanning-9164da9eb42aaed0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/fix-generate-hostnqn-in-case-old-nvmecli.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/fix-host-uuid-warning-3814b7e47bde8010.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/fix-multipath-disconnect-819d01e6e981883e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/fix-nvme-issues-8dfc15cb691389fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/improve-get_sysfs_wwn-df38ea88cdcdcc94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/improve-iscsi-multipath-detection-f36f28a993f61936.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/introduce-encryption-provider-constants-a7cd0ce58da2bae8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/iscsi_manual_scan_support-d64a1c3c8e1986b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/local-attach-in-rbd-connector-c06347fb164b084a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/lock_path-c1c58a253391b41c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/lvm-delete-error-76f2cc9d8dc91f01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/multipath-improvements-596c2c6eadfba6ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/multipath-nvme-f77a53eb2717a44c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/no-systool-use-b7bc430de1033670.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/nvme-flush-f31ab337224e5d3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/nvme-hostnqn-c2611dc56729183b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/nvme-rsd-support-d487afd77c534fa1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/nvmeof-connecting-788f77a42fe7dd3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1740 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/nvmeof-consolidate-004dbe3a98f6f815.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/nvmeof-create-hostid-15bf84ec00726fad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/nvmeof-disconnect-83f9aaf17f8c8988.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/nvmeof-faster-create-hostnqn-81a63844142858bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/nvmeof-findmnt-args-b2c966af83bd3bf3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/nvmeof-hide-traceback-a968ab71352684e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/nvmeof-multiple-volumes-within-subsystem-support-05879c1c3bdf52c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/nvmeof-new-address-56044523cf8fc203.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/nvmeof-old-shownqn-c8cc2820b9c1418e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/nvmeof-support-v2-0d3a423c26eee003.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/privsep-logs-9e938e5a2aee042e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/rbd-disconnect-failure-9efa6932df40271b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/rbd-non-openstack-support-28ee093d7d3a700e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/rbd-windows-support-ef6e8184842409dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/rbd_check_valid_device-2f50c0639adb8e7c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/rbd_extend_volume-5bc6adc08f662c5b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/refactor_iscsi_connect-dfbb24305a954783.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/refactor_iscsi_disconnect-557f4173bc1ae4ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/remove-aoe-7a97315a73c7b24f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/remove-bug-1633518-workaround-75c2e26843660696.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/remove-disco-0809537ffb8c50eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/remove-drbd-21872230fcac1138.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/remove-hgst-daa7f07c307974d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/remove-hyperscale-468f1b61bf4dadf8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/remove-old-constants-20021f5b30bde890.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/remove-sheepdog-611257b28bc88934.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/scaleio-extend-attached-ec44d3a72395882c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/scsi-addressing-modes-7674ea30d4ff4c49.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/start-using-reno-23e8d5f1a30851a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/unsupported-lvm-versions-cbaeabce3ace1805.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/update-nvmeof-connector-6260a658c15a9a6e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/ussuri-release-979d709dfa7df068.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/veritas-hyperscale-connector-fe56cec68b1947cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/vmware-vmdk-connector-19e6999e6cae43cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/notes/yoga-known-issues-f1248af0e328d63e.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.231999 os-brick-6.8.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.231999 os-brick-6.8.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.231999 os-brick-6.8.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1732 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-05-23 08:02:29.000000 os-brick-6.8.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2024-05-23 08:02:29.000000 os-brick-6.8.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2024-05-23 08:02:56.236001 os-brick-6.8.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-05-23 08:02:29.000000 os-brick-6.8.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2024-05-23 08:02:29.000000 os-brick-6.8.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:56.231999 os-brick-6.8.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1189 2024-05-23 08:02:29.000000 os-brick-6.8.0/tools/coding-checks.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      299 2024-05-23 08:02:29.000000 os-brick-6.8.0/tools/fast8.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6189 2024-05-23 08:02:29.000000 os-brick-6.8.0/tools/generate_connector_list.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6793 2024-05-23 08:02:29.000000 os-brick-6.8.0/tools/lintstack.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2182 2024-05-23 08:02:29.000000 os-brick-6.8.0/tools/lintstack.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2024-05-23 08:02:29.000000 os-brick-6.8.0/tools/mypywrap.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4674 2024-05-23 08:02:29.000000 os-brick-6.8.0/tox.ini
```

### Comparing `os-brick-6.7.0/.pylintrc` & `os-brick-6.8.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/.zuul.yaml` & `os-brick-6.8.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/AUTHORS` & `os-brick-6.8.0/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 LisaLi <xiaoyan.li@intel.com>
 Liu Qing <liuqing@chinac.com>
 Lucian Petrut <lpetrut@cloudbasesolutions.com>
 Luigi Toscano <ltoscano@redhat.com>
 Lukas Bezdicka <lbezdick@redhat.com>
 Luong Anh Tuan <tuanla@vn.fujitsu.com>
 Maciej Kucia <maciej@kucia.net>
+Mark Goddard <mark@stackhpc.com>
 Matan Sabag <matan.sabag@emc.com>
 Mathieu Gagné <mgagne@iweb.com>
 Matt Riedemann <mriedem@us.ibm.com>
 Matthew Booth <mbooth@redhat.com>
 Michael Price <michael.price@netapp.com>
 Michal Dulko <michal.dulko@intel.com>
 Michał Dulko <michal.dulko@intel.com>
```

### Comparing `os-brick-6.7.0/CONTRIBUTING.rst` & `os-brick-6.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/ChangeLog` & `os-brick-6.8.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 CHANGES
 =======
 
+6.8.0
+-----
+
+* reno: Update master for unmaintained/zed
+* Update CI for Dalmatian
+* Cleanup pylintrc adjustments for six
+* Update master for stable/2024.1
+* reno: Update master for xena Unmaintained status
+* reno: Update master for wallaby Unmaintained status
+* reno: Update master for victoria Unmaintained status
+
 6.7.0
 -----
 
 * Deprecate Windows OS support
 * Add releasenote for unchecked LVM versions
 * Fix: FC partial target scan
 * reno: Update master for yoga Unmaintained status
@@ -13,14 +24,15 @@
 -----
 
 * Update python classifier in setup.cfg
 * NVMe-oF: Support nvme cli v2
 * NVME-oF: Fix to support new "address" in sysfs
 * NVMe-oF: Fix attach when reconnecting
 * Dell Powerflex: Add new VOLUME\_NOT\_MAPPED\_ERROR
+* Silence warning when running in a container with overlayfs
 * Remove unnecessary 'type: ignore' comments
 * NVMe-oF: Improve hostnqn creation
 * Dell PowerFlex: Unnecessary login happen
 
 6.5.0
 -----
```

### Comparing `os-brick-6.7.0/LICENSE` & `os-brick-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/PKG-INFO` & `os-brick-6.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: os-brick
-Version: 6.7.0
+Version: 6.8.0
 Summary: OpenStack Cinder brick library for managing local volume attaches
 Home-page: https://docs.openstack.org/os-brick/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: OpenStack Cinder brick library for managing local volume attaches
 Platform: UNKNOWN
@@ -13,12 +13,11 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
```

### Comparing `os-brick-6.7.0/README.rst` & `os-brick-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/bindep.txt` & `os-brick-6.8.0/bindep.txt`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/doc/source/conf.py` & `os-brick-6.8.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/doc/source/contributor/contributing.rst` & `os-brick-6.8.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/doc/source/reference/os_brick/exception.rst` & `os-brick-6.8.0/doc/source/reference/os_brick/exception.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/doc/source/reference/os_brick/initiator/connector.rst` & `os-brick-6.8.0/doc/source/reference/os_brick/initiator/connector.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/doc/source/user/tutorial.rst` & `os-brick-6.8.0/doc/source/user/tutorial.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/mypy-files.txt` & `os-brick-6.8.0/mypy-files.txt`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/__init__.py` & `os-brick-6.8.0/os_brick/__init__.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/caches/__init__.py` & `os-brick-6.8.0/os_brick/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/caches/opencas.py` & `os-brick-6.8.0/os_brick/caches/opencas.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/constants.py` & `os-brick-6.8.0/os_brick/constants.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/encryptors/__init__.py` & `os-brick-6.8.0/os_brick/encryptors/__init__.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/encryptors/base.py` & `os-brick-6.8.0/os_brick/encryptors/base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/encryptors/cryptsetup.py` & `os-brick-6.8.0/os_brick/encryptors/cryptsetup.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/encryptors/luks.py` & `os-brick-6.8.0/os_brick/encryptors/luks.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/encryptors/nop.py` & `os-brick-6.8.0/os_brick/encryptors/nop.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/exception.py` & `os-brick-6.8.0/os_brick/exception.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/executor.py` & `os-brick-6.8.0/os_brick/executor.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/i18n.py` & `os-brick-6.8.0/os_brick/i18n.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/__init__.py` & `os-brick-6.8.0/os_brick/initiator/__init__.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connector.py` & `os-brick-6.8.0/os_brick/initiator/connector.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/base.py` & `os-brick-6.8.0/os_brick/initiator/connectors/base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/base_iscsi.py` & `os-brick-6.8.0/os_brick/initiator/connectors/base_iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/base_rbd.py` & `os-brick-6.8.0/os_brick/initiator/connectors/base_rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/fake.py` & `os-brick-6.8.0/os_brick/initiator/connectors/fake.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/fibre_channel.py` & `os-brick-6.8.0/os_brick/initiator/connectors/fibre_channel.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/fibre_channel_ppc64.py` & `os-brick-6.8.0/os_brick/initiator/connectors/fibre_channel_ppc64.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/fibre_channel_s390x.py` & `os-brick-6.8.0/os_brick/initiator/connectors/fibre_channel_s390x.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/gpfs.py` & `os-brick-6.8.0/os_brick/initiator/connectors/gpfs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/huawei.py` & `os-brick-6.8.0/os_brick/initiator/connectors/huawei.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/iscsi.py` & `os-brick-6.8.0/os_brick/initiator/connectors/iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/lightos.py` & `os-brick-6.8.0/os_brick/initiator/connectors/lightos.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/local.py` & `os-brick-6.8.0/os_brick/initiator/connectors/local.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/nvmeof.py` & `os-brick-6.8.0/os_brick/initiator/connectors/nvmeof.py`

 * *Files 0% similar despite different names*

```diff
@@ -815,16 +815,21 @@
 
     def _get_host_uuid(self) -> Optional[str]:
         """Get the UUID of the first mounted filesystem."""
         cmd = ('findmnt', '-v', '/', '-n', '-o', 'SOURCE')
         try:
             lines, err = self._execute(
                 *cmd, run_as_root=True, root_helper=self._root_helper)
+            source = lines.split('\n')[0]
+            # In a container this could be 'overlay', which causes the blkid
+            # command to fail.
+            if source == "overlay":
+                return None
             blkid_cmd = (
-                'blkid', lines.split('\n')[0], '-s', 'UUID', '-o', 'value')
+                'blkid', source, '-s', 'UUID', '-o', 'value')
             lines, _err = self._execute(
                 *blkid_cmd, run_as_root=True, root_helper=self._root_helper)
             return lines.split('\n')[0]
         except putils.ProcessExecutionError as e:
             LOG.warning(
                 "Process execution error in _get_host_uuid: %s", e)
             return None
```

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/rbd.py` & `os-brick-6.8.0/os_brick/initiator/connectors/rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/remotefs.py` & `os-brick-6.8.0/os_brick/initiator/connectors/remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/scaleio.py` & `os-brick-6.8.0/os_brick/initiator/connectors/scaleio.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/storpool.py` & `os-brick-6.8.0/os_brick/initiator/connectors/storpool.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/connectors/vmware.py` & `os-brick-6.8.0/os_brick/initiator/connectors/vmware.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/host_driver.py` & `os-brick-6.8.0/os_brick/initiator/host_driver.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/initiator_connector.py` & `os-brick-6.8.0/os_brick/initiator/initiator_connector.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/linuxfc.py` & `os-brick-6.8.0/os_brick/initiator/linuxfc.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/linuxrbd.py` & `os-brick-6.8.0/os_brick/initiator/linuxrbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/linuxscsi.py` & `os-brick-6.8.0/os_brick/initiator/linuxscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/utils.py` & `os-brick-6.8.0/os_brick/initiator/utils.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/windows/base.py` & `os-brick-6.8.0/os_brick/initiator/windows/base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/windows/fibre_channel.py` & `os-brick-6.8.0/os_brick/initiator/windows/fibre_channel.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/windows/iscsi.py` & `os-brick-6.8.0/os_brick/initiator/windows/iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/windows/rbd.py` & `os-brick-6.8.0/os_brick/initiator/windows/rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/initiator/windows/smbfs.py` & `os-brick-6.8.0/os_brick/initiator/windows/smbfs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/local_dev/lvm.py` & `os-brick-6.8.0/os_brick/local_dev/lvm.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/opts.py` & `os-brick-6.8.0/os_brick/opts.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/privileged/__init__.py` & `os-brick-6.8.0/os_brick/privileged/__init__.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/privileged/lightos.py` & `os-brick-6.8.0/os_brick/privileged/lightos.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/privileged/nvmeof.py` & `os-brick-6.8.0/os_brick/privileged/nvmeof.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/privileged/rbd.py` & `os-brick-6.8.0/os_brick/privileged/rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/privileged/rootwrap.py` & `os-brick-6.8.0/os_brick/privileged/rootwrap.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/privileged/scaleio.py` & `os-brick-6.8.0/os_brick/privileged/scaleio.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/remotefs/remotefs.py` & `os-brick-6.8.0/os_brick/remotefs/remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/remotefs/windows_remotefs.py` & `os-brick-6.8.0/os_brick/remotefs/windows_remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/base.py` & `os-brick-6.8.0/os_brick/tests/base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/caches/test_init.py` & `os-brick-6.8.0/os_brick/tests/caches/test_init.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/caches/test_opencas.py` & `os-brick-6.8.0/os_brick/tests/caches/test_opencas.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/encryptors/test_base.py` & `os-brick-6.8.0/os_brick/tests/encryptors/test_base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/encryptors/test_cryptsetup.py` & `os-brick-6.8.0/os_brick/tests/encryptors/test_cryptsetup.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/encryptors/test_luks.py` & `os-brick-6.8.0/os_brick/tests/encryptors/test_luks.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/encryptors/test_nop.py` & `os-brick-6.8.0/os_brick/tests/encryptors/test_nop.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_base_iscsi.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_base_iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_base_rbd.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_base_rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_fibre_channel.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_fibre_channel.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_fibre_channel_ppc64.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_fibre_channel_ppc64.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_fibre_channel_s390x.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_fibre_channel_s390x.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_gpfs.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_gpfs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_huawei.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_huawei.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_iscsi.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_iser.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_iser.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_lightos.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_lightos.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_local.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_local.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_nvmeof.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_nvmeof.py`

 * *Files 0% similar despite different names*

```diff
@@ -914,26 +914,34 @@
         nvme_present = self.connector.nvme_present()
         log = mock_log.debug if isinstance(exc, OSError) else mock_log.warning
         log.assert_called_once()
         self.assertFalse(nvme_present)
 
     @mock.patch.object(nvmeof.NVMeOFConnector, '_execute', autospec=True)
     def test_get_sysuuid_without_newline(self, mock_execute):
-        mock_execute.return_value = (
-            "9126E942-396D-11E7-B0B7-A81E84C186D1\n", "")
+        mock_execute.side_effect = [
+            ("/dev/sda1", ""),
+            ("9126E942-396D-11E7-B0B7-A81E84C186D1\n", "")
+        ]
         uuid = self.connector._get_host_uuid()
         expected_uuid = "9126E942-396D-11E7-B0B7-A81E84C186D1"
         self.assertEqual(expected_uuid, uuid)
 
     @mock.patch.object(nvmeof.NVMeOFConnector, '_execute', autospec=True)
     def test_get_sysuuid_err(self, mock_execute):
         mock_execute.side_effect = putils.ProcessExecutionError()
         uuid = self.connector._get_host_uuid()
         self.assertIsNone(uuid)
 
+    @mock.patch.object(nvmeof.NVMeOFConnector, '_execute', autospec=True)
+    def test_get_sysuuid_overlay(self, mock_execute):
+        mock_execute.return_value = ("overlay\n", "")
+        uuid = self.connector._get_host_uuid()
+        self.assertIsNone(uuid)
+
     @mock.patch.object(utils, 'get_nvme_host_id',
                        return_value=SYS_UUID)
     @mock.patch.object(nvmeof.NVMeOFConnector,
                        '_is_native_multipath_supported',
                        return_value=True)
     @mock.patch.object(nvmeof.NVMeOFConnector, 'nvme_present',
                        return_value=True)
```

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_rbd.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_remotefs.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_scaleio.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_scaleio.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_storpool.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_storpool.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/connectors/test_vmware.py` & `os-brick-6.8.0/os_brick/tests/initiator/connectors/test_vmware.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/test_connector.py` & `os-brick-6.8.0/os_brick/tests/initiator/test_connector.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/test_host_driver.py` & `os-brick-6.8.0/os_brick/tests/initiator/test_host_driver.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/test_linuxfc.py` & `os-brick-6.8.0/os_brick/tests/initiator/test_linuxfc.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/test_linuxrbd.py` & `os-brick-6.8.0/os_brick/tests/initiator/test_linuxrbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/test_linuxscsi.py` & `os-brick-6.8.0/os_brick/tests/initiator/test_linuxscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/initiator/test_utils.py` & `os-brick-6.8.0/os_brick/tests/initiator/test_utils.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/local_dev/fake_lvm.py` & `os-brick-6.8.0/os_brick/tests/local_dev/fake_lvm.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/local_dev/test_brick_lvm.py` & `os-brick-6.8.0/os_brick/tests/local_dev/test_brick_lvm.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/privileged/test_nvmeof.py` & `os-brick-6.8.0/os_brick/tests/privileged/test_nvmeof.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/privileged/test_rbd.py` & `os-brick-6.8.0/os_brick/tests/privileged/test_rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/privileged/test_rootwrap.py` & `os-brick-6.8.0/os_brick/tests/privileged/test_rootwrap.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/remotefs/test_remotefs.py` & `os-brick-6.8.0/os_brick/tests/remotefs/test_remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/remotefs/test_windows_remotefs.py` & `os-brick-6.8.0/os_brick/tests/remotefs/test_windows_remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/test_brick.py` & `os-brick-6.8.0/os_brick/tests/test_brick.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/test_exception.py` & `os-brick-6.8.0/os_brick/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/test_executor.py` & `os-brick-6.8.0/os_brick/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/test_utils.py` & `os-brick-6.8.0/os_brick/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/windows/fake_win_conn.py` & `os-brick-6.8.0/os_brick/tests/windows/fake_win_conn.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/windows/test_base.py` & `os-brick-6.8.0/os_brick/tests/windows/test_base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/windows/test_base_connector.py` & `os-brick-6.8.0/os_brick/tests/windows/test_base_connector.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/windows/test_factory.py` & `os-brick-6.8.0/os_brick/tests/windows/test_factory.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/windows/test_fibre_channel.py` & `os-brick-6.8.0/os_brick/tests/windows/test_fibre_channel.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/windows/test_iscsi.py` & `os-brick-6.8.0/os_brick/tests/windows/test_iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/windows/test_rbd.py` & `os-brick-6.8.0/os_brick/tests/windows/test_rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/tests/windows/test_smbfs.py` & `os-brick-6.8.0/os_brick/tests/windows/test_smbfs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/utils.py` & `os-brick-6.8.0/os_brick/utils.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick/version.py` & `os-brick-6.8.0/os_brick/version.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/os_brick.egg-info/PKG-INFO` & `os-brick-6.8.0/os_brick.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: os-brick
-Version: 6.7.0
+Version: 6.8.0
 Summary: OpenStack Cinder brick library for managing local volume attaches
 Home-page: https://docs.openstack.org/os-brick/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: OpenStack Cinder brick library for managing local volume attaches
 Platform: UNKNOWN
@@ -13,12 +13,11 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
```

### Comparing `os-brick-6.7.0/os_brick.egg-info/SOURCES.txt` & `os-brick-6.8.0/os_brick.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,15 @@
 releasenotes/notes/fc-always-check-single-wwnn-1595689da0eb673b.yaml
 releasenotes/notes/fc-flush-single-path-22ed6cc7b56a6d9b.yaml
 releasenotes/notes/fc-force-disconnect-1a33cf46c233dd04.yaml
 releasenotes/notes/fix-extend-multipath-a308d333061665fd.yaml
 releasenotes/notes/fix-fc-scan-too-broad-3c576e1846b7f05f.yaml
 releasenotes/notes/fix-fc-scanning-9164da9eb42aaed0.yaml
 releasenotes/notes/fix-generate-hostnqn-in-case-old-nvmecli.yaml
+releasenotes/notes/fix-host-uuid-warning-3814b7e47bde8010.yaml
 releasenotes/notes/fix-multipath-disconnect-819d01e6e981883e.yaml
 releasenotes/notes/fix-nvme-issues-8dfc15cb691389fe.yaml
 releasenotes/notes/improve-get_sysfs_wwn-df38ea88cdcdcc94.yaml
 releasenotes/notes/improve-iscsi-multipath-detection-f36f28a993f61936.yaml
 releasenotes/notes/introduce-encryption-provider-constants-a7cd0ce58da2bae8.yaml
 releasenotes/notes/iscsi_manual_scan_support-d64a1c3c8e1986b4.yaml
 releasenotes/notes/local-attach-in-rbd-connector-c06347fb164b084a.yaml
@@ -245,14 +246,15 @@
 releasenotes/notes/update-nvmeof-connector-6260a658c15a9a6e.yaml
 releasenotes/notes/ussuri-release-979d709dfa7df068.yaml
 releasenotes/notes/veritas-hyperscale-connector-fe56cec68b1947cd.yaml
 releasenotes/notes/vmware-vmdk-connector-19e6999e6cae43cd.yaml
 releasenotes/notes/yoga-known-issues-f1248af0e328d63e.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/mitaka.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
```

### Comparing `os-brick-6.7.0/pylintrc` & `os-brick-6.8.0/pylintrc`

 * *Files 20% similar despite different names*

```diff
@@ -26,13 +26,7 @@
 max-public-methods=100
 min-public-methods=0
 max-args=6
 
 [Variables]
 
 dummy-variables-rgx=_
-
-[Typecheck]
-# Disable warnings on the HTTPSConnection classes because pylint doesn't
-# support importing from six.moves yet, see:
-# https://bitbucket.org/logilab/pylint/issue/550/
-ignored-classes=HTTPSConnection
```

### Comparing `os-brick-6.7.0/releasenotes/notes/bug-1823200-scaleio-upgrade-3e83b5c9dd148714.yaml` & `os-brick-6.8.0/releasenotes/notes/bug-1823200-scaleio-upgrade-3e83b5c9dd148714.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/releasenotes/notes/bug-1823200-victoria-b414a1806cba3998.yaml` & `os-brick-6.8.0/releasenotes/notes/bug-1823200-victoria-b414a1806cba3998.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/releasenotes/notes/bug-1865754-ceph-octopus-compatibility-0aa9b8bc1b028301.yaml` & `os-brick-6.8.0/releasenotes/notes/bug-1865754-ceph-octopus-compatibility-0aa9b8bc1b028301.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/releasenotes/notes/introduce-encryption-provider-constants-a7cd0ce58da2bae8.yaml` & `os-brick-6.8.0/releasenotes/notes/introduce-encryption-provider-constants-a7cd0ce58da2bae8.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/releasenotes/notes/lock_path-c1c58a253391b41c.yaml` & `os-brick-6.8.0/releasenotes/notes/lock_path-c1c58a253391b41c.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/releasenotes/notes/nvmeof-consolidate-004dbe3a98f6f815.yaml` & `os-brick-6.8.0/releasenotes/notes/nvmeof-consolidate-004dbe3a98f6f815.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/releasenotes/source/conf.py` & `os-brick-6.8.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/requirements.txt` & `os-brick-6.8.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/setup.cfg` & `os-brick-6.8.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [files]
 packages = 
 	os_brick
```

### Comparing `os-brick-6.7.0/setup.py` & `os-brick-6.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/test-requirements.txt` & `os-brick-6.8.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/tools/coding-checks.sh` & `os-brick-6.8.0/tools/coding-checks.sh`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/tools/generate_connector_list.py` & `os-brick-6.8.0/tools/generate_connector_list.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/tools/lintstack.py` & `os-brick-6.8.0/tools/lintstack.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/tools/lintstack.sh` & `os-brick-6.8.0/tools/lintstack.sh`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/tools/mypywrap.sh` & `os-brick-6.8.0/tools/mypywrap.sh`

 * *Files identical despite different names*

### Comparing `os-brick-6.7.0/tox.ini` & `os-brick-6.8.0/tox.ini`

 * *Files identical despite different names*

