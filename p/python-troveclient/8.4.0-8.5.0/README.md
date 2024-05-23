# Comparing `tmp/python-troveclient-8.4.0.tar.gz` & `tmp/python-troveclient-8.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-troveclient-8.4.0.tar", last modified: Thu Feb 29 09:47:37 2024, max compression
+gzip compressed data, was "python-troveclient-8.5.0.tar", last modified: Thu May 23 08:03:02 2024, max compression
```

## Comparing `python-troveclient-8.4.0.tar` & `python-troveclient-8.5.0.tar`

### file list

```diff
@@ -1,304 +1,305 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.153272 python-troveclient-8.4.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6174 2024-02-29 09:47:36.000000 python-troveclient-8.4.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30111 2024-02-29 09:47:36.000000 python-troveclient-8.4.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2987 2024-02-29 09:47:37.153272 python-troveclient-8.4.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1783 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.105273 python-troveclient-8.4.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.105273 python-troveclient-8.4.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1869 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.105273 python-troveclient-8.4.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.105273 python-troveclient-8.4.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3864 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/doc/source/user/api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.105273 python-troveclient-8.4.0/python_troveclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2987 2024-02-29 09:47:37.000000 python-troveclient-8.4.0/python_troveclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12834 2024-02-29 09:47:37.000000 python-troveclient-8.4.0/python_troveclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-29 09:47:37.000000 python-troveclient-8.4.0/python_troveclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7122 2024-02-29 09:47:37.000000 python-troveclient-8.4.0/python_troveclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-29 09:47:37.000000 python-troveclient-8.4.0/python_troveclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-29 09:47:37.000000 python-troveclient-8.4.0/python_troveclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-02-29 09:47:37.000000 python-troveclient-8.4.0/python_troveclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2024-02-29 09:47:37.000000 python-troveclient-8.4.0/python_troveclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.101273 python-troveclient-8.4.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.125273 python-troveclient-8.4.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-backup-create-to-osc-c3d257365cf65cae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-backup-delete-to-osc-e302b87809cb814c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-backup-list-instance-to-osc-e01cf8527e499768.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-backup-list-to-osc-ea5cbfb579f3ffc7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-backup-show-to-osc-022f42ad93136ce6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-cluster-create-to-osc-47e3bb3a83dcab76.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-cluster-delete-to-osc-9601c8bc0e637c4b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-cluster-grow-shrink-to-osc-a07bc0d974b0c0a4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-cluster-instances-to-osc-429eeb91d86da663.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-cluster-list-to-osc-93532b79db906a14.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-cluster-modules-to-osc-647a0564dafcef24.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-cluster-show-to-osc-5925431f5e94a746.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-configuration-attach-detach-to-osc-c5b52784910f2b09.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-configuration-create-to-osc-fd556891b57cce05.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-configuration-default-to-osc-55867236d19d83c4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-configuration-delete-to-osc-d52e6a2cc84994e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-configuration-groups-for-clusters-6183b0b7b4fb8c9e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-configuration-instances-to-osc-80a7d7b9d0c79f62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-configuration-list-to-osc-4a12d508f6bb5472.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-configuration-parameter-list-to-osc-3d1a383999dd2d64.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-configuration-parameter-show-to-osc-5bcf21662683ceee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-configuration-show-to-osc-c139bb20a2ec18ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-database-create-to-osc-b9e85dd2cbd9b21e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-database-delete-to-osc-e6703e2d438824d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-database-list-to-osc-b547e8954e8b6fc7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-datastore-list-to-osc-007ff4144f630c57.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-datastore-show-to-osc-79a855d2e026ae80.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-datastore-version-list-to-osc-3fe8729d493f3de2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-datastore-version-show-to-osc-8c2035dbf6104a9f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-detach-replica-to-osc-1fadef6220e96f35.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-eject-replica-source-to-osc-c985a70eaab3f16b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-execution-delete-to-osc-013b4bf00a1cb8ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-flavor-list-to-osc-b8b3a42f3bae3851.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-flavor-show-to-osc-16ab5640f144cab7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-force-delete-to-osc-dfff1db4da937415.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-instance-create-to-osc-77484f1c477aa864.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-instance-delete-to-osc-bf8de501c8945d58.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-instance-detailed-list-23dc77ed898cc6db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-instance-list-to-osc-05714dfce947a57e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-instance-show-to-osc-d97cac1c697dcbdd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-log-enable-to-osc-a97bbb3a7af7b80b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-log-list-to-osc-4bc11aa6e20de286.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-promote-to-replica-source-to-osc-6eca8c5507344205.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-quota-to-osc-c50c8ec190af8f58.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-reset-status-to-osc-bd84dcdc369e2270.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-resize-flavor-to-osc-ba0e7c038df8ecfe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-resize-volume-to-osc-aa5eaabb8f25edec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-restart-instance-to-osc-760c292b5b5c95de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-root-disable-to-osc-52d81d96ec7e4e54.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-root-enable-to-osc-e3a087cc6f10a6f9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-root-show-to-osc-17e49422c5dc71de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-update-to-osc-05eb21c5fa18a788.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-upgrade-to-osc-837461ff1d588be2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-user-access-related-to-osc-ae7da3a8f5fbdd6a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-user-create-to-osc-03158640dcaa8a0e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-user-delete-to-osc-35cb82b041ee2b48.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-user-show-to-osc-6ef3db10a82f1f46.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add-user-update-attributes-to-osc-5adfffe826a62f3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add_mod_inst_count-ce532a2187b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/add_module_reapply-7645e34256d4c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/allow-backup-name-in-create-1a9e85978a3ab8bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/bulk-delete-database-instances-7938121487fb11e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/cli-configuration-name-allowed-747c5d6f2d1f8c7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/cluster-upgrade-d58d1fc4b8da0a03.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/datastore-specific-api-extensions-973b455a9922d072.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/datastore-version-volume-types-62556ce5917195fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/drop-py-2-7-4ca3cf6a8ab8ca34.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/drop-python-3-6-and-3-7-8e07d44dd0e12619.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/fix-config-param-list-output-27bf30fce5388d4b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/fix-output-of-cluster-create-584d85ffe1129d57.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/fix-wrong-datastore-flavors-args-in-osc-e0322cb5424f8c1b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/fix_admin_keystoneauth1-ed534462434.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/flavor-list-disk-befd656f86592af1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/flavor-list-ephemeral-de4eee3a30b09b64.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/flavor-list-vcpu-d3fd769a137e307c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/force_delete-2d6bb5f99fe821c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/get-all-database-instance-admin-3f1b83a487dd11e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/image-upgrade-dfa20861d756532d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/incremental_backup-c18804d6277adf62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/locality-support-for-clusters-7e89f9ddbe5f4131.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/locality-support-for-replication-5834f1a2dcaf6883.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/module-ordering-2d1e1a3c37c30c71.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/module-support-for-clusters-87b41dd7648275bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/module_update_all_ds-f5cdbb71462e3de4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/mongo-cluster-create-use-extended-perperties-be7c075585dc709a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/multi-region-ec516da866def1ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/paginate-config-list-c311ce3c5394d437.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/persist-error-message-cda8dfe485fe92ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/quota-upgrade-aed30d50c1f58502.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/remove-rax-references-in-client-33551aa2bb25181b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/run-an-action-on-many-resources-41bbe191318b97dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/scheduled-backups-49729ce37e586463.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/train-01-backup-filtering-43dc1912c72f11e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/train-02-public-instance-642d6490d47811e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/use-i18n-for-shell.py-924c1624e30a6617.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/use-i18n-for-v1-shell.py-08209f5721f20a1f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/ussuri-01-instance-log-actions-794fced41f9c11ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/ussuri-02-instance-log-tail-save-0b267a761faa11ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/ussuri-03-force-delete-instance-1643114c2e1b11ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/ussuri-04-osc-reboot-instance-760190e02eac11ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/ussuri-05-osc-delete-datastore-version-6e03d20430e611ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/ussuri-06-osc-delete-datastore-57bab744345911ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/victoria-01-update-config-group.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/victoria-02-remove-flavor-api.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/victoria-03-replication-cli.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/victoria-add-role-for-instances.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/victoria-backup-strategy.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/victoria-create-datastore-version.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/victoria-flavor-optional.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/victoria-get-and-update-instance-access.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/victoria-rebuild-instance.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/wallaby-bulk-backup-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/wallaby-datastore-version-number.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/wallaby-instance-operating-status.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/wallaby-project-backups.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/wallaby-restore-backup-from-remote.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/wallaby-update-datastore-version.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/notes/xena-support-project-name-quota-cli.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.129273 python-troveclient-8.4.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.129273 python-troveclient-8.4.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.129273 python-troveclient-8.4.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8543 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/requirements.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1432 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/run_local.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8015 2024-02-29 09:47:37.153272 python-troveclient-8.4.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.129273 python-troveclient-8.4.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5920 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/tools/install_venv_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.133273 python-troveclient-8.4.0/troveclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/_i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.133273 python-troveclient-8.4.0/troveclient/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6975 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/apiclient/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16094 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/apiclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12662 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/apiclient/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12796 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/apiclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3344 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/auth_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9249 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19150 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1618 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/common.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.137272 python-troveclient-8.4.0/troveclient/compat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1548 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/compat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13840 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/compat/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9759 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/compat/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16231 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/compat/cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14117 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/compat/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14048 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/compat/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4850 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/compat/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7714 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/compat/mcli.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.137272 python-troveclient-8.4.0/troveclient/compat/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/compat/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14469 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/compat/tests/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13536 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/compat/tests/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1465 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/compat/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/compat/versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.137272 python-troveclient-8.4.0/troveclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.141272 python-troveclient-8.4.0/troveclient/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/v1/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3759 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/v1/database_backup_strategy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12431 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/v1/database_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14705 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/v1/database_clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16737 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/v1/database_configurations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3425 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/v1/database_flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30403 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/v1/database_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1280 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/v1/database_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7863 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/v1/database_logs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2625 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/v1/database_quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4945 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/v1/database_root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11254 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/v1/database_users.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4077 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/v1/databases.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11581 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/osc/v1/datastores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/service_catalog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31222 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.145272 python-troveclient-8.4.0/troveclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31339 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.145272 python-troveclient-8.4.0/troveclient/tests/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2949 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.149272 python-troveclient-8.4.0/troveclient/tests/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7056 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/v1/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3220 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_backup_strategy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12736 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12520 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14875 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_configurations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3023 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26675 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1684 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3579 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_logs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2205 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5187 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9040 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_users.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4191 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/v1/test_databases.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7153 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/osc/v1/test_datastores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3641 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_accounts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1920 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_apiclient_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11134 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17426 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23143 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5571 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3245 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9663 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_configurations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3551 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_databases.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8840 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_datastores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2995 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_discover.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12278 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3348 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11501 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6341 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6036 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_modules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4410 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_secgroups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12961 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5098 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_users.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4020 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3487 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/tests/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11305 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:37.153272 python-troveclient-8.4.0/troveclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2113 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/accounts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2200 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/backup_strategy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10852 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5232 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4807 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/configurations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2511 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/databases.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5337 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/datastores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1743 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/diagnostics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1996 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2242 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/hosts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20206 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1562 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11337 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2951 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7321 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/modules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3681 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2946 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    98469 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5010 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/users.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2024-02-29 09:47:04.000000 python-troveclient-8.4.0/troveclient/v1/volume_types.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.467623 python-troveclient-8.5.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6254 2024-05-23 08:03:02.000000 python-troveclient-8.5.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30287 2024-05-23 08:03:02.000000 python-troveclient-8.5.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2987 2024-05-23 08:03:02.467623 python-troveclient-8.5.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1783 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.399620 python-troveclient-8.5.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.399620 python-troveclient-8.5.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1869 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.399620 python-troveclient-8.5.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.403621 python-troveclient-8.5.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3864 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/doc/source/user/api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.403621 python-troveclient-8.5.0/python_troveclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2987 2024-05-23 08:03:02.000000 python-troveclient-8.5.0/python_troveclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12865 2024-05-23 08:03:02.000000 python-troveclient-8.5.0/python_troveclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:03:02.000000 python-troveclient-8.5.0/python_troveclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7122 2024-05-23 08:03:02.000000 python-troveclient-8.5.0/python_troveclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:03:02.000000 python-troveclient-8.5.0/python_troveclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-23 08:03:02.000000 python-troveclient-8.5.0/python_troveclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2024-05-23 08:03:02.000000 python-troveclient-8.5.0/python_troveclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2024-05-23 08:03:02.000000 python-troveclient-8.5.0/python_troveclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.395620 python-troveclient-8.5.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.431622 python-troveclient-8.5.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-backup-create-to-osc-c3d257365cf65cae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-backup-delete-to-osc-e302b87809cb814c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-backup-list-instance-to-osc-e01cf8527e499768.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-backup-list-to-osc-ea5cbfb579f3ffc7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-backup-show-to-osc-022f42ad93136ce6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-cluster-create-to-osc-47e3bb3a83dcab76.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-cluster-delete-to-osc-9601c8bc0e637c4b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-cluster-grow-shrink-to-osc-a07bc0d974b0c0a4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-cluster-instances-to-osc-429eeb91d86da663.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-cluster-list-to-osc-93532b79db906a14.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-cluster-modules-to-osc-647a0564dafcef24.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-cluster-show-to-osc-5925431f5e94a746.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-configuration-attach-detach-to-osc-c5b52784910f2b09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-configuration-create-to-osc-fd556891b57cce05.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-configuration-default-to-osc-55867236d19d83c4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-configuration-delete-to-osc-d52e6a2cc84994e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-configuration-groups-for-clusters-6183b0b7b4fb8c9e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-configuration-instances-to-osc-80a7d7b9d0c79f62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-configuration-list-to-osc-4a12d508f6bb5472.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-configuration-parameter-list-to-osc-3d1a383999dd2d64.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-configuration-parameter-show-to-osc-5bcf21662683ceee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-configuration-show-to-osc-c139bb20a2ec18ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-database-create-to-osc-b9e85dd2cbd9b21e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-database-delete-to-osc-e6703e2d438824d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-database-list-to-osc-b547e8954e8b6fc7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-datastore-list-to-osc-007ff4144f630c57.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-datastore-show-to-osc-79a855d2e026ae80.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-datastore-version-list-to-osc-3fe8729d493f3de2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-datastore-version-show-to-osc-8c2035dbf6104a9f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-detach-replica-to-osc-1fadef6220e96f35.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-eject-replica-source-to-osc-c985a70eaab3f16b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-execution-delete-to-osc-013b4bf00a1cb8ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-flavor-list-to-osc-b8b3a42f3bae3851.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-flavor-show-to-osc-16ab5640f144cab7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-force-delete-to-osc-dfff1db4da937415.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-instance-create-to-osc-77484f1c477aa864.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-instance-delete-to-osc-bf8de501c8945d58.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-instance-detailed-list-23dc77ed898cc6db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-instance-list-to-osc-05714dfce947a57e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-instance-show-to-osc-d97cac1c697dcbdd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-log-enable-to-osc-a97bbb3a7af7b80b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-log-list-to-osc-4bc11aa6e20de286.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-promote-to-replica-source-to-osc-6eca8c5507344205.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-quota-to-osc-c50c8ec190af8f58.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-reset-status-to-osc-bd84dcdc369e2270.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-resize-flavor-to-osc-ba0e7c038df8ecfe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-resize-volume-to-osc-aa5eaabb8f25edec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-restart-instance-to-osc-760c292b5b5c95de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-root-disable-to-osc-52d81d96ec7e4e54.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-root-enable-to-osc-e3a087cc6f10a6f9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-root-show-to-osc-17e49422c5dc71de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-update-to-osc-05eb21c5fa18a788.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-upgrade-to-osc-837461ff1d588be2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-user-access-related-to-osc-ae7da3a8f5fbdd6a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-user-create-to-osc-03158640dcaa8a0e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-user-delete-to-osc-35cb82b041ee2b48.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-user-show-to-osc-6ef3db10a82f1f46.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add-user-update-attributes-to-osc-5adfffe826a62f3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add_mod_inst_count-ce532a2187b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/add_module_reapply-7645e34256d4c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/allow-backup-name-in-create-1a9e85978a3ab8bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/bulk-delete-database-instances-7938121487fb11e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/cli-configuration-name-allowed-747c5d6f2d1f8c7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/cluster-upgrade-d58d1fc4b8da0a03.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/datastore-specific-api-extensions-973b455a9922d072.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/datastore-version-volume-types-62556ce5917195fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/drop-py-2-7-4ca3cf6a8ab8ca34.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/drop-python-3-6-and-3-7-8e07d44dd0e12619.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/fix-config-param-list-output-27bf30fce5388d4b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/fix-output-of-cluster-create-584d85ffe1129d57.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/fix-wrong-datastore-flavors-args-in-osc-e0322cb5424f8c1b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/fix_admin_keystoneauth1-ed534462434.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/flavor-list-disk-befd656f86592af1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/flavor-list-ephemeral-de4eee3a30b09b64.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/flavor-list-vcpu-d3fd769a137e307c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/force_delete-2d6bb5f99fe821c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/get-all-database-instance-admin-3f1b83a487dd11e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/image-upgrade-dfa20861d756532d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/incremental_backup-c18804d6277adf62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/locality-support-for-clusters-7e89f9ddbe5f4131.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/locality-support-for-replication-5834f1a2dcaf6883.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/module-ordering-2d1e1a3c37c30c71.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/module-support-for-clusters-87b41dd7648275bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/module_update_all_ds-f5cdbb71462e3de4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/mongo-cluster-create-use-extended-perperties-be7c075585dc709a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/multi-region-ec516da866def1ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/paginate-config-list-c311ce3c5394d437.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/persist-error-message-cda8dfe485fe92ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/quota-upgrade-aed30d50c1f58502.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/remove-rax-references-in-client-33551aa2bb25181b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/run-an-action-on-many-resources-41bbe191318b97dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/scheduled-backups-49729ce37e586463.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/train-01-backup-filtering-43dc1912c72f11e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/train-02-public-instance-642d6490d47811e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/use-i18n-for-shell.py-924c1624e30a6617.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/use-i18n-for-v1-shell.py-08209f5721f20a1f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/ussuri-01-instance-log-actions-794fced41f9c11ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/ussuri-02-instance-log-tail-save-0b267a761faa11ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/ussuri-03-force-delete-instance-1643114c2e1b11ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/ussuri-04-osc-reboot-instance-760190e02eac11ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/ussuri-05-osc-delete-datastore-version-6e03d20430e611ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/ussuri-06-osc-delete-datastore-57bab744345911ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/victoria-01-update-config-group.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/victoria-02-remove-flavor-api.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/victoria-03-replication-cli.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/victoria-add-role-for-instances.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/victoria-backup-strategy.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/victoria-create-datastore-version.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/victoria-flavor-optional.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/victoria-get-and-update-instance-access.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/victoria-rebuild-instance.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/wallaby-bulk-backup-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/wallaby-datastore-version-number.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/wallaby-instance-operating-status.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/wallaby-project-backups.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/wallaby-restore-backup-from-remote.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/wallaby-update-datastore-version.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/notes/xena-support-project-name-quota-cli.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.439622 python-troveclient-8.5.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.439622 python-troveclient-8.5.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.439622 python-troveclient-8.5.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8543 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/requirements.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1432 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/run_local.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8015 2024-05-23 08:03:02.467623 python-troveclient-8.5.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.439622 python-troveclient-8.5.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5920 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/tools/install_venv_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.439622 python-troveclient-8.5.0/troveclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.443622 python-troveclient-8.5.0/troveclient/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6975 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/apiclient/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16094 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/apiclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12602 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/apiclient/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12796 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/apiclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3344 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/auth_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9249 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18972 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1618 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/common.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.443622 python-troveclient-8.5.0/troveclient/compat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1548 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/compat/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13840 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/compat/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9759 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/compat/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16231 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/compat/cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14056 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/compat/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14048 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/compat/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4850 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/compat/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7714 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/compat/mcli.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.447622 python-troveclient-8.5.0/troveclient/compat/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/compat/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14469 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/compat/tests/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13536 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/compat/tests/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1465 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/compat/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/compat/versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.447622 python-troveclient-8.5.0/troveclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.451623 python-troveclient-8.5.0/troveclient/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/v1/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3759 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/v1/database_backup_strategy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12431 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/v1/database_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14705 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/v1/database_clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16737 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/v1/database_configurations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3425 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/v1/database_flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30403 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/v1/database_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1280 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/v1/database_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7863 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/v1/database_logs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2625 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/v1/database_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4945 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/v1/database_root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11254 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/v1/database_users.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4077 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/v1/databases.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13067 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/osc/v1/datastores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/service_catalog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31222 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.455623 python-troveclient-8.5.0/troveclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31339 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.455623 python-troveclient-8.5.0/troveclient/tests/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2949 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.459623 python-troveclient-8.5.0/troveclient/tests/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7056 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/v1/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3220 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_backup_strategy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12736 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12520 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14875 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_configurations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3023 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26675 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1684 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3579 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_logs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2205 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5187 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9040 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_users.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4191 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/v1/test_databases.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7485 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/osc/v1/test_datastores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3641 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_accounts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1920 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_apiclient_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11134 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17426 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23143 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5571 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3245 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9663 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_configurations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3551 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_databases.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8840 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_datastores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2995 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_discover.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12278 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3348 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11690 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6341 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6036 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_modules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4410 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_secgroups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12901 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5098 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_users.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4020 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3487 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/tests/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11291 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:03:02.467623 python-troveclient-8.5.0/troveclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2113 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/accounts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2200 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/backup_strategy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10852 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5232 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4807 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/configurations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2511 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/databases.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5337 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/datastores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1743 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/diagnostics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1996 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2242 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/hosts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20206 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1562 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11736 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2951 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7321 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/modules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3681 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2946 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    98409 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5010 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/users.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2024-05-23 08:02:34.000000 python-troveclient-8.5.0/troveclient/v1/volume_types.py
```

### Comparing `python-troveclient-8.4.0/.coveragerc` & `python-troveclient-8.5.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/.zuul.yaml` & `python-troveclient-8.5.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/AUTHORS` & `python-troveclient-8.5.0/AUTHORS`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 Andreas Jaeger <aj@suse.com>
 Andreas Jaeger <aj@suse.de>
 Andrey Shestakov <ashestakov@mirantis.com>
 Anh Tran <anhtt@vn.fujitsu.com>
 Arata Notsu <notsu@virtualtech.jp>
 Ashleigh Farnham <ashleighfarnham@gmail.com>
 Bartosz Zurkowski <b.zurkowski@samsung.com>
+Bo Tran <ministry.96.nd@gmail.com>
 Bob Thyne <bob.thyne@hp.com>
 Cao Xuan Hoang <hoangcx@vn.fujitsu.com>
 Chandan Kumar <chkumar@redhat.com>
 Chaozhe.Chen <chaozhe.chen@easystack.cn>
 Chen <dstbtgagt@foxmail.com>
 Christian Berendt <berendt@b1-systems.de>
 Chuck Short <chucks@redhat.com>
@@ -105,14 +106,15 @@
 Sudarshan Acharya <sudarshan.acharya@rackspace.com>
 Sushil Kumar <skm.net@gmail.com>
 Sushil Kumar <sushil.kumar2@globallogic.com>
 Sushil Kumar <sushil.kumar3@hp.com>
 SushilKM <skm.net@gmail.com>
 Swapnil Kulkarni (coolsvap) <me@coolsvap.net>
 Swapnil Kulkarni <swapnilkulkarni2608@gmail.com>
+Takashi Kajinami <kajinamit@oss.nttdata.com>
 Takashi Kajinami <tkajinam@redhat.com>
 Theron Voran <theron.voran@rackspace.com>
 Tim Simpson <tim.simpson@rackspace.com>
 Tin Lam <tl3438@att.com>
 Tony Xu <hhktony@gmail.com>
 Tovin Seven <vinhnt@vn.fujitsu.com>
 Trevor McCasland <TM2086@att.com>
```

