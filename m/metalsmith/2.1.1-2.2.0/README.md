# Comparing `tmp/metalsmith-2.1.1.tar.gz` & `tmp/metalsmith-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalsmith-2.1.1.tar", last modified: Thu Feb 22 15:05:18 2024, max compression
+gzip compressed data, was "metalsmith-2.2.0.tar", last modified: Thu May 23 07:55:54 2024, max compression
```

## Comparing `metalsmith-2.1.1.tar` & `metalsmith-2.2.0.tar`

### file list

```diff
@@ -1,139 +1,140 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.484915 metalsmith-2.1.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2024-02-22 15:04:47.000000 metalsmith-2.1.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6272 2024-02-22 15:04:47.000000 metalsmith-2.1.1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2024-02-22 15:05:18.000000 metalsmith-2.1.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11740 2024-02-22 15:05:18.000000 metalsmith-2.1.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2024-02-22 15:04:47.000000 metalsmith-2.1.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2952 2024-02-22 15:05:18.484915 metalsmith-2.1.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1559 2024-02-22 15:04:47.000000 metalsmith-2.1.1/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.464915 metalsmith-2.1.1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2024-02-22 15:04:47.000000 metalsmith-2.1.1/doc/joined-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2024-02-22 15:04:47.000000 metalsmith-2.1.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.464915 metalsmith-2.1.1/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.464915 metalsmith-2.1.1/doc/source/_exts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9068 2024-02-22 15:04:47.000000 metalsmith-2.1.1/doc/source/_exts/ansible-autodoc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.468915 metalsmith-2.1.1/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-02-22 15:04:47.000000 metalsmith-2.1.1/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2889 2024-02-22 15:04:47.000000 metalsmith-2.1.1/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2024-02-22 15:04:47.000000 metalsmith-2.1.1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.468915 metalsmith-2.1.1/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2024-02-22 15:04:47.000000 metalsmith-2.1.1/doc/source/user/ansible.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.468915 metalsmith-2.1.1/metalsmith/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11069 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_cmd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4122 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5504 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3506 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_network_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9141 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_nics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31736 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_provisioner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6097 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4276 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5717 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/instance_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13443 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/sources.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.472915 metalsmith-2.1.1/metalsmith/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33972 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_cmd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7069 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5820 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_instance_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10431 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_metalsmith_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5206 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_network_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15050 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_nics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   101043 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_provisioner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5386 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9678 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_sources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3361 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.468915 metalsmith-2.1.1/metalsmith.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2952 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4331 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.460915 metalsmith-2.1.1/metalsmith_ansible/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.460915 metalsmith-2.1.1/metalsmith_ansible/ansible_plugins/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.472915 metalsmith-2.1.1/metalsmith_ansible/ansible_plugins/modules/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4457 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith_ansible/ansible_plugins/modules/metalsmith_deployment_defaults.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15915 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith_ansible/ansible_plugins/modules/metalsmith_instances.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.460915 metalsmith-2.1.1/metalsmith_ansible/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.472915 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7263 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.472915 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.472915 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.472915 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.464915 metalsmith-2.1.1/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.476915 metalsmith-2.1.1/playbooks/integration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4541 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/centos-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/centos8-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/centos8-integration.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/centos9-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/centos9-integration.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3790 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/cirros-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3688 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/exercise.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/initial-setup.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1250 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/ssh-key.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.464915 metalsmith-2.1.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.480915 metalsmith-2.1.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/0.9-deprecations-f403ce4961b77fe1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/allocation-hostname-f148e8adf0aee89a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/allow-both-network-and-subnet-in-nic-info-af8b40a26d55828e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/api-stein-8e5d165aa6d115cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/associated-993c26ac5dc0cfc0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/config_drive-f59bb5d8e684b2ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/deprecations-14-4292eaa456564782.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/drop-py-2-7-3cd57c85e8eb8d2d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/exceptions-395ae4f1ad4de6da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/file-checksum-d19370a8fde00a81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/fix-ip-allocation-deferred-causing-broken-network-metadata-9c3ccfab2c563466.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/format-hostname-634a412ea933a966.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/iinfo-2014b1de4dbeca2d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/initial-5afe4a5f6a13fa8e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/instance-config-c4ea6a169f782138.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/keep-instance-info-3e7bb09244d5aaa6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/network-metadata-ff0c3e80e5e0f53c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/no-clean-up-03bfaee6bbb112fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/openstacksdk-9ad2298b84e34a5f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/prettytable-1db78a96c1d921d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/raw_http_images-41007351896ff642.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/reserve-hostname-85d02321156bde3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/resource-class-1957e83fa8235641.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/source-detect-673ad8c3e98c3df1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/states-79b593683c0783d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/stein-deprecation-6a4c9217a6ac4f13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/subnet-1c177e4b40cc607c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/update-references-for-checksums-44206e710b0506fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/whole-disk-root-gb-bd8ee3600de9ec8d.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.484915 metalsmith-2.1.1/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.484915 metalsmith-2.1.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.484915 metalsmith-2.1.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6627 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2024-02-22 15:04:47.000000 metalsmith-2.1.1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1154 2024-02-22 15:05:18.484915 metalsmith-2.1.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-02-22 15:04:47.000000 metalsmith-2.1.1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2024-02-22 15:04:47.000000 metalsmith-2.1.1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.484915 metalsmith-2.1.1/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-02-22 15:04:47.000000 metalsmith-2.1.1/tools/ansible-lint.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3567 2024-02-22 15:04:47.000000 metalsmith-2.1.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.897324 metalsmith-2.2.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2024-05-23 07:55:24.000000 metalsmith-2.2.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6428 2024-05-23 07:55:24.000000 metalsmith-2.2.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2024-05-23 07:55:54.000000 metalsmith-2.2.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12012 2024-05-23 07:55:54.000000 metalsmith-2.2.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2024-05-23 07:55:24.000000 metalsmith-2.2.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2952 2024-05-23 07:55:54.897324 metalsmith-2.2.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1559 2024-05-23 07:55:24.000000 metalsmith-2.2.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.881324 metalsmith-2.2.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2024-05-23 07:55:24.000000 metalsmith-2.2.0/doc/joined-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2024-05-23 07:55:24.000000 metalsmith-2.2.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.881324 metalsmith-2.2.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.881324 metalsmith-2.2.0/doc/source/_exts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9068 2024-05-23 07:55:24.000000 metalsmith-2.2.0/doc/source/_exts/ansible-autodoc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.881324 metalsmith-2.2.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-05-23 07:55:24.000000 metalsmith-2.2.0/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2889 2024-05-23 07:55:24.000000 metalsmith-2.2.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2024-05-23 07:55:24.000000 metalsmith-2.2.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.881324 metalsmith-2.2.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2024-05-23 07:55:24.000000 metalsmith-2.2.0/doc/source/user/ansible.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.885324 metalsmith-2.2.0/metalsmith/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11069 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/_cmd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4122 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5504 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3506 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/_network_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9141 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/_nics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31736 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/_provisioner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6097 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/_scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4276 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5717 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/instance_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13443 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/sources.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.889324 metalsmith-2.2.0/metalsmith/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/test/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33972 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/test/test_cmd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7069 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/test/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5820 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/test/test_instance_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10431 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/test/test_metalsmith_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5206 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/test/test_network_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15050 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/test/test_nics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   101043 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/test/test_provisioner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5386 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/test/test_scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9678 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/test/test_sources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3361 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/test/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.885324 metalsmith-2.2.0/metalsmith.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2952 2024-05-23 07:55:54.000000 metalsmith-2.2.0/metalsmith.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4362 2024-05-23 07:55:54.000000 metalsmith-2.2.0/metalsmith.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 07:55:54.000000 metalsmith-2.2.0/metalsmith.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-05-23 07:55:54.000000 metalsmith-2.2.0/metalsmith.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 07:55:54.000000 metalsmith-2.2.0/metalsmith.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-23 07:55:54.000000 metalsmith-2.2.0/metalsmith.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2024-05-23 07:55:54.000000 metalsmith-2.2.0/metalsmith.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2024-05-23 07:55:54.000000 metalsmith-2.2.0/metalsmith.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.877324 metalsmith-2.2.0/metalsmith_ansible/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.877324 metalsmith-2.2.0/metalsmith_ansible/ansible_plugins/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.889324 metalsmith-2.2.0/metalsmith_ansible/ansible_plugins/modules/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4457 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith_ansible/ansible_plugins/modules/metalsmith_deployment_defaults.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15915 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith_ansible/ansible_plugins/modules/metalsmith_instances.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.877324 metalsmith-2.2.0/metalsmith_ansible/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.889324 metalsmith-2.2.0/metalsmith_ansible/roles/metalsmith_deployment/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7263 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith_ansible/roles/metalsmith_deployment/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.889324 metalsmith-2.2.0/metalsmith_ansible/roles/metalsmith_deployment/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith_ansible/roles/metalsmith_deployment/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.889324 metalsmith-2.2.0/metalsmith_ansible/roles/metalsmith_deployment/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith_ansible/roles/metalsmith_deployment/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.889324 metalsmith-2.2.0/metalsmith_ansible/roles/metalsmith_deployment/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2024-05-23 07:55:24.000000 metalsmith-2.2.0/metalsmith_ansible/roles/metalsmith_deployment/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.877324 metalsmith-2.2.0/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.889324 metalsmith-2.2.0/playbooks/integration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4541 2024-05-23 07:55:24.000000 metalsmith-2.2.0/playbooks/integration/centos-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2663 2024-05-23 07:55:24.000000 metalsmith-2.2.0/playbooks/integration/centos8-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2024-05-23 07:55:24.000000 metalsmith-2.2.0/playbooks/integration/centos8-integration.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2669 2024-05-23 07:55:24.000000 metalsmith-2.2.0/playbooks/integration/centos9-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2024-05-23 07:55:24.000000 metalsmith-2.2.0/playbooks/integration/centos9-integration.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3790 2024-05-23 07:55:24.000000 metalsmith-2.2.0/playbooks/integration/cirros-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3688 2024-05-23 07:55:24.000000 metalsmith-2.2.0/playbooks/integration/exercise.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2024-05-23 07:55:24.000000 metalsmith-2.2.0/playbooks/integration/initial-setup.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2024-05-23 07:55:24.000000 metalsmith-2.2.0/playbooks/integration/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1250 2024-05-23 07:55:24.000000 metalsmith-2.2.0/playbooks/integration/run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2024-05-23 07:55:24.000000 metalsmith-2.2.0/playbooks/integration/ssh-key.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.877324 metalsmith-2.2.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.897324 metalsmith-2.2.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/0.9-deprecations-f403ce4961b77fe1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/allocation-hostname-f148e8adf0aee89a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/allow-both-network-and-subnet-in-nic-info-af8b40a26d55828e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/api-stein-8e5d165aa6d115cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/associated-993c26ac5dc0cfc0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/config_drive-f59bb5d8e684b2ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/deprecations-14-4292eaa456564782.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/drop-py-2-7-3cd57c85e8eb8d2d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/exceptions-395ae4f1ad4de6da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/file-checksum-d19370a8fde00a81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/fix-ip-allocation-deferred-causing-broken-network-metadata-9c3ccfab2c563466.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/format-hostname-634a412ea933a966.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/iinfo-2014b1de4dbeca2d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/initial-5afe4a5f6a13fa8e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/instance-config-c4ea6a169f782138.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/keep-instance-info-3e7bb09244d5aaa6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/network-metadata-ff0c3e80e5e0f53c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/no-clean-up-03bfaee6bbb112fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/openstacksdk-9ad2298b84e34a5f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/prettytable-1db78a96c1d921d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/raw_http_images-41007351896ff642.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/reserve-hostname-85d02321156bde3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/resource-class-1957e83fa8235641.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/source-detect-673ad8c3e98c3df1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/states-79b593683c0783d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/stein-deprecation-6a4c9217a6ac4f13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/subnet-1c177e4b40cc607c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/update-references-for-checksums-44206e710b0506fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/notes/whole-disk-root-gb-bd8ee3600de9ec8d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.897324 metalsmith-2.2.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.897324 metalsmith-2.2.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.897324 metalsmith-2.2.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6627 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-23 07:55:24.000000 metalsmith-2.2.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2024-05-23 07:55:24.000000 metalsmith-2.2.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1154 2024-05-23 07:55:54.901324 metalsmith-2.2.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-05-23 07:55:24.000000 metalsmith-2.2.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2024-05-23 07:55:24.000000 metalsmith-2.2.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:54.897324 metalsmith-2.2.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-05-23 07:55:24.000000 metalsmith-2.2.0/tools/ansible-lint.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3567 2024-05-23 07:55:24.000000 metalsmith-2.2.0/tox.ini
```

### Comparing `metalsmith-2.1.1/.zuul.yaml` & `metalsmith-2.2.0/.zuul.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -183,18 +183,21 @@
       - openstack-python3-antelope-jobs
       - openstack-cover-jobs
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
     check:
       jobs:
         - metalsmith-integration-glance-centos9-uefi
