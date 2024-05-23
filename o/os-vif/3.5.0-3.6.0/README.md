# Comparing `tmp/os_vif-3.5.0.tar.gz` & `tmp/os_vif-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os_vif-3.5.0.tar", last modified: Tue Feb 27 14:15:12 2024, max compression
+gzip compressed data, was "os_vif-3.6.0.tar", last modified: Thu May 23 08:16:44 2024, max compression
```

## Comparing `os_vif-3.5.0.tar` & `os_vif-3.6.0.tar`

### file list

```diff
@@ -1,224 +1,225 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.605554 os_vif-3.5.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-02-27 14:14:12.000000 os_vif-3.5.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-02-27 14:14:12.000000 os_vif-3.5.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2024-02-27 14:14:12.000000 os_vif-3.5.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5253 2024-02-27 14:14:12.000000 os_vif-3.5.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3215 2024-02-27 14:15:12.000000 os_vif-3.5.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      599 2024-02-27 14:14:12.000000 os_vif-3.5.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13628 2024-02-27 14:15:12.000000 os_vif-3.5.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-27 14:14:12.000000 os_vif-3.5.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-02-27 14:14:12.000000 os_vif-3.5.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2029 2024-02-27 14:15:12.605554 os_vif-3.5.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      843 2024-02-27 14:14:12.000000 os_vif-3.5.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2024-02-27 14:14:12.000000 os_vif-3.5.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.561555 os_vif-3.5.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-02-27 14:14:12.000000 os_vif-3.5.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.561555 os_vif-3.5.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2024-02-27 14:14:12.000000 os_vif-3.5.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.561555 os_vif-3.5.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2100 2024-02-27 14:14:12.000000 os_vif-3.5.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2024-02-27 14:14:12.000000 os_vif-3.5.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.561555 os_vif-3.5.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7078 2024-02-27 14:14:12.000000 os_vif-3.5.0/doc/source/reference/glossary.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.561555 os_vif-3.5.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2803 2024-02-27 14:14:12.000000 os_vif-3.5.0/doc/source/user/host-info.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.561555 os_vif-3.5.0/doc/source/user/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-02-27 14:14:12.000000 os_vif-3.5.0/doc/source/user/plugins/linux-bridge.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2024-02-27 14:14:12.000000 os_vif-3.5.0/doc/source/user/plugins/noop.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2024-02-27 14:14:12.000000 os_vif-3.5.0/doc/source/user/plugins/ovs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2352 2024-02-27 14:14:12.000000 os_vif-3.5.0/doc/source/user/usage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2164 2024-02-27 14:14:12.000000 os_vif-3.5.0/doc/source/user/vif-types.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.565555 os_vif-3.5.0/os_vif/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5484 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1040 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.565555 os_vif-3.5.0/os_vif/internal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/internal/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.565555 os_vif-3.5.0/os_vif/internal/ip/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/internal/ip/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/internal/ip/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2787 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/internal/ip/ip_command.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.569555 os_vif-3.5.0/os_vif/internal/ip/linux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/internal/ip/linux/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5511 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/internal/ip/linux/impl_pyroute2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.569555 os_vif-3.5.0/os_vif/internal/ip/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/internal/ip/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1745 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/internal/ip/windows/impl_netifaces.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.569555 os_vif-3.5.0/os_vif/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/objects/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1761 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/objects/fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1282 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/objects/fixed_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6698 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/objects/host_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/objects/instance_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2134 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/objects/network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1352 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/objects/route.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/objects/subnet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21668 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/objects/vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3032 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.569555 os_vif-3.5.0/os_vif/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.569555 os_vif-3.5.0/os_vif/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5005 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.573555 os_vif-3.5.0/os_vif/tests/functional/internal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/functional/internal/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.573555 os_vif-3.5.0/os_vif/tests/functional/internal/command/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/functional/internal/command/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.573555 os_vif-3.5.0/os_vif/tests/functional/internal/command/ip/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/functional/internal/command/ip/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9982 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/functional/internal/command/ip/test_impl_pyroute2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/functional/privsep.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.573555 os_vif-3.5.0/os_vif/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/unit/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.573555 os_vif-3.5.0/os_vif/tests/unit/internal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/unit/internal/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.573555 os_vif-3.5.0/os_vif/tests/unit/internal/ip/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/unit/internal/ip/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.577555 os_vif-3.5.0/os_vif/tests/unit/internal/ip/linux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/unit/internal/ip/linux/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7364 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/unit/internal/ip/linux/test_impl_pyroute2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1415 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/unit/internal/ip/test_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.577555 os_vif-3.5.0/os_vif/tests/unit/internal/ip/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/unit/internal/ip/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1992 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/unit/internal/ip/windows/test_impl_netifaces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3137 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/unit/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1335 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/unit/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7576 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/unit/test_host_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3709 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/unit/test_objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6609 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/unit/test_os_vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18000 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/tests/unit/test_vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2024-02-27 14:14:12.000000 os_vif-3.5.0/os_vif/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.565555 os_vif-3.5.0/os_vif.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2029 2024-02-27 14:15:12.000000 os_vif-3.5.0/os_vif.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6851 2024-02-27 14:15:12.000000 os_vif-3.5.0/os_vif.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-27 14:15:12.000000 os_vif-3.5.0/os_vif.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-02-27 14:15:12.000000 os_vif-3.5.0/os_vif.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-27 14:15:12.000000 os_vif-3.5.0/os_vif.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-27 14:15:12.000000 os_vif-3.5.0/os_vif.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2024-02-27 14:15:12.000000 os_vif-3.5.0/os_vif.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2024-02-27 14:15:12.000000 os_vif-3.5.0/os_vif.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.553555 os_vif-3.5.0/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.577555 os_vif-3.5.0/playbooks/openstack-tox-functional-ovs-with-sudo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2024-02-27 14:14:12.000000 os_vif-3.5.0/playbooks/openstack-tox-functional-ovs-with-sudo/Debian.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2024-02-27 14:14:12.000000 os_vif-3.5.0/playbooks/openstack-tox-functional-ovs-with-sudo/Gentoo.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-02-27 14:14:12.000000 os_vif-3.5.0/playbooks/openstack-tox-functional-ovs-with-sudo/RedHat.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-02-27 14:14:12.000000 os_vif-3.5.0/playbooks/openstack-tox-functional-ovs-with-sudo/Suse.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      566 2024-02-27 14:14:12.000000 os_vif-3.5.0/playbooks/openstack-tox-functional-ovs-with-sudo/pre.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.553555 os_vif-3.5.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.589554 os_vif-3.5.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/OVSVif-hybrid-unplug-f37bf57bc8e913de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/add-abstract-ovsdb-api-8f04df58d4ed5b73.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/add-fast-path-vhostuser-support-fe87e558326909b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/add-no-op-plugin-763a6703e7328a24.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/add-ovs-representor-portprofile-5f8290e5a40bf0a4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/add-ovs-vhostuser-support-2ba8de51c1f3a244.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/add-ovsdb-native-322fffb49c91503d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2079 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/always-plug-vifs-for-ovs-1d033fc49a9c6c4e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/brctl-removal-a5b0e69b865afa57.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/bug-1892132-812e6d5ce0588ebb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/contextlib-and-nested-with-statements-2747a9ebb9a5bfd7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2011 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/default-qos-policy-for-ovs-26f8806046a59c82.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/default-to-native-ovsdb-driver-112fb5adf6e19a30.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/deprecate-windows-support-49f5ca1b1a1f4d66.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/do-not-force-mac-ageing-c6e8d750130c5740.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/drop-py36-support-0e9b07073f6ad73f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/drop-python2-support-7a4bc7d31253c1e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/ensure-ovs-bridge-a0c1b51f469c92d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/extend-vhostuser-object-fada14a1457d4e56.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/fix-broken-dataplane-on-nova-restart-with-isolate_vif-71617a41741b33e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/fix-ovs-plugin-describe-049750609559f1ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/fix-stevedore-entrypoints-8002ec7a5166c977.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/fix-vif-openvswitch-fa0d19be9dd668e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/generic-datapath-offloads-41cabb6842b41533.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/initial-release-2c71d6bbf55f763b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/oslo-config-opts-entrypoints-e83f907b686d774a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1659 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/per-port-bridge-c6a50179a0256de3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/port-profile-info-linux-bridge-4800f5a0b7328615.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/port-profile-info-ovs-63b46a3eafc11de2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/prevent-lb-reply-arp-6459133bfb056069.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/remove_iptools_implementation-2eb866573a680e61.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/revert-always-plug-port-for-ovs-hybrid-plug-false-dc015985cbc5443b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/vhost-user-mtu-support-cbc7d02a6665fab1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/notes/vhost-user-reconnect-fa4cbb731b787f71.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.593554 os_vif-3.5.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.593554 os_vif-3.5.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.593554 os_vif-3.5.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-27 14:14:12.000000 os_vif-3.5.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2024-02-27 14:14:12.000000 os_vif-3.5.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2024-02-27 14:15:12.605554 os_vif-3.5.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2024-02-27 14:14:12.000000 os_vif-3.5.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-02-27 14:14:12.000000 os_vif-3.5.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2437 2024-02-27 14:14:12.000000 os_vif-3.5.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.593554 os_vif-3.5.0/vif_plug_linux_bridge/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_linux_bridge/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_linux_bridge/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20641 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_linux_bridge/iptables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4949 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_linux_bridge/linux_bridge.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9481 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_linux_bridge/linux_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_linux_bridge/privsep.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.597554 os_vif-3.5.0/vif_plug_linux_bridge/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_linux_bridge/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.597554 os_vif-3.5.0/vif_plug_linux_bridge/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_linux_bridge/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6740 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_linux_bridge/tests/unit/test_linux_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4803 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_linux_bridge/tests/unit/test_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.597554 os_vif-3.5.0/vif_plug_noop/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_noop/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_noop/noop.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.597554 os_vif-3.5.0/vif_plug_noop/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_noop/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.597554 os_vif-3.5.0/vif_plug_noop/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_noop/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_noop/tests/unit/test_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.601554 os_vif-3.5.0/vif_plug_ovs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1328 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14289 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/linux_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24166 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/ovs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.601554 os_vif-3.5.0/vif_plug_ovs/ovsdb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/ovsdb/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/ovsdb/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3028 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/ovsdb/impl_idl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14437 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/ovsdb/impl_vsctl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10599 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/ovsdb/ovsdb_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1100 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/privsep.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.601554 os_vif-3.5.0/vif_plug_ovs/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.601554 os_vif-3.5.0/vif_plug_ovs/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1872 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.601554 os_vif-3.5.0/vif_plug_ovs/tests/functional/ovsdb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/tests/functional/ovsdb/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13513 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/tests/functional/ovsdb/test_ovsdb_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6648 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/tests/functional/test_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.601554 os_vif-3.5.0/vif_plug_ovs/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:15:12.605554 os_vif-3.5.0/vif_plug_ovs/tests/unit/ovsdb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/tests/unit/ovsdb/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10705 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/tests/unit/ovsdb/test_ovsdb_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17532 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/tests/unit/test_linux_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33303 2024-02-27 14:14:12.000000 os_vif-3.5.0/vif_plug_ovs/tests/unit/test_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.423886 os_vif-3.6.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-05-23 08:16:12.000000 os_vif-3.6.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-05-23 08:16:12.000000 os_vif-3.6.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2024-05-23 08:16:12.000000 os_vif-3.6.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5253 2024-05-23 08:16:12.000000 os_vif-3.6.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3215 2024-05-23 08:16:44.000000 os_vif-3.6.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      599 2024-05-23 08:16:12.000000 os_vif-3.6.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13917 2024-05-23 08:16:44.000000 os_vif-3.6.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-05-23 08:16:12.000000 os_vif-3.6.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-23 08:16:12.000000 os_vif-3.6.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2080 2024-05-23 08:16:44.423886 os_vif-3.6.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      843 2024-05-23 08:16:12.000000 os_vif-3.6.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2024-05-23 08:16:12.000000 os_vif-3.6.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.387888 os_vif-3.6.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-05-23 08:16:12.000000 os_vif-3.6.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.387888 os_vif-3.6.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2024-05-23 08:16:12.000000 os_vif-3.6.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.387888 os_vif-3.6.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2100 2024-05-23 08:16:12.000000 os_vif-3.6.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2024-05-23 08:16:12.000000 os_vif-3.6.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.387888 os_vif-3.6.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7078 2024-05-23 08:16:12.000000 os_vif-3.6.0/doc/source/reference/glossary.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.391887 os_vif-3.6.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2803 2024-05-23 08:16:12.000000 os_vif-3.6.0/doc/source/user/host-info.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.391887 os_vif-3.6.0/doc/source/user/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-05-23 08:16:12.000000 os_vif-3.6.0/doc/source/user/plugins/linux-bridge.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2024-05-23 08:16:12.000000 os_vif-3.6.0/doc/source/user/plugins/noop.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2024-05-23 08:16:12.000000 os_vif-3.6.0/doc/source/user/plugins/ovs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2352 2024-05-23 08:16:12.000000 os_vif-3.6.0/doc/source/user/usage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2164 2024-05-23 08:16:12.000000 os_vif-3.6.0/doc/source/user/vif-types.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.391887 os_vif-3.6.0/os_vif/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5484 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1040 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.391887 os_vif-3.6.0/os_vif/internal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/internal/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.395887 os_vif-3.6.0/os_vif/internal/ip/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/internal/ip/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/internal/ip/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2787 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/internal/ip/ip_command.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.395887 os_vif-3.6.0/os_vif/internal/ip/linux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/internal/ip/linux/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5511 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/internal/ip/linux/impl_pyroute2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.395887 os_vif-3.6.0/os_vif/internal/ip/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/internal/ip/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1745 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/internal/ip/windows/impl_netifaces.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.395887 os_vif-3.6.0/os_vif/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/objects/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1761 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/objects/fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1282 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/objects/fixed_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6698 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/objects/host_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/objects/instance_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2134 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/objects/network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1352 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/objects/route.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/objects/subnet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21668 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/objects/vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3032 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.395887 os_vif-3.6.0/os_vif/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.395887 os_vif-3.6.0/os_vif/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5005 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.395887 os_vif-3.6.0/os_vif/tests/functional/internal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/functional/internal/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.395887 os_vif-3.6.0/os_vif/tests/functional/internal/command/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/functional/internal/command/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.399887 os_vif-3.6.0/os_vif/tests/functional/internal/command/ip/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/functional/internal/command/ip/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9982 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/functional/internal/command/ip/test_impl_pyroute2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/functional/privsep.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.399887 os_vif-3.6.0/os_vif/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.399887 os_vif-3.6.0/os_vif/tests/unit/internal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/unit/internal/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.399887 os_vif-3.6.0/os_vif/tests/unit/internal/ip/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/unit/internal/ip/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.399887 os_vif-3.6.0/os_vif/tests/unit/internal/ip/linux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/unit/internal/ip/linux/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7364 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/unit/internal/ip/linux/test_impl_pyroute2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1415 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/unit/internal/ip/test_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.399887 os_vif-3.6.0/os_vif/tests/unit/internal/ip/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/unit/internal/ip/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1992 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/unit/internal/ip/windows/test_impl_netifaces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3137 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/unit/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1335 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/unit/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7576 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/unit/test_host_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3709 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/unit/test_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6609 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/unit/test_os_vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18000 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/tests/unit/test_vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2024-05-23 08:16:12.000000 os_vif-3.6.0/os_vif/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.391887 os_vif-3.6.0/os_vif.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2080 2024-05-23 08:16:44.000000 os_vif-3.6.0/os_vif.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6882 2024-05-23 08:16:44.000000 os_vif-3.6.0/os_vif.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:16:44.000000 os_vif-3.6.0/os_vif.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-05-23 08:16:44.000000 os_vif-3.6.0/os_vif.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:16:44.000000 os_vif-3.6.0/os_vif.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-23 08:16:44.000000 os_vif-3.6.0/os_vif.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2024-05-23 08:16:44.000000 os_vif-3.6.0/os_vif.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2024-05-23 08:16:44.000000 os_vif-3.6.0/os_vif.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.383888 os_vif-3.6.0/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.399887 os_vif-3.6.0/playbooks/openstack-tox-functional-ovs-with-sudo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2024-05-23 08:16:12.000000 os_vif-3.6.0/playbooks/openstack-tox-functional-ovs-with-sudo/Debian.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2024-05-23 08:16:12.000000 os_vif-3.6.0/playbooks/openstack-tox-functional-ovs-with-sudo/Gentoo.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-05-23 08:16:12.000000 os_vif-3.6.0/playbooks/openstack-tox-functional-ovs-with-sudo/RedHat.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-05-23 08:16:12.000000 os_vif-3.6.0/playbooks/openstack-tox-functional-ovs-with-sudo/Suse.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      566 2024-05-23 08:16:12.000000 os_vif-3.6.0/playbooks/openstack-tox-functional-ovs-with-sudo/pre.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.383888 os_vif-3.6.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.407887 os_vif-3.6.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/OVSVif-hybrid-unplug-f37bf57bc8e913de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/add-abstract-ovsdb-api-8f04df58d4ed5b73.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/add-fast-path-vhostuser-support-fe87e558326909b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/add-no-op-plugin-763a6703e7328a24.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/add-ovs-representor-portprofile-5f8290e5a40bf0a4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/add-ovs-vhostuser-support-2ba8de51c1f3a244.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/add-ovsdb-native-322fffb49c91503d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2079 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/always-plug-vifs-for-ovs-1d033fc49a9c6c4e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/brctl-removal-a5b0e69b865afa57.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/bug-1892132-812e6d5ce0588ebb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/contextlib-and-nested-with-statements-2747a9ebb9a5bfd7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2011 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/default-qos-policy-for-ovs-26f8806046a59c82.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/default-to-native-ovsdb-driver-112fb5adf6e19a30.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/deprecate-windows-support-49f5ca1b1a1f4d66.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/do-not-force-mac-ageing-c6e8d750130c5740.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/drop-py36-support-0e9b07073f6ad73f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/drop-python2-support-7a4bc7d31253c1e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/ensure-ovs-bridge-a0c1b51f469c92d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/extend-vhostuser-object-fada14a1457d4e56.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/fix-broken-dataplane-on-nova-restart-with-isolate_vif-71617a41741b33e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/fix-ovs-plugin-describe-049750609559f1ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/fix-stevedore-entrypoints-8002ec7a5166c977.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/fix-vif-openvswitch-fa0d19be9dd668e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/generic-datapath-offloads-41cabb6842b41533.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/initial-release-2c71d6bbf55f763b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/oslo-config-opts-entrypoints-e83f907b686d774a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1659 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/per-port-bridge-c6a50179a0256de3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/port-profile-info-linux-bridge-4800f5a0b7328615.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/port-profile-info-ovs-63b46a3eafc11de2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/prevent-lb-reply-arp-6459133bfb056069.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/remove_iptools_implementation-2eb866573a680e61.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/revert-always-plug-port-for-ovs-hybrid-plug-false-dc015985cbc5443b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/vhost-user-mtu-support-cbc7d02a6665fab1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/notes/vhost-user-reconnect-fa4cbb731b787f71.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.411886 os_vif-3.6.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.411886 os_vif-3.6.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.415886 os_vif-3.6.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-23 08:16:12.000000 os_vif-3.6.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2024-05-23 08:16:12.000000 os_vif-3.6.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2024-05-23 08:16:44.423886 os_vif-3.6.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2024-05-23 08:16:12.000000 os_vif-3.6.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-05-23 08:16:12.000000 os_vif-3.6.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2296 2024-05-23 08:16:12.000000 os_vif-3.6.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.415886 os_vif-3.6.0/vif_plug_linux_bridge/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_linux_bridge/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_linux_bridge/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20641 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_linux_bridge/iptables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4949 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_linux_bridge/linux_bridge.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9481 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_linux_bridge/linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_linux_bridge/privsep.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.415886 os_vif-3.6.0/vif_plug_linux_bridge/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_linux_bridge/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.415886 os_vif-3.6.0/vif_plug_linux_bridge/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_linux_bridge/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6740 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_linux_bridge/tests/unit/test_linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4803 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_linux_bridge/tests/unit/test_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.415886 os_vif-3.6.0/vif_plug_noop/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_noop/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_noop/noop.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.415886 os_vif-3.6.0/vif_plug_noop/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_noop/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.419886 os_vif-3.6.0/vif_plug_noop/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_noop/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_noop/tests/unit/test_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.419886 os_vif-3.6.0/vif_plug_ovs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1328 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14289 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24166 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/ovs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.419886 os_vif-3.6.0/vif_plug_ovs/ovsdb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/ovsdb/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/ovsdb/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3028 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/ovsdb/impl_idl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14437 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/ovsdb/impl_vsctl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10599 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/ovsdb/ovsdb_lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1100 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/privsep.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.419886 os_vif-3.6.0/vif_plug_ovs/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.419886 os_vif-3.6.0/vif_plug_ovs/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1872 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.419886 os_vif-3.6.0/vif_plug_ovs/tests/functional/ovsdb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/tests/functional/ovsdb/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13513 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/tests/functional/ovsdb/test_ovsdb_lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6648 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/tests/functional/test_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.419886 os_vif-3.6.0/vif_plug_ovs/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:44.423886 os_vif-3.6.0/vif_plug_ovs/tests/unit/ovsdb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/tests/unit/ovsdb/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10705 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/tests/unit/ovsdb/test_ovsdb_lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17532 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/tests/unit/test_linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33303 2024-05-23 08:16:12.000000 os_vif-3.6.0/vif_plug_ovs/tests/unit/test_plugin.py
```

### Comparing `os_vif-3.5.0/.zuul.yaml` & `os_vif-3.6.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/AUTHORS` & `os_vif-3.6.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/CONTRIBUTING.rst` & `os_vif-3.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/ChangeLog` & `os_vif-3.6.0/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 CHANGES
 =======
 