### Comparing `python-troveclient-8.4.0/CONTRIBUTING.rst` & `python-troveclient-8.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/ChangeLog` & `python-troveclient-8.5.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 CHANGES
 =======
 
+8.5.0
+-----
+
+* Update master for stable/2024.1
+
 8.4.0
 -----
 
 * reno: Update master for unmaintained/yoga
 
 8.3.0
 -----
 
 * Update python classifier in setup.cfg
+* Add Datastore Version Registry Extension
+* Drop unused simplejson
+* Drop implementation to keep compatibility with Python 2.5
 * Update master for stable/2023.2
 
 8.2.1
 -----
 
 * Drop openstack-lower-constraints-jobs
```

### Comparing `python-troveclient-8.4.0/LICENSE` & `python-troveclient-8.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/PKG-INFO` & `python-troveclient-8.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-troveclient
-Version: 8.4.0
+Version: 8.5.0
 Summary: Client library for OpenStack DBaaS API
 Home-page: https://docs.openstack.org/python-troveclient/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Python bindings to the OpenStack Trove API
         ==========================================
```

### Comparing `python-troveclient-8.4.0/README.rst` & `python-troveclient-8.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/doc/source/conf.py` & `python-troveclient-8.5.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/doc/source/index.rst` & `python-troveclient-8.5.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/doc/source/user/api.rst` & `python-troveclient-8.5.0/doc/source/user/api.rst`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/doc/source/user/index.rst` & `python-troveclient-8.5.0/doc/source/user/index.rst`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/python_troveclient.egg-info/PKG-INFO` & `python-troveclient-8.5.0/python_troveclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-troveclient
-Version: 8.4.0
+Version: 8.5.0
 Summary: Client library for OpenStack DBaaS API
 Home-page: https://docs.openstack.org/python-troveclient/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Python bindings to the OpenStack Trove API
         ==========================================