-        - metalsmith-integration-glance-centos9-legacy
+        # NOTE(rpittau): this is broken because of an issue with tinycore
+        # moving to non-voting while we evaluate if it's worth trying to
+        # fix it or just removing it
+        - metalsmith-integration-glance-centos9-legacy:
+            voting: false
         - metalsmith-integration-http-cirros
         - openstack-tox-linters
         - metalsmith-tox-codespell:
             voting: false
     gate:
       jobs:
         - metalsmith-integration-glance-centos9-uefi
-        - metalsmith-integration-glance-centos9-legacy
         - metalsmith-integration-http-cirros
         - openstack-tox-linters
```

### Comparing `metalsmith-2.1.1/AUTHORS` & `metalsmith-2.2.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/ChangeLog` & `metalsmith-2.2.0/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 CHANGES
 =======
 
+2.2.0
+-----
+
+* reno: Update master for unmaintained/zed
+* Use bootloader element instead of grub2
+* reno: Update master for unmaintained/xena
+* reno: Update master for unmaintained/wallaby
+* reno: Update master for unmaintained/victoria
+* Update master for stable/2024.1
+
 2.1.1
 -----
 
 * reno: Update master for unmaintained/yoga
 * [codespell] Adding CI target for Tox Codespell
 * [codespell] Adding Tox Target for Codespell
 * CI: Ask ironic devstack to set node owner