+3.6.0
+-----
+
+* reno: Update master for unmaintained/zed
+* Update master for stable/2024.1
+* reno: Update master for unmaintained/xena
+* reno: Update master for unmaintained/wallaby
+* reno: Update master for unmaintained/victoria
+
 3.5.0
 -----
 
 * Drop wrong stacklevel
 * Fix missing or unnecessary dependencies
 * reno: Update master for unmaintained/yoga
+* tox: Drop envdir
+* Update python classifier in setup.cfg
 
 3.4.0
 -----
 
 * coveragerc: Remove non-existent path
 * Deprecate Windows support
```

### Comparing `os_vif-3.5.0/LICENSE` & `os_vif-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/PKG-INFO` & `os_vif-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: os_vif
-Version: 3.5.0
+Version: 3.6.0
 Summary: A library for plugging and unplugging virtual interfaces in OpenStack.
 Home-page: https://docs.openstack.org/os-vif/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -44,9 +44,10 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
```

### Comparing `os_vif-3.5.0/README.rst` & `os_vif-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/doc/source/conf.py` & `os_vif-3.6.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/doc/source/contributor/contributing.rst` & `os_vif-3.6.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/doc/source/index.rst` & `os_vif-3.6.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/doc/source/reference/glossary.rst` & `os_vif-3.6.0/doc/source/reference/glossary.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/doc/source/user/host-info.rst` & `os_vif-3.6.0/doc/source/user/host-info.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/doc/source/user/plugins/linux-bridge.rst` & `os_vif-3.6.0/doc/source/user/plugins/linux-bridge.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/doc/source/user/plugins/noop.rst` & `os_vif-3.6.0/doc/source/user/plugins/noop.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/doc/source/user/plugins/ovs.rst` & `os_vif-3.6.0/doc/source/user/plugins/ovs.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/doc/source/user/usage.rst` & `os_vif-3.6.0/doc/source/user/usage.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/doc/source/user/vif-types.rst` & `os_vif-3.6.0/doc/source/user/vif-types.rst`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/__init__.py` & `os_vif-3.6.0/os_vif/__init__.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/exception.py` & `os_vif-3.6.0/os_vif/exception.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/i18n.py` & `os_vif-3.6.0/os_vif/i18n.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/internal/__init__.py` & `os_vif-3.6.0/os_vif/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/internal/ip/api.py` & `os_vif-3.6.0/os_vif/internal/ip/api.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/internal/ip/ip_command.py` & `os_vif-3.6.0/os_vif/internal/ip/ip_command.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/internal/ip/linux/impl_pyroute2.py` & `os_vif-3.6.0/os_vif/internal/ip/linux/impl_pyroute2.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/internal/ip/windows/impl_netifaces.py` & `os_vif-3.6.0/os_vif/internal/ip/windows/impl_netifaces.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/objects/__init__.py` & `os_vif-3.6.0/os_vif/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/objects/base.py` & `os_vif-3.6.0/os_vif/objects/base.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/objects/fields.py` & `os_vif-3.6.0/os_vif/objects/fields.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/objects/fixed_ip.py` & `os_vif-3.6.0/os_vif/objects/fixed_ip.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/objects/host_info.py` & `os_vif-3.6.0/os_vif/objects/host_info.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/objects/instance_info.py` & `os_vif-3.6.0/os_vif/objects/instance_info.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/objects/network.py` & `os_vif-3.6.0/os_vif/objects/network.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/objects/route.py` & `os_vif-3.6.0/os_vif/objects/route.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/objects/subnet.py` & `os_vif-3.6.0/os_vif/objects/subnet.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/objects/vif.py` & `os_vif-3.6.0/os_vif/objects/vif.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/opts.py` & `os_vif-3.6.0/os_vif/opts.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/plugin.py` & `os_vif-3.6.0/os_vif/plugin.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/tests/functional/base.py` & `os_vif-3.6.0/os_vif/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/tests/functional/internal/command/ip/test_impl_pyroute2.py` & `os_vif-3.6.0/os_vif/tests/functional/internal/command/ip/test_impl_pyroute2.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/tests/functional/privsep.py` & `os_vif-3.6.0/os_vif/tests/functional/privsep.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/tests/unit/base.py` & `os_vif-3.6.0/os_vif/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/tests/unit/internal/ip/linux/test_impl_pyroute2.py` & `os_vif-3.6.0/os_vif/tests/unit/internal/ip/linux/test_impl_pyroute2.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/tests/unit/internal/ip/test_api.py` & `os_vif-3.6.0/os_vif/tests/unit/internal/ip/test_api.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/tests/unit/internal/ip/windows/test_impl_netifaces.py` & `os_vif-3.6.0/os_vif/tests/unit/internal/ip/windows/test_impl_netifaces.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/tests/unit/test_base.py` & `os_vif-3.6.0/os_vif/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/tests/unit/test_exception.py` & `os_vif-3.6.0/os_vif/tests/unit/test_exception.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/tests/unit/test_host_info.py` & `os_vif-3.6.0/os_vif/tests/unit/test_host_info.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/tests/unit/test_objects.py` & `os_vif-3.6.0/os_vif/tests/unit/test_objects.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/tests/unit/test_os_vif.py` & `os_vif-3.6.0/os_vif/tests/unit/test_os_vif.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/tests/unit/test_vif.py` & `os_vif-3.6.0/os_vif/tests/unit/test_vif.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/utils.py` & `os_vif-3.6.0/os_vif/utils.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif/version.py` & `os_vif-3.6.0/os_vif/version.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/os_vif.egg-info/PKG-INFO` & `os_vif-3.6.0/os_vif.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: os-vif
-Version: 3.5.0
+Version: 3.6.0
 Summary: A library for plugging and unplugging virtual interfaces in OpenStack.
 Home-page: https://docs.openstack.org/os-vif/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -44,9 +44,10 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
```