```

### Comparing `python-troveclient-8.4.0/python_troveclient.egg-info/SOURCES.txt` & `python-troveclient-8.5.0/python_troveclient.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -143,14 +143,15 @@
 releasenotes/notes/wallaby-instance-operating-status.yaml
 releasenotes/notes/wallaby-project-backups.yaml
 releasenotes/notes/wallaby-restore-backup-from-remote.yaml
 releasenotes/notes/wallaby-update-datastore-version.yaml
 releasenotes/notes/xena-support-project-name-quota-cli.yaml
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

### Comparing `python-troveclient-8.4.0/python_troveclient.egg-info/entry_points.txt` & `python-troveclient-8.5.0/python_troveclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/releasenotes/source/conf.py` & `python-troveclient-8.5.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/requirements.txt` & `python-troveclient-8.5.0/test-requirements.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # The order of packages is significant, because pip processes them in the order
 # of appearance. Changing the order has an impact on the overall integration
 # process, which may cause wedges in the gate later.
-pbr!=2.1.0,>=2.0.0 # Apache-2.0
-PrettyTable>=0.7.2 # BSD
-requests>=2.14.2 # Apache-2.0
-simplejson>=3.5.1 # MIT
-oslo.i18n>=3.15.3 # Apache-2.0
-oslo.utils>=3.33.0 # Apache-2.0
-keystoneauth1>=3.4.0 # Apache-2.0
-python-swiftclient>=3.2.0 # Apache-2.0
-python-mistralclient!=3.2.0,>=3.1.0 # Apache-2.0
-osc-lib>=1.8.0 # Apache-2.0
+hacking>=3.0.1,<3.1.0 # Apache-2.0
+coverage!=4.4,>=4.0 # Apache-2.0
+fixtures>=3.0.0 # Apache-2.0/BSD
+oslotest>=3.2.0 # Apache-2.0
 python-openstackclient>=3.12.0 # Apache-2.0