```

### Comparing `metalsmith-2.1.1/LICENSE` & `metalsmith-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/PKG-INFO` & `metalsmith-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: metalsmith
-Version: 2.1.1
+Version: 2.2.0
 Summary: Deployment and Scheduling tool for Bare Metal
 Home-page: https://opendev.org/openstack/metalsmith
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: Deployment and Scheduling tool for Bare Metal
         =============================================
```

### Comparing `metalsmith-2.1.1/README.rst` & `metalsmith-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/doc/source/_exts/ansible-autodoc.py` & `metalsmith-2.2.0/doc/source/_exts/ansible-autodoc.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/doc/source/cli/index.rst` & `metalsmith-2.2.0/doc/source/cli/index.rst`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/doc/source/conf.py` & `metalsmith-2.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/__init__.py` & `metalsmith-2.2.0/metalsmith/__init__.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/_cmd.py` & `metalsmith-2.2.0/metalsmith/_cmd.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/_format.py` & `metalsmith-2.2.0/metalsmith/_format.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/_instance.py` & `metalsmith-2.2.0/metalsmith/_instance.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/_network_metadata.py` & `metalsmith-2.2.0/metalsmith/_network_metadata.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/_nics.py` & `metalsmith-2.2.0/metalsmith/_nics.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/_provisioner.py` & `metalsmith-2.2.0/metalsmith/_provisioner.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/_scheduler.py` & `metalsmith-2.2.0/metalsmith/_scheduler.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/_utils.py` & `metalsmith-2.2.0/metalsmith/_utils.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/exceptions.py` & `metalsmith-2.2.0/metalsmith/exceptions.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/instance_config.py` & `metalsmith-2.2.0/metalsmith/instance_config.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/sources.py` & `metalsmith-2.2.0/metalsmith/sources.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/test/test_cmd.py` & `metalsmith-2.2.0/metalsmith/test/test_cmd.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/test/test_instance.py` & `metalsmith-2.2.0/metalsmith/test/test_instance.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/test/test_instance_config.py` & `metalsmith-2.2.0/metalsmith/test/test_instance_config.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/test/test_metalsmith_instances.py` & `metalsmith-2.2.0/metalsmith/test/test_metalsmith_instances.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/test/test_network_metadata.py` & `metalsmith-2.2.0/metalsmith/test/test_network_metadata.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/test/test_nics.py` & `metalsmith-2.2.0/metalsmith/test/test_nics.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/test/test_provisioner.py` & `metalsmith-2.2.0/metalsmith/test/test_provisioner.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/test/test_scheduler.py` & `metalsmith-2.2.0/metalsmith/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/test/test_sources.py` & `metalsmith-2.2.0/metalsmith/test/test_sources.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/test/test_utils.py` & `metalsmith-2.2.0/metalsmith/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith/version.py` & `metalsmith-2.2.0/metalsmith/version.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith.egg-info/PKG-INFO` & `metalsmith-2.2.0/metalsmith.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: metalsmith
-Version: 2.1.1
+Version: 2.2.0
 Summary: Deployment and Scheduling tool for Bare Metal
 Home-page: https://opendev.org/openstack/metalsmith
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: Deployment and Scheduling tool for Bare Metal
         =============================================
```