### Comparing `os_vif-3.5.0/os_vif.egg-info/SOURCES.txt` & `os_vif-3.6.0/os_vif.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,15 @@
 releasenotes/notes/prevent-lb-reply-arp-6459133bfb056069.yaml
 releasenotes/notes/remove_iptools_implementation-2eb866573a680e61.yaml
 releasenotes/notes/revert-always-plug-port-for-ovs-hybrid-plug-false-dc015985cbc5443b.yaml
 releasenotes/notes/vhost-user-mtu-support-cbc7d02a6665fab1.yaml
 releasenotes/notes/vhost-user-reconnect-fa4cbb731b787f71.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
```

### Comparing `os_vif-3.5.0/playbooks/openstack-tox-functional-ovs-with-sudo/pre.yaml` & `os_vif-3.6.0/playbooks/openstack-tox-functional-ovs-with-sudo/pre.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/releasenotes/notes/add-ovsdb-native-322fffb49c91503d.yaml` & `os_vif-3.6.0/releasenotes/notes/add-ovsdb-native-322fffb49c91503d.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/releasenotes/notes/always-plug-vifs-for-ovs-1d033fc49a9c6c4e.yaml` & `os_vif-3.6.0/releasenotes/notes/always-plug-vifs-for-ovs-1d033fc49a9c6c4e.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/releasenotes/notes/brctl-removal-a5b0e69b865afa57.yaml` & `os_vif-3.6.0/releasenotes/notes/brctl-removal-a5b0e69b865afa57.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/releasenotes/notes/default-qos-policy-for-ovs-26f8806046a59c82.yaml` & `os_vif-3.6.0/releasenotes/notes/default-qos-policy-for-ovs-26f8806046a59c82.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/releasenotes/notes/default-to-native-ovsdb-driver-112fb5adf6e19a30.yaml` & `os_vif-3.6.0/releasenotes/notes/default-to-native-ovsdb-driver-112fb5adf6e19a30.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/releasenotes/notes/do-not-force-mac-ageing-c6e8d750130c5740.yaml` & `os_vif-3.6.0/releasenotes/notes/do-not-force-mac-ageing-c6e8d750130c5740.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/releasenotes/notes/generic-datapath-offloads-41cabb6842b41533.yaml` & `os_vif-3.6.0/releasenotes/notes/generic-datapath-offloads-41cabb6842b41533.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/releasenotes/notes/per-port-bridge-c6a50179a0256de3.yaml` & `os_vif-3.6.0/releasenotes/notes/per-port-bridge-c6a50179a0256de3.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/releasenotes/notes/revert-always-plug-port-for-ovs-hybrid-plug-false-dc015985cbc5443b.yaml` & `os_vif-3.6.0/releasenotes/notes/revert-always-plug-port-for-ovs-hybrid-plug-false-dc015985cbc5443b.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/releasenotes/notes/vhost-user-reconnect-fa4cbb731b787f71.yaml` & `os_vif-3.6.0/releasenotes/notes/vhost-user-reconnect-fa4cbb731b787f71.yaml`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/releasenotes/source/conf.py` & `os_vif-3.6.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/requirements.txt` & `os_vif-3.6.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/setup.cfg` & `os_vif-3.6.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 
 [files]
 packages = 
 	os_vif
 	vif_plug_linux_bridge
 	vif_plug_ovs
```