+requests-mock>=1.2.0 # Apache-2.0
+stestr>=2.0.0 # Apache-2.0
+testscenarios>=0.4 # Apache-2.0/BSD
+testtools>=2.2.0 # MIT
+httplib2>=0.9.1 # MIT
```

### Comparing `python-troveclient-8.4.0/run_local.sh` & `python-troveclient-8.5.0/run_local.sh`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/setup.cfg` & `python-troveclient-8.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/setup.py` & `python-troveclient-8.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/tools/install_venv_common.py` & `python-troveclient-8.5.0/tools/install_venv_common.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/tox.ini` & `python-troveclient-8.5.0/tox.ini`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/__init__.py` & `python-troveclient-8.5.0/troveclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/_i18n.py` & `python-troveclient-8.5.0/troveclient/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/apiclient/auth.py` & `python-troveclient-8.5.0/troveclient/apiclient/auth.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/apiclient/base.py` & `python-troveclient-8.5.0/troveclient/apiclient/base.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/apiclient/client.py` & `python-troveclient-8.5.0/troveclient/apiclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,22 +21,18 @@
 """
 OpenStack Client interface. Handles the REST calls and responses.
 """
 
 # E0202: An attribute inherited from %s hide this method
 # pylint: disable=E0202
 
+import json
 import logging
 import time
 