### Comparing `metalsmith-2.1.1/metalsmith.egg-info/SOURCES.txt` & `metalsmith-2.2.0/metalsmith.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 releasenotes/notes/states-79b593683c0783d5.yaml
 releasenotes/notes/stein-deprecation-6a4c9217a6ac4f13.yaml
 releasenotes/notes/subnet-1c177e4b40cc607c.yaml
 releasenotes/notes/update-references-for-checksums-44206e710b0506fe.yaml
 releasenotes/notes/whole-disk-root-gb-bd8ee3600de9ec8d.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/stein.rst
 releasenotes/source/train.rst
 releasenotes/source/unreleased.rst
 releasenotes/source/ussuri.rst
 releasenotes/source/victoria.rst
```

### Comparing `metalsmith-2.1.1/metalsmith_ansible/ansible_plugins/modules/metalsmith_deployment_defaults.py` & `metalsmith-2.2.0/metalsmith_ansible/ansible_plugins/modules/metalsmith_deployment_defaults.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith_ansible/ansible_plugins/modules/metalsmith_instances.py` & `metalsmith-2.2.0/metalsmith_ansible/ansible_plugins/modules/metalsmith_instances.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/README.rst` & `metalsmith-2.2.0/metalsmith_ansible/roles/metalsmith_deployment/README.rst`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/defaults/main.yml` & `metalsmith-2.2.0/metalsmith_ansible/roles/metalsmith_deployment/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/tasks/main.yml` & `metalsmith-2.2.0/metalsmith_ansible/roles/metalsmith_deployment/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/playbooks/integration/centos-image.yaml` & `metalsmith-2.2.0/playbooks/integration/centos-image.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/playbooks/integration/centos8-image.yaml` & `metalsmith-2.2.0/playbooks/integration/centos9-image.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 ---
 - name: "Set centos image facts"
   set_fact:
-    centos_image_file: ~/centos8-wholedisk.qcow2
-    centos_initramfs_file: ~/centos8-partition.initrd
-    centos_kernel_file: ~/centos8-partition.vmlinuz
-    centos_partition_file: ~/centos8-partition.qcow2
+    centos_image_file: ~/centos9-wholedisk.qcow2
+    centos_initramfs_file: ~/centos9-partition.initrd
+    centos_kernel_file: ~/centos9-partition.vmlinuz
+    centos_partition_file: ~/centos9-partition.qcow2
 
 - name: Install kpartx
   package:
     name: kpartx
     state: present
   become: true
 
 - name: Install DIB
   pip:
-    name: diskimage-builder
+    name: "/home/zuul/src/opendev.org/openstack/diskimage-builder"
   become: true
   vars:
     ansible_python_interpreter: /usr/bin/{{ metalsmith_python | default('python') }}
 
 - name: Make kernel files readable (workaround for Ubuntu)
   shell: chmod 0644 /boot/vmlinuz-*
   become: true
 
 - name: Detect the right block device element
   set_fact:
     centos_block_device: block-device-efi
   when: metalsmith_boot_mode | default('uefi') != 'bios'
 
-- name: Build a centos8 wholedisk image
+- name: Build a centos9 wholedisk image
   command: >
-    disk-image-create centos grub2 vm {{ centos_block_device | default('') }}
-    -o centos8-wholedisk
+    disk-image-create -x centos bootloader vm {{ centos_block_device | default('') }}
+    -o centos9-wholedisk
   environment:
-    DIB_RELEASE: 8-stream
+    DIB_RELEASE: 9-stream
 
-- name: Build a centos8 partition image
-  command: disk-image-create centos grub2 baremetal -o centos8-partition
+- name: Build a centos9 partition image
+  command: disk-image-create -x centos bootloader baremetal -o centos9-partition
   environment:
-    DIB_RELEASE: 8-stream
+    DIB_RELEASE: 9-stream
 
 - name: Upload the CentOS whole-disk image
   command: >
       openstack image create --disk-format qcow2
       --public --file {{ centos_image_file }}
       {{ centos_glance_whole_disk_image }}
   environment:
```