### Comparing `os_vif-3.5.0/setup.py` & `os_vif-3.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/tox.ini` & `os_vif-3.6.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -8,62 +8,57 @@
 deps =
   -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/requirements.txt
   -r{toxinidir}/test-requirements.txt
 commands = stestr run --exclude-regex ".tests.functional" {posargs}
 
 [testenv:functional]
-envdir = {toxworkdir}/shared
 setenv =
   {[testenv]setenv}
 commands =
   stestr run --exclude-regex ".tests.unit" {posargs}
 
 [testenv:docs]
 deps =
   -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/doc/requirements.txt
 commands = sphinx-build -W -b html doc/source doc/build/html
 
 [testenv:pdf-docs]
-envdir = {toxworkdir}/docs
 deps = {[testenv:docs]deps}
 allowlist_externals =
   rm
   make
 commands =
   rm -rf doc/build/pdf
   sphinx-build -W -b latex doc/source doc/build/pdf
   make -C doc/build/pdf
 
 [testenv:releasenotes]
-envdir = {toxworkdir}/docs
 deps = {[testenv:docs]deps}
 commands = sphinx-build -a -E -W -d releasenotes/build/doctrees -b html releasenotes/source releasenotes/build/html
 
 [testenv:venv]
 commands = {posargs}
 deps =
   {[testenv]deps}
   -r{toxinidir}/doc/requirements.txt
 
 [testenv:cover]