-try:
-    import simplejson as json
-except ImportError:
-    import json
-
 import requests
 
 from oslo_utils import importutils
 from troveclient.apiclient import exceptions
 
 
 LOG = logging.getLogger(__name__)
```

### Comparing `python-troveclient-8.4.0/troveclient/apiclient/exceptions.py` & `python-troveclient-8.5.0/troveclient/apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/auth_plugin.py` & `python-troveclient-8.5.0/troveclient/auth_plugin.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/base.py` & `python-troveclient-8.5.0/troveclient/base.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/client.py` & `python-troveclient-8.5.0/troveclient/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 """
 OpenStack Client interface. Handles the REST calls and responses.
 """
 
+import json
 import logging
 
 from keystoneauth1 import adapter
 from oslo_utils import importutils
 import requests
 from urllib import parse as urlparse
 
@@ -31,24 +32,14 @@
 from troveclient import service_catalog
 
 try:
     import eventlet as sleep_lib
 except ImportError:
     import time as sleep_lib
 
-try:
-    import json
-except ImportError:
-    import simplejson as json
-
-# Python 2.5 compat fix
-if not hasattr(urlparse, 'parse_qsl'):
-    import cgi
-    urlparse.parse_qsl = cgi.parse_qsl
-
 osprofiler_web = importutils.try_import("osprofiler.web")
 
 
 class TroveClientMixin(object):
 
     def get_database_api_version_from_endpoint(self):
         magic_tuple = urlparse.urlsplit(self.management_url)