### Comparing `metalsmith-2.1.1/playbooks/integration/centos8-integration.yaml` & `metalsmith-2.2.0/playbooks/integration/centos8-integration.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/playbooks/integration/centos9-image.yaml` & `metalsmith-2.2.0/playbooks/integration/centos8-image.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 ---
 - name: "Set centos image facts"
   set_fact:
-    centos_image_file: ~/centos9-wholedisk.qcow2
-    centos_initramfs_file: ~/centos9-partition.initrd
-    centos_kernel_file: ~/centos9-partition.vmlinuz
-    centos_partition_file: ~/centos9-partition.qcow2
+    centos_image_file: ~/centos8-wholedisk.qcow2
+    centos_initramfs_file: ~/centos8-partition.initrd
+    centos_kernel_file: ~/centos8-partition.vmlinuz
+    centos_partition_file: ~/centos8-partition.qcow2
 
 - name: Install kpartx
   package:
     name: kpartx
     state: present
   become: true
 
 - name: Install DIB
   pip:
-    name: diskimage-builder
+    name: "/home/zuul/src/opendev.org/openstack/diskimage-builder"
   become: true
   vars:
     ansible_python_interpreter: /usr/bin/{{ metalsmith_python | default('python') }}
 
 - name: Make kernel files readable (workaround for Ubuntu)
   shell: chmod 0644 /boot/vmlinuz-*
   become: true
 
 - name: Detect the right block device element
   set_fact:
     centos_block_device: block-device-efi
   when: metalsmith_boot_mode | default('uefi') != 'bios'
 