-envdir = {toxworkdir}/shared
 setenv =
   {[testenv]setenv}
   PYTHON=coverage run --source os_vif,vif_plug_linux_bridge,vif_plug_ovs,vif_plug_noop --parallel-mode
 commands =
   stestr run --exclude-regex ".tests.functional" {posargs}
   coverage combine
   coverage html -d cover
   coverage xml -o cover/coverage.xml
   coverage report
 
 [testenv:pep8]
-envdir = {toxworkdir}/shared
 deps =
   hacking>=3.0.1,<3.1.0
 commands = flake8
 
 [flake8]
 # E123, E125 skipped as they are invalid PEP-8.
 # Following checks are ignored on purpose.
```

### Comparing `os_vif-3.5.0/vif_plug_linux_bridge/constants.py` & `os_vif-3.6.0/vif_plug_linux_bridge/constants.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_linux_bridge/iptables.py` & `os_vif-3.6.0/vif_plug_linux_bridge/iptables.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_linux_bridge/linux_bridge.py` & `os_vif-3.6.0/vif_plug_linux_bridge/linux_bridge.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_linux_bridge/linux_net.py` & `os_vif-3.6.0/vif_plug_linux_bridge/linux_net.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_linux_bridge/privsep.py` & `os_vif-3.6.0/vif_plug_linux_bridge/privsep.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_linux_bridge/tests/unit/test_linux_net.py` & `os_vif-3.6.0/vif_plug_linux_bridge/tests/unit/test_linux_net.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_linux_bridge/tests/unit/test_plugin.py` & `os_vif-3.6.0/vif_plug_linux_bridge/tests/unit/test_plugin.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_noop/noop.py` & `os_vif-3.6.0/vif_plug_noop/noop.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_noop/tests/unit/test_plugin.py` & `os_vif-3.6.0/vif_plug_noop/tests/unit/test_plugin.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_ovs/constants.py` & `os_vif-3.6.0/vif_plug_ovs/constants.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_ovs/exception.py` & `os_vif-3.6.0/vif_plug_ovs/exception.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_ovs/linux_net.py` & `os_vif-3.6.0/vif_plug_ovs/linux_net.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_ovs/ovs.py` & `os_vif-3.6.0/vif_plug_ovs/ovs.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_ovs/ovsdb/api.py` & `os_vif-3.6.0/vif_plug_ovs/ovsdb/api.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_ovs/ovsdb/impl_idl.py` & `os_vif-3.6.0/vif_plug_ovs/ovsdb/impl_idl.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_ovs/ovsdb/impl_vsctl.py` & `os_vif-3.6.0/vif_plug_ovs/ovsdb/impl_vsctl.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_ovs/ovsdb/ovsdb_lib.py` & `os_vif-3.6.0/vif_plug_ovs/ovsdb/ovsdb_lib.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_ovs/privsep.py` & `os_vif-3.6.0/vif_plug_ovs/privsep.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_ovs/tests/functional/base.py` & `os_vif-3.6.0/vif_plug_ovs/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_ovs/tests/functional/ovsdb/test_ovsdb_lib.py` & `os_vif-3.6.0/vif_plug_ovs/tests/functional/ovsdb/test_ovsdb_lib.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_ovs/tests/functional/test_plugin.py` & `os_vif-3.6.0/vif_plug_ovs/tests/functional/test_plugin.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_ovs/tests/unit/ovsdb/test_ovsdb_lib.py` & `os_vif-3.6.0/vif_plug_ovs/tests/unit/ovsdb/test_ovsdb_lib.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_ovs/tests/unit/test_linux_net.py` & `os_vif-3.6.0/vif_plug_ovs/tests/unit/test_linux_net.py`

 * *Files identical despite different names*

### Comparing `os_vif-3.5.0/vif_plug_ovs/tests/unit/test_plugin.py` & `os_vif-3.6.0/vif_plug_ovs/tests/unit/test_plugin.py`

 * *Files identical despite different names*