```

### Comparing `python-troveclient-8.4.0/troveclient/common.py` & `python-troveclient-8.5.0/troveclient/common.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/compat/__init__.py` & `python-troveclient-8.5.0/troveclient/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/compat/auth.py` & `python-troveclient-8.5.0/troveclient/compat/auth.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/compat/base.py` & `python-troveclient-8.5.0/troveclient/compat/base.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/compat/cli.py` & `python-troveclient-8.5.0/troveclient/compat/cli.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/compat/client.py` & `python-troveclient-8.5.0/troveclient/compat/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,25 +10,20 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import httplib2
+import json
 import logging
 import os
 import sys
 import time
 
-try:
-    import json
-except ImportError:
-    import simplejson as json
-
-
 from troveclient.compat import auth
 from troveclient.compat import exceptions
 
 
 LOG = logging.getLogger(__name__)
 RDC_PP = os.environ.get("RDC_PP", "False") == "True"
```

### Comparing `python-troveclient-8.4.0/troveclient/compat/common.py` & `python-troveclient-8.5.0/troveclient/compat/common.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/compat/exceptions.py` & `python-troveclient-8.5.0/troveclient/compat/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/compat/mcli.py` & `python-troveclient-8.5.0/troveclient/compat/mcli.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/compat/tests/test_auth.py` & `python-troveclient-8.5.0/troveclient/compat/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/compat/tests/test_common.py` & `python-troveclient-8.5.0/troveclient/compat/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/compat/utils.py` & `python-troveclient-8.5.0/troveclient/compat/utils.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/compat/versions.py` & `python-troveclient-8.5.0/troveclient/compat/versions.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/exceptions.py` & `python-troveclient-8.5.0/troveclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/extension.py` & `python-troveclient-8.5.0/troveclient/extension.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/i18n.py` & `python-troveclient-8.5.0/troveclient/i18n.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/osc/plugin.py` & `python-troveclient-8.5.0/troveclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/osc/v1/base.py` & `python-troveclient-8.5.0/troveclient/osc/v1/base.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/osc/v1/database_backup_strategy.py` & `python-troveclient-8.5.0/troveclient/osc/v1/database_backup_strategy.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/osc/v1/database_backups.py` & `python-troveclient-8.5.0/troveclient/osc/v1/database_backups.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/osc/v1/database_clusters.py` & `python-troveclient-8.5.0/troveclient/osc/v1/database_clusters.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/osc/v1/database_configurations.py` & `python-troveclient-8.5.0/troveclient/osc/v1/database_configurations.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/osc/v1/database_flavors.py` & `python-troveclient-8.5.0/troveclient/osc/v1/database_flavors.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/osc/v1/database_instances.py` & `python-troveclient-8.5.0/troveclient/osc/v1/database_instances.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/osc/v1/database_limits.py` & `python-troveclient-8.5.0/troveclient/osc/v1/database_limits.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/osc/v1/database_logs.py` & `python-troveclient-8.5.0/troveclient/osc/v1/database_logs.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/osc/v1/database_quota.py` & `python-troveclient-8.5.0/troveclient/osc/v1/database_quota.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/osc/v1/database_root.py` & `python-troveclient-8.5.0/troveclient/osc/v1/database_root.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/osc/v1/database_users.py` & `python-troveclient-8.5.0/troveclient/osc/v1/database_users.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/osc/v1/databases.py` & `python-troveclient-8.5.0/troveclient/osc/v1/databases.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/osc/v1/datastores.py` & `python-troveclient-8.5.0/troveclient/osc/v1/datastores.py`

 * *Files 5% similar despite different names*

```diff
@@ -191,14 +191,28 @@
         )
         parser.add_argument(
             'image_id',
             help=_('ID of the datastore image in Glance. This can be empty '
                    'string if --image-tags is specified.'),
         )
         parser.add_argument(
+            '--registry-ext',
+            help=_('Extension for default datastore managers. '
+                   'Allows the use of custom managers for each of '
+                   'the datastores supported by Trove.'
+                   'This can be empty string.'),
+        )
+        parser.add_argument(
+            '--repl-strategy',
+            help=_('Extension for default strategy for replication. '
+                   'Allows the use of custom replication strategy '
+                   'for each of the datastores supported by Trove.'
+                   'This can be empty string.'),
+        )
+        parser.add_argument(
             '--active',
             action='store_true',
             help=_('Enable the datastore version.'),
         )
         parser.add_argument(
             '--image-tags',
             help=_('List of image tags separated by comma, e.g. trove,mysql'),
@@ -225,14 +239,16 @@
         try:
             client.create(
                 parsed_args.version_name,
                 parsed_args.datastore_name,
                 parsed_args.datastore_manager,
                 parsed_args.image_id,
                 image_tags=image_tags,
+                registry_ext=parsed_args.registry_ext,
+                repl_strategy=parsed_args.repl_strategy,
                 active='true' if parsed_args.active else 'false',
                 default='true' if parsed_args.default else 'false',
                 version=parsed_args.version_number
             )
         except Exception as e:
             msg = (_("Failed to create datastore version %(version)s: %(e)s")
                    % {'version': parsed_args.version_name, 'e': e})
@@ -260,14 +276,28 @@
         )
         parser.add_argument(
             '--image-tags',
             default=None,
             help=_('List of image tags separated by comma, e.g. trove,mysql'),
         )
         parser.add_argument(
+            '--registry-ext',
+            help=_('Extension for default datastore managers. '
+                   'Allows the use of custom managers for each of '
+                   'the datastores supported by Trove.'
+                   'This can be empty string.'),
+        )
+        parser.add_argument(
+            '--repl-strategy',
+            help=_('Extension for default strategy for replication. '
+                   'Allows the use of custom replication strategy '
+                   'for each of the datastores supported by Trove.'
+                   'This can be empty string.'),
+        )
+        parser.add_argument(
             '--version-name',
             help=_('New datastore version name.'),
         )
 
         enable_group = parser.add_mutually_exclusive_group()
         enable_group.add_argument('--enable', dest='enable',
                                   default=None,
@@ -299,14 +329,16 @@
 
         try:
             client.edit(
                 parsed_args.datastore_version_id,
                 datastore_manager=parsed_args.datastore_manager,
                 image=parsed_args.image,
                 image_tags=image_tags,
+                registry_ext=parsed_args.registry_ext,
+                repl_strategy=parsed_args.repl_strategy,
                 active=parsed_args.enable, default=parsed_args.default,
                 name=parsed_args.version_name
             )
         except Exception as e:
             msg = (_("Failed to update datastore version %(version)s: %(e)s")
                    % {'version': parsed_args.datastore_version_id, 'e': e})
             raise exceptions.CommandError(msg)
```

### Comparing `python-troveclient-8.4.0/troveclient/service_catalog.py` & `python-troveclient-8.5.0/troveclient/service_catalog.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/shell.py` & `python-troveclient-8.5.0/troveclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/fakes.py` & `python-troveclient-8.5.0/troveclient/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/fakes.py` & `python-troveclient-8.5.0/troveclient/tests/osc/fakes.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/utils.py` & `python-troveclient-8.5.0/troveclient/tests/osc/utils.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/v1/fakes.py` & `python-troveclient-8.5.0/troveclient/tests/osc/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_backup_strategy.py` & `python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_backup_strategy.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_backups.py` & `python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_backups.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_clusters.py` & `python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_clusters.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_configurations.py` & `python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_configurations.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_flavors.py` & `python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_flavors.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_instances.py` & `python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_instances.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_limits.py` & `python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_limits.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_logs.py` & `python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_logs.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_quota.py` & `python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_quota.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_root.py` & `python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_root.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/v1/test_database_users.py` & `python-troveclient-8.5.0/troveclient/tests/osc/v1/test_database_users.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/v1/test_databases.py` & `python-troveclient-8.5.0/troveclient/tests/osc/v1/test_databases.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/osc/v1/test_datastores.py` & `python-troveclient-8.5.0/troveclient/tests/osc/v1/test_datastores.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,35 +162,40 @@
     def setUp(self):
         super(TestCreateDatastoreVersion, self).setUp()
         self.cmd = datastores.CreateDatastoreVersion(self.app, None)
 
     def test_create_datastore_version(self):
         image_id = uuidutils.generate_uuid()
         args = ['new_name', 'ds_name', 'ds_manager', image_id, '--active',
-                '--default', '--image-tags', 'trove,mysql']
+                '--default', '--image-tags', 'trove,mysql',
+                '--registry-ext', 'registry-ext',
+                '--repl-strategy', 'repl_strategy']
         parsed_args = self.check_parser(self.cmd, args, [])
 
         self.cmd.take_action(parsed_args)
 
         self.dsversion_mgmt_client.create.assert_called_once_with(
             'new_name', 'ds_name', 'ds_manager', image_id, active='true',
             default='true', image_tags=['trove', 'mysql'],
-            version=None)
+            registry_ext="registry-ext",
+            repl_strategy="repl_strategy", version=None)
 
 
 class TestUpdateDatastoreVersion(TestDatastores):
     def setUp(self):
         super(TestUpdateDatastoreVersion, self).setUp()
         self.cmd = datastores.UpdateDatastoreVersion(self.app, None)
 
     def test_update_datastore_version(self):
         version_id = uuidutils.generate_uuid()