-- name: Build a centos9 wholedisk image
+- name: Build a centos8 wholedisk image
   command: >
-    disk-image-create centos grub2 vm {{ centos_block_device | default('') }}
-    -o centos9-wholedisk
+    disk-image-create centos bootloader vm {{ centos_block_device | default('') }}
+    -o centos8-wholedisk
   environment:
-    DIB_RELEASE: 9-stream
+    DIB_RELEASE: 8-stream
 
-- name: Build a centos9 partition image
-  command: disk-image-create centos grub2 baremetal -o centos9-partition
+- name: Build a centos8 partition image
+  command: disk-image-create centos bootloader baremetal -o centos8-partition
   environment:
-    DIB_RELEASE: 9-stream
+    DIB_RELEASE: 8-stream
 
 - name: Upload the CentOS whole-disk image
   command: >
       openstack image create --disk-format qcow2
       --public --file {{ centos_image_file }}
       {{ centos_glance_whole_disk_image }}
   environment:
```

### Comparing `metalsmith-2.1.1/playbooks/integration/centos9-integration.yaml` & `metalsmith-2.2.0/playbooks/integration/centos9-integration.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/playbooks/integration/cirros-image.yaml` & `metalsmith-2.2.0/playbooks/integration/cirros-image.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/playbooks/integration/exercise.yaml` & `metalsmith-2.2.0/playbooks/integration/exercise.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/playbooks/integration/initial-setup.yaml` & `metalsmith-2.2.0/playbooks/integration/initial-setup.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/playbooks/integration/run.yaml` & `metalsmith-2.2.0/playbooks/integration/run.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/releasenotes/notes/network-metadata-ff0c3e80e5e0f53c.yaml` & `metalsmith-2.2.0/releasenotes/notes/network-metadata-ff0c3e80e5e0f53c.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/releasenotes/notes/openstacksdk-9ad2298b84e34a5f.yaml` & `metalsmith-2.2.0/releasenotes/notes/openstacksdk-9ad2298b84e34a5f.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/releasenotes/notes/states-79b593683c0783d5.yaml` & `metalsmith-2.2.0/releasenotes/notes/states-79b593683c0783d5.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/releasenotes/source/conf.py` & `metalsmith-2.2.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/setup.cfg` & `metalsmith-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/setup.py` & `metalsmith-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.1/tox.ini` & `metalsmith-2.2.0/tox.ini`

 * *Files identical despite different names*