-        args = [version_id, '--image-tags', 'trove,mysql', '--enable',
-                '--non-default']
+        args = [version_id, '--registry-ext', 'registry-ext',
+                '--repl-strategy', 'repl_strategy',
+                '--image-tags', 'trove,mysql', '--enable', '--non-default']
         parsed_args = self.check_parser(self.cmd, args, [])
 
         self.cmd.take_action(parsed_args)
 
         self.dsversion_mgmt_client.edit.assert_called_once_with(
             version_id, datastore_manager=None, image=None,
             active='true', default='false', image_tags=['trove', 'mysql'],
-            name=None)
+            registry_ext="registry-ext",
+            repl_strategy="repl_strategy", name=None)
```

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_accounts.py` & `python-troveclient-8.5.0/troveclient/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_apiclient_exceptions.py` & `python-troveclient-8.5.0/troveclient/tests/test_apiclient_exceptions.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_backups.py` & `python-troveclient-8.5.0/troveclient/tests/test_backups.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_base.py` & `python-troveclient-8.5.0/troveclient/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_client.py` & `python-troveclient-8.5.0/troveclient/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_clusters.py` & `python-troveclient-8.5.0/troveclient/tests/test_clusters.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_common.py` & `python-troveclient-8.5.0/troveclient/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_configurations.py` & `python-troveclient-8.5.0/troveclient/tests/test_configurations.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_databases.py` & `python-troveclient-8.5.0/troveclient/tests/test_databases.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_datastores.py` & `python-troveclient-8.5.0/troveclient/tests/test_datastores.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_discover.py` & `python-troveclient-8.5.0/troveclient/tests/test_discover.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_instances.py` & `python-troveclient-8.5.0/troveclient/tests/test_instances.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_limits.py` & `python-troveclient-8.5.0/troveclient/tests/test_limits.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_management.py` & `python-troveclient-8.5.0/troveclient/tests/test_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -231,20 +231,23 @@
     def test_create(self):
         def side_effect_func(path, body, *kw):
             return path, body
 
         self.ds_version._create = mock.Mock(side_effect=side_effect_func)
         p, b, = self.ds_version.create(
             "ds-version1", "mysql", "mysql", "image-id",
-            ["mysql-server-5.5"], "true", "true")
+            ["mysql-server-5.5"], "registry-ext",
+            "repl-strategy", "true", "true")
         self.assertEqual("/mgmt/datastore-versions", p)
         self.assertEqual("ds-version1", b["version"]["name"])
         self.assertEqual("mysql", b["version"]["datastore_name"])
         self.assertEqual("mysql", b["version"]["datastore_manager"])
         self.assertEqual("image-id", b["version"]["image"])
+        self.assertEqual("registry-ext", b["version"]["registry_ext"])
+        self.assertEqual("repl-strategy", b["version"]["repl_strategy"])
         self.assertEqual(["mysql-server-5.5"], b["version"]["packages"])
         self.assertTrue(b["version"]["active"])
         self.assertTrue(b["version"]["default"])
 
     def test_get(self):
         def side_effect_func(path, ins):
             return path, ins
```

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_metadata.py` & `python-troveclient-8.5.0/troveclient/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_modules.py` & `python-troveclient-8.5.0/troveclient/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_root.py` & `python-troveclient-8.5.0/troveclient/tests/test_root.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_secgroups.py` & `python-troveclient-8.5.0/troveclient/tests/test_secgroups.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_shell.py` & `python-troveclient-8.5.0/troveclient/tests/test_shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,33 +8,29 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import io
+import json
 import re
 import sys
 from unittest import mock
 
 import fixtures
 from keystoneauth1 import fixture
 import requests_mock
 import testtools
 import uuid
 
 import troveclient.client
 from troveclient import exceptions
 import troveclient.shell
 
-try:
-    import json
-except ImportError:
-    import simplejson as json
-
 V2_URL = "http://no.where/v2.0"
 V3_URL = "http://no.where/v3"
 
 FAKE_V2_ENV = {'OS_USERNAME': uuid.uuid4().hex,
                'OS_PASSWORD': uuid.uuid4().hex,
                'OS_TENANT_ID': uuid.uuid4().hex,
                'OS_AUTH_URL': V2_URL}
```

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_users.py` & `python-troveclient-8.5.0/troveclient/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/test_utils.py` & `python-troveclient-8.5.0/troveclient/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/tests/utils.py` & `python-troveclient-8.5.0/troveclient/tests/utils.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/utils.py` & `python-troveclient-8.5.0/troveclient/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
+import base64
+import json
+import os
+import sys
 import uuid
 
-import base64
 from openstackclient.identity import common as identity_common
-import os
 from oslo_utils import encodeutils
 from oslo_utils import uuidutils
 import prettytable
-import simplejson as json
-import sys
 
 from troveclient.apiclient import exceptions
 
 
 def arg(*args, **kwargs):
     """Decorator for CLI args."""
     def _decorator(func):
```

### Comparing `python-troveclient-8.4.0/troveclient/v1/accounts.py` & `python-troveclient-8.5.0/troveclient/v1/accounts.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/backup_strategy.py` & `python-troveclient-8.5.0/troveclient/v1/backup_strategy.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/backups.py` & `python-troveclient-8.5.0/troveclient/v1/backups.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/client.py` & `python-troveclient-8.5.0/troveclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/clusters.py` & `python-troveclient-8.5.0/troveclient/v1/clusters.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/configurations.py` & `python-troveclient-8.5.0/troveclient/v1/configurations.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/databases.py` & `python-troveclient-8.5.0/troveclient/v1/databases.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/datastores.py` & `python-troveclient-8.5.0/troveclient/v1/datastores.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/diagnostics.py` & `python-troveclient-8.5.0/troveclient/v1/diagnostics.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/flavors.py` & `python-troveclient-8.5.0/troveclient/v1/flavors.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/hosts.py` & `python-troveclient-8.5.0/troveclient/v1/hosts.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/instances.py` & `python-troveclient-8.5.0/troveclient/v1/instances.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/limits.py` & `python-troveclient-8.5.0/troveclient/v1/limits.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/management.py` & `python-troveclient-8.5.0/troveclient/v1/management.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,16 +264,16 @@
 
     def get(self, datastore_version_id):
         """Get details of a datastore version."""
         return self._get("/mgmt/datastore-versions/%s" % datastore_version_id,
                          "version")
 
     def create(self, name, datastore_name, datastore_manager, image,
-               packages=None, active='true', default='false', image_tags=[],
-               version=None):
+               packages=None, registry_ext=None, repl_strategy=None,
+               active='true', default='false', image_tags=[], version=None):
         """Create a new datastore version."""
         packages = packages or []
         body = {
             "version": {
                 "name": name,
                 "datastore_name": datastore_name,
                 "datastore_manager": datastore_manager,
@@ -281,31 +281,40 @@
                 "packages": packages,
                 "active": json.loads(active),
                 "default": json.loads(default)
             }
         }
         if image:
             body['version']['image'] = image
+
+        if registry_ext:
+            body['version']['registry_ext'] = registry_ext
+        if repl_strategy:
+            body['version']['repl_strategy'] = repl_strategy
         if version:
             body['version']['version'] = version
 
         return self._create("/mgmt/datastore-versions", body, None, True)
 
     def edit(self, datastore_version_id, datastore_manager=None, image=None,
-             packages=None, active=None, default=None, image_tags=None,
-             name=None):
+             packages=None, registry_ext=None, repl_strategy=None,
+             active=None, default=None, image_tags=None, name=None):
         """Update a datastore-version."""
         packages = packages or []
         body = {}
         if datastore_manager is not None:
             body['datastore_manager'] = datastore_manager
         if image is not None:
             body['image'] = image
         if packages:
             body['packages'] = packages
+        if registry_ext:
+            body['registry_ext'] = registry_ext
+        if repl_strategy:
+            body['repl_strategy'] = repl_strategy
         if active is not None:
             body['active'] = json.loads(active)
         if default is not None:
             body['default'] = json.loads(default)
         if image_tags is not None:
             body['image_tags'] = image_tags
         if name:
```

### Comparing `python-troveclient-8.4.0/troveclient/v1/metadata.py` & `python-troveclient-8.5.0/troveclient/v1/metadata.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/modules.py` & `python-troveclient-8.5.0/troveclient/v1/modules.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/quota.py` & `python-troveclient-8.5.0/troveclient/v1/quota.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/root.py` & `python-troveclient-8.5.0/troveclient/v1/root.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/security_groups.py` & `python-troveclient-8.5.0/troveclient/v1/security_groups.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/shell.py` & `python-troveclient-8.5.0/troveclient/v1/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,20 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import argparse
+import json
 import sys
 import time
 
 from troveclient.i18n import _
 
-try:
-    import simplejson as json
-except ImportError:
-    import json
-
 from troveclient import exceptions
 from troveclient import utils
 from troveclient.v1 import modules
 
 INSTANCE_ARG_NAME = _('instance')
 INSTANCE_METAVAR = _('"opt=<value>[,opt=<value> ...] "')
 INSTANCE_ERROR = _("Instance argument(s) must be of the form --instance "
```

### Comparing `python-troveclient-8.4.0/troveclient/v1/storage.py` & `python-troveclient-8.5.0/troveclient/v1/storage.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/users.py` & `python-troveclient-8.5.0/troveclient/v1/users.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.4.0/troveclient/v1/volume_types.py` & `python-troveclient-8.5.0/troveclient/v1/volume_types.py`

 * *Files identical despite different names*

