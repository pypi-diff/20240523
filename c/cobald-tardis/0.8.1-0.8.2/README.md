# Comparing `tmp/cobald-tardis-0.8.1.tar.gz` & `tmp/cobald-tardis-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobald-tardis-0.8.1.tar", last modified: Wed Nov 29 11:12:26 2023, max compression
+gzip compressed data, was "cobald-tardis-0.8.2.tar", last modified: Thu May 23 11:48:08 2024, max compression
```

## Comparing `cobald-tardis-0.8.1.tar` & `cobald-tardis-0.8.2.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.233869 cobald-tardis-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2023-11-29 11:12:26.233869 cobald-tardis-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.213869 cobald-tardis-0.8.1/cobald_tardis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2023-11-29 11:12:26.000000 cobald-tardis-0.8.1/cobald_tardis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2023-11-29 11:12:26.000000 cobald-tardis-0.8.1/cobald_tardis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 11:12:26.000000 cobald-tardis-0.8.1/cobald_tardis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      706 2023-11-29 11:12:26.000000 cobald-tardis-0.8.1/cobald_tardis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 11:12:26.000000 cobald-tardis-0.8.1/cobald_tardis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-11-29 11:12:26.000000 cobald-tardis-0.8.1/cobald_tardis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-29 11:12:26.000000 cobald-tardis-0.8.1/cobald_tardis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-29 11:12:26.233869 cobald-tardis-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.213869 cobald-tardis-0.8.1/tardis/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.213869 cobald-tardis-0.8.1/tardis/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.217869 cobald-tardis-0.8.1/tardis/adapters/batchsystems/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/adapters/batchsystems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/adapters/batchsystems/fakebatchsystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     9562 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/adapters/batchsystems/htcondor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9456 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/adapters/batchsystems/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.217869 cobald-tardis-0.8.1/tardis/adapters/sites/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/adapters/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/adapters/sites/cloudstack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/adapters/sites/fakesite.py
--rw-r--r--   0 runner    (1001) docker     (127)    10759 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/adapters/sites/htcondor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8681 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/adapters/sites/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/adapters/sites/moab.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/adapters/sites/openstack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/adapters/sites/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.217869 cobald-tardis-0.8.1/tardis/agents/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/agents/batchsystemagent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/agents/siteagent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.217869 cobald-tardis-0.8.1/tardis/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/configuration/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.217869 cobald-tardis-0.8.1/tardis/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/exceptions/executorexceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/exceptions/tardisexceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.221869 cobald-tardis-0.8.1/tardis/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/interfaces/batchsystemadapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/interfaces/borg.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/interfaces/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/interfaces/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/interfaces/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10862 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/interfaces/siteadapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/interfaces/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.221869 cobald-tardis-0.8.1/tardis/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/plugins/auditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/plugins/elasticsearchmonitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/plugins/prometheusmonitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/plugins/sqliteregistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/plugins/telegrafmonitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.221869 cobald-tardis-0.8.1/tardis/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/resources/drone.py
--rw-r--r--   0 runner    (1001) docker     (127)    12676 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/resources/dronestates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/resources/poolfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.221869 cobald-tardis-0.8.1/tardis/rest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.221869 cobald-tardis-0.8.1/tardis/rest/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/rest/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/rest/app/crud.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/rest/app/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/rest/app/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.221869 cobald-tardis-0.8.1/tardis/rest/app/routers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/rest/app/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/rest/app/routers/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/rest/app/routers/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/rest/app/routers/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/rest/app/scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/rest/app/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.221869 cobald-tardis-0.8.1/tardis/rest/hash_credentials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/rest/hash_credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/rest/hash_credentials/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/rest/hash_credentials/hash_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/rest/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.225869 cobald-tardis-0.8.1/tardis/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7666 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/utilities/asyncbulkcall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/utilities/asynccachemap.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/utilities/attributedict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.225869 cobald-tardis-0.8.1/tardis/utilities/executors/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/utilities/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/utilities/executors/shellexecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/utilities/executors/sshexecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/utilities/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.225869 cobald-tardis-0.8.1/tardis/utilities/simulators/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/utilities/simulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/utilities/simulators/periodicvalue.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/utilities/simulators/randomgauss.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/utilities/staticmapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tardis/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.213869 cobald-tardis-0.8.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.225869 cobald-tardis-0.8.1/tests/adapters_t/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/adapters_t/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.225869 cobald-tardis-0.8.1/tests/adapters_t/batchsystems_t/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/adapters_t/batchsystems_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/adapters_t/batchsystems_t/test_fakebatchsystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    11571 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/adapters_t/batchsystems_t/test_htcondor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/adapters_t/batchsystems_t/test_slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.225869 cobald-tardis-0.8.1/tests/adapters_t/sites_t/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/adapters_t/sites_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7493 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/adapters_t/sites_t/test_cloudstack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/adapters_t/sites_t/test_fakesite.py
--rw-r--r--   0 runner    (1001) docker     (127)    14875 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/adapters_t/sites_t/test_htcondorsiteadapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13146 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/adapters_t/sites_t/test_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18934 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/adapters_t/sites_t/test_moab.py
--rw-r--r--   0 runner    (1001) docker     (127)     8061 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/adapters_t/sites_t/test_openstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    13848 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/adapters_t/sites_t/test_slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.225869 cobald-tardis-0.8.1/tests/agents_t/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/agents_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/agents_t/test_batchsystemagent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/agents_t/test_siteagent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.229869 cobald-tardis-0.8.1/tests/configuration_t/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/configuration_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/configuration_t/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/configuration_t/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.229869 cobald-tardis-0.8.1/tests/interfaces_t/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/interfaces_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/interfaces_t/test_batchsystemadapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9441 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/interfaces_t/test_siteadapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.229869 cobald-tardis-0.8.1/tests/plugins_t/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/plugins_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/plugins_t/test_auditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/plugins_t/test_elasticsearchmonitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/plugins_t/test_prometheusmonitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    12092 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/plugins_t/test_sqliteregistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/plugins_t/test_telegrafmonitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.229869 cobald-tardis-0.8.1/tests/resources_t/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/resources_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/resources_t/test_drone.py
--rw-r--r--   0 runner    (1001) docker     (127)    14950 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/resources_t/test_dronestates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/resources_t/test_poolfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.229869 cobald-tardis-0.8.1/tests/rest_t/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/rest_t/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.229869 cobald-tardis-0.8.1/tests/rest_t/app_t/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/rest_t/app_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/rest_t/app_t/test_crutd.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/rest_t/app_t/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/rest_t/app_t/test_security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.229869 cobald-tardis-0.8.1/tests/rest_t/hash_credentials_t/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/rest_t/hash_credentials_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/rest_t/hash_credentials_t/test_hash_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/rest_t/hash_credentials_t/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.229869 cobald-tardis-0.8.1/tests/rest_t/routers_t/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/rest_t/routers_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/rest_t/routers_t/base_test_case_routers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/rest_t/routers_t/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/rest_t/routers_t/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/rest_t/routers_t/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/rest_t/test_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.233869 cobald-tardis-0.8.1/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/utilities/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.233869 cobald-tardis-0.8.1/tests/utilities_t/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/utilities_t/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.233869 cobald-tardis-0.8.1/tests/utilities_t/executors_t/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/utilities_t/executors_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/utilities_t/executors_t/test_shellexecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8082 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/utilities_t/executors_t/test_sshexecutor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:26.233869 cobald-tardis-0.8.1/tests/utilities_t/simulators_t/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/utilities_t/simulators_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/utilities_t/simulators_t/test_periodicvalue.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/utilities_t/simulators_t/test_randomgauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/utilities_t/test_asyncbulkcall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/utilities_t/test_asynccachemap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/utilities_t/test_attributedict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/utilities_t/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/utilities_t/test_staticmapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2023-11-29 11:12:15.000000 cobald-tardis-0.8.1/tests/utilities_t/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.089680 cobald-tardis-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-23 11:48:08.089680 cobald-tardis-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.069680 cobald-tardis-0.8.2/cobald_tardis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-23 11:48:07.000000 cobald-tardis-0.8.2/cobald_tardis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-23 11:48:08.000000 cobald-tardis-0.8.2/cobald_tardis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:48:07.000000 cobald-tardis-0.8.2/cobald_tardis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-23 11:48:07.000000 cobald-tardis-0.8.2/cobald_tardis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:48:07.000000 cobald-tardis-0.8.2/cobald_tardis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-23 11:48:07.000000 cobald-tardis-0.8.2/cobald_tardis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 11:48:07.000000 cobald-tardis-0.8.2/cobald_tardis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-23 11:48:08.089680 cobald-tardis-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.069680 cobald-tardis-0.8.2/tardis/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.069680 cobald-tardis-0.8.2/tardis/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.069680 cobald-tardis-0.8.2/tardis/adapters/batchsystems/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/adapters/batchsystems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/adapters/batchsystems/fakebatchsystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/adapters/batchsystems/htcondor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/adapters/batchsystems/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.069680 cobald-tardis-0.8.2/tardis/adapters/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/adapters/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/adapters/sites/cloudstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/adapters/sites/fakesite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/adapters/sites/htcondor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/adapters/sites/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/adapters/sites/moab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/adapters/sites/openstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/adapters/sites/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.069680 cobald-tardis-0.8.2/tardis/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/agents/batchsystemagent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/agents/siteagent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.073680 cobald-tardis-0.8.2/tardis/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/configuration/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.073680 cobald-tardis-0.8.2/tardis/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/exceptions/executorexceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/exceptions/tardisexceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.073680 cobald-tardis-0.8.2/tardis/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/interfaces/batchsystemadapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/interfaces/borg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/interfaces/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/interfaces/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/interfaces/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/interfaces/siteadapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/interfaces/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.073680 cobald-tardis-0.8.2/tardis/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/plugins/auditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/plugins/elasticsearchmonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/plugins/prometheusmonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/plugins/sqliteregistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/plugins/telegrafmonitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.073680 cobald-tardis-0.8.2/tardis/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/resources/drone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12676 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/resources/dronestates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/resources/poolfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.073680 cobald-tardis-0.8.2/tardis/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.077680 cobald-tardis-0.8.2/tardis/rest/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/rest/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/rest/app/crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/rest/app/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/rest/app/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.077680 cobald-tardis-0.8.2/tardis/rest/app/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/rest/app/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/rest/app/routers/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/rest/app/routers/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/rest/app/routers/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/rest/app/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/rest/app/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.077680 cobald-tardis-0.8.2/tardis/rest/hash_credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/rest/hash_credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/rest/hash_credentials/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/rest/hash_credentials/hash_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/rest/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.077680 cobald-tardis-0.8.2/tardis/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/utilities/asyncbulkcall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/utilities/asynccachemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/utilities/attributedict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.077680 cobald-tardis-0.8.2/tardis/utilities/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/utilities/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/utilities/executors/shellexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/utilities/executors/sshexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/utilities/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.077680 cobald-tardis-0.8.2/tardis/utilities/simulators/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/utilities/simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/utilities/simulators/periodicvalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/utilities/simulators/randomgauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/utilities/staticmapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tardis/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.065680 cobald-tardis-0.8.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.077680 cobald-tardis-0.8.2/tests/adapters_t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/adapters_t/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.081680 cobald-tardis-0.8.2/tests/adapters_t/batchsystems_t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/adapters_t/batchsystems_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/adapters_t/batchsystems_t/test_fakebatchsystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/adapters_t/batchsystems_t/test_htcondor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/adapters_t/batchsystems_t/test_slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.081680 cobald-tardis-0.8.2/tests/adapters_t/sites_t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/adapters_t/sites_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/adapters_t/sites_t/test_cloudstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/adapters_t/sites_t/test_fakesite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14875 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/adapters_t/sites_t/test_htcondorsiteadapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/adapters_t/sites_t/test_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18934 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/adapters_t/sites_t/test_moab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/adapters_t/sites_t/test_openstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15577 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/adapters_t/sites_t/test_slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.081680 cobald-tardis-0.8.2/tests/agents_t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/agents_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/agents_t/test_batchsystemagent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/agents_t/test_siteagent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.081680 cobald-tardis-0.8.2/tests/configuration_t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/configuration_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/configuration_t/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/configuration_t/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.081680 cobald-tardis-0.8.2/tests/interfaces_t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/interfaces_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/interfaces_t/test_batchsystemadapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/interfaces_t/test_siteadapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.085680 cobald-tardis-0.8.2/tests/plugins_t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/plugins_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/plugins_t/test_auditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/plugins_t/test_elasticsearchmonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/plugins_t/test_prometheusmonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/plugins_t/test_sqliteregistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/plugins_t/test_telegrafmonitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.085680 cobald-tardis-0.8.2/tests/resources_t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/resources_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/resources_t/test_drone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14950 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/resources_t/test_dronestates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/resources_t/test_poolfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.085680 cobald-tardis-0.8.2/tests/rest_t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/rest_t/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.085680 cobald-tardis-0.8.2/tests/rest_t/app_t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/rest_t/app_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/rest_t/app_t/test_crutd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/rest_t/app_t/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/rest_t/app_t/test_security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.085680 cobald-tardis-0.8.2/tests/rest_t/hash_credentials_t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/rest_t/hash_credentials_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/rest_t/hash_credentials_t/test_hash_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/rest_t/hash_credentials_t/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.085680 cobald-tardis-0.8.2/tests/rest_t/routers_t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/rest_t/routers_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/rest_t/routers_t/base_test_case_routers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/rest_t/routers_t/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/rest_t/routers_t/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/rest_t/routers_t/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/rest_t/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.085680 cobald-tardis-0.8.2/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.089680 cobald-tardis-0.8.2/tests/utilities_t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/utilities_t/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.089680 cobald-tardis-0.8.2/tests/utilities_t/executors_t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/utilities_t/executors_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/utilities_t/executors_t/test_shellexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/utilities_t/executors_t/test_sshexecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:48:08.089680 cobald-tardis-0.8.2/tests/utilities_t/simulators_t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/utilities_t/simulators_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/utilities_t/simulators_t/test_periodicvalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/utilities_t/simulators_t/test_randomgauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/utilities_t/test_asyncbulkcall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/utilities_t/test_asynccachemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/utilities_t/test_attributedict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/utilities_t/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/utilities_t/test_staticmapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-23 11:47:55.000000 cobald-tardis-0.8.2/tests/utilities_t/test_utils.py
```

### Comparing `cobald-tardis-0.8.1/LICENSE.txt` & `cobald-tardis-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/PKG-INFO` & `cobald-tardis-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobald-tardis
-Version: 0.8.1
+Version: 0.8.2
 Summary: Transparent Adaptive Resource Dynamic Integration System
 Home-page: https://github.com/matterminers/tardis
 Author: Manuel Giffels, Matthias Schnepf
 Author-email: giffels@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/matterminers/tardis/issues
 Project-URL: Source, https://github.com/matterminers/tardis
```

### Comparing `cobald-tardis-0.8.1/README.md` & `cobald-tardis-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/cobald_tardis.egg-info/PKG-INFO` & `cobald-tardis-0.8.2/cobald_tardis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobald-tardis
-Version: 0.8.1
+Version: 0.8.2
 Summary: Transparent Adaptive Resource Dynamic Integration System
 Home-page: https://github.com/matterminers/tardis
 Author: Manuel Giffels, Matthias Schnepf
 Author-email: giffels@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/matterminers/tardis/issues
 Project-URL: Source, https://github.com/matterminers/tardis
```

### Comparing `cobald-tardis-0.8.1/cobald_tardis.egg-info/SOURCES.txt` & `cobald-tardis-0.8.2/cobald_tardis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/cobald_tardis.egg-info/entry_points.txt` & `cobald-tardis-0.8.2/cobald_tardis.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/cobald_tardis.egg-info/requires.txt` & `cobald-tardis-0.8.2/cobald_tardis.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 elasticsearch<8.0.0,>=7.17
 aioprometheus>=21.9.0
 kubernetes_asyncio
 pydantic<2.0.0
 asyncstdlib
 async-timeout
 typing_extensions
-python-auditor==0.3.1
+python-auditor==0.5.0
 tzlocal
 fastapi-jwt-auth
 fastapi
 python-jose
 uvicorn[standard]
 typer
 bcrypt
```

### Comparing `cobald-tardis-0.8.1/setup.py` & `cobald-tardis-0.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         "elasticsearch>=7.17,<8.0.0",
         "aioprometheus>=21.9.0",
         "kubernetes_asyncio",
         "pydantic<2.0.0",
         "asyncstdlib",
         "async-timeout",
         "typing_extensions",
-        "python-auditor==0.3.1",
+        "python-auditor==0.5.0",
         "tzlocal",
         *REST_REQUIRES,
     ],
     extras_require={
         "docs": [
             "docutils<0.17",  # fixes rendering issue with two column layout
             "sphinx",
```

### Comparing `cobald-tardis-0.8.1/tardis/adapters/batchsystems/fakebatchsystem.py` & `cobald-tardis-0.8.2/tardis/adapters/batchsystems/fakebatchsystem.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/adapters/batchsystems/htcondor.py` & `cobald-tardis-0.8.2/tardis/adapters/batchsystems/htcondor.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/adapters/batchsystems/slurm.py` & `cobald-tardis-0.8.2/tardis/adapters/batchsystems/slurm.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/adapters/sites/cloudstack.py` & `cobald-tardis-0.8.2/tardis/adapters/sites/cloudstack.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/adapters/sites/fakesite.py` & `cobald-tardis-0.8.2/tardis/adapters/sites/fakesite.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         resource_boot_time = self._resource_boot_time.get_value()
         # check if resource should already run
         if (datetime.now() - created_time) > timedelta(
             seconds=resource_boot_time
         ) and resource_attributes.get(
             "resource_status",
-            ResourceStatus.Booting
+            ResourceStatus.Booting,
             # When cobald is restarted, "resource_status" is not set. Since this is a
             # FakeAdapter, when can safely start the cycle again by assuming
             # ResourceStatus.Booting and let TARDIS manage the drone's life cycle
         ) is ResourceStatus.Booting:
             return self.handle_response(
                 AttributeDict(resource_status=ResourceStatus.Running)
             )
```

### Comparing `cobald-tardis-0.8.1/tardis/adapters/sites/htcondor.py` & `cobald-tardis-0.8.2/tardis/adapters/sites/htcondor.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/adapters/sites/kubernetes.py` & `cobald-tardis-0.8.2/tardis/adapters/sites/kubernetes.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/adapters/sites/moab.py` & `cobald-tardis-0.8.2/tardis/adapters/sites/moab.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/adapters/sites/openstack.py` & `cobald-tardis-0.8.2/tardis/adapters/sites/openstack.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/adapters/sites/slurm.py` & `cobald-tardis-0.8.2/tardis/adapters/sites/slurm.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,16 +41,26 @@
     cmd = f'squeue -o "{attributes_string}" -h -t all --job={remote_resource_ids}'
 
     slurm_resource_status = {}
     logger.debug("Slurm status update is started.")
     try:
         slurm_status = await executor.run_command(cmd)
     except CommandExecutionFailure as cf:
+        # In case a job is already completed and
+        # only **one** non-existing job id is provided
+        # squeue is failing with exit code 1
+        # and prints "Invalid job id specified" to stderr
+        if "Invalid job id specified" in cf.stderr and len(resource_attributes) == 1:
+            logger.info(
+                f"{remote_resource_ids} is not valid anymore. Assuming it is completed."
+            )
+            return [{"State": "COMPLETED"}]
         logger.warning(f"Slurm status update has failed due to {cf}.")
         raise
+
     else:
         for row in csv_parser(
             slurm_status.stdout, fieldnames=tuple(attributes.keys()), delimiter="|"
         ):
             row["State"] = row["State"].strip()
             slurm_resource_status[row["JobId"]] = row
         logger.debug("Slurm status update finished.")
```

### Comparing `cobald-tardis-0.8.1/tardis/agents/batchsystemagent.py` & `cobald-tardis-0.8.2/tardis/agents/batchsystemagent.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/agents/siteagent.py` & `cobald-tardis-0.8.2/tardis/agents/siteagent.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/configuration/configuration.py` & `cobald-tardis-0.8.2/tardis/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/configuration/utilities.py` & `cobald-tardis-0.8.2/tardis/configuration/utilities.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/exceptions/executorexceptions.py` & `cobald-tardis-0.8.2/tardis/exceptions/executorexceptions.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/interfaces/batchsystemadapter.py` & `cobald-tardis-0.8.2/tardis/interfaces/batchsystemadapter.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/interfaces/borg.py` & `cobald-tardis-0.8.2/tardis/interfaces/borg.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/interfaces/siteadapter.py` & `cobald-tardis-0.8.2/tardis/interfaces/siteadapter.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/interfaces/state.py` & `cobald-tardis-0.8.2/tardis/interfaces/state.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/plugins/auditor.py` & `cobald-tardis-0.8.2/tardis/plugins/auditor.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/plugins/elasticsearchmonitoring.py` & `cobald-tardis-0.8.2/tardis/plugins/elasticsearchmonitoring.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/plugins/prometheusmonitoring.py` & `cobald-tardis-0.8.2/tardis/plugins/prometheusmonitoring.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/plugins/sqliteregistry.py` & `cobald-tardis-0.8.2/tardis/plugins/sqliteregistry.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/plugins/telegrafmonitoring.py` & `cobald-tardis-0.8.2/tardis/plugins/telegrafmonitoring.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/resources/drone.py` & `cobald-tardis-0.8.2/tardis/resources/drone.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/resources/dronestates.py` & `cobald-tardis-0.8.2/tardis/resources/dronestates.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/resources/poolfactory.py` & `cobald-tardis-0.8.2/tardis/resources/poolfactory.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/rest/app/crud.py` & `cobald-tardis-0.8.2/tardis/rest/app/crud.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/rest/app/main.py` & `cobald-tardis-0.8.2/tardis/rest/app/main.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/rest/app/routers/resources.py` & `cobald-tardis-0.8.2/tardis/rest/app/routers/resources.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/rest/app/routers/types.py` & `cobald-tardis-0.8.2/tardis/rest/app/routers/types.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/rest/app/routers/user.py` & `cobald-tardis-0.8.2/tardis/rest/app/routers/user.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/rest/app/security.py` & `cobald-tardis-0.8.2/tardis/rest/app/security.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/rest/service.py` & `cobald-tardis-0.8.2/tardis/rest/service.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/utilities/asyncbulkcall.py` & `cobald-tardis-0.8.2/tardis/utilities/asyncbulkcall.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 
     A bulk command must take an arbitrary number of tasks and is expected to provide
     an iterable of one result per task. Alternatively, it may provide a single
     :py:data:`None` value to indicate that there is no result. An unhandled
     :py:class:`Exception` means that all tasks failed with that :py:class:`Exception`.
     """
 
-    async def __call__(self, *__tasks: T) -> Optional[Iterable[R]]:
-        ...
+    async def __call__(self, *__tasks: T) -> Optional[Iterable[R]]: ...  # noqa E704
 
 
 class AsyncBulkCall(Generic[T, R]):
     """
     Framework for queueing and executing several tasks via bulk commands
 
     :param command: async callable that executes several tasks
```

### Comparing `cobald-tardis-0.8.1/tardis/utilities/asynccachemap.py` & `cobald-tardis-0.8.2/tardis/utilities/asynccachemap.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/utilities/attributedict.py` & `cobald-tardis-0.8.2/tardis/utilities/attributedict.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/utilities/executors/shellexecutor.py` & `cobald-tardis-0.8.2/tardis/utilities/executors/shellexecutor.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/utilities/executors/sshexecutor.py` & `cobald-tardis-0.8.2/tardis/utilities/executors/sshexecutor.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/utilities/pipeline.py` & `cobald-tardis-0.8.2/tardis/utilities/pipeline.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/utilities/simulators/periodicvalue.py` & `cobald-tardis-0.8.2/tardis/utilities/simulators/periodicvalue.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/utilities/simulators/randomgauss.py` & `cobald-tardis-0.8.2/tardis/utilities/simulators/randomgauss.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tardis/utilities/utils.py` & `cobald-tardis-0.8.2/tardis/utilities/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,19 @@
     :type skipinitialspace: bool
     :param skiptrailingspace: ignore whitespace at the end of each csv row
     :type skiptrailingspace: bool
     """
     if skiptrailingspace:
         input_csv = "\n".join((line.strip() for line in input_csv.splitlines()))
 
+    if len(fieldnames) > 1:
+        input_csv = "\n".join(
+            (line for line in input_csv.splitlines() if delimiter in line)
+        )
+
     replacements = replacements or {}
     with StringIO(input_csv) as csv_input:
         csv_reader = csv.DictReader(
             csv_input,
             fieldnames=fieldnames,
             delimiter=delimiter,
             skipinitialspace=skipinitialspace,
```

### Comparing `cobald-tardis-0.8.1/tests/adapters_t/batchsystems_t/test_fakebatchsystem.py` & `cobald-tardis-0.8.2/tests/adapters_t/batchsystems_t/test_fakebatchsystem.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/adapters_t/batchsystems_t/test_htcondor.py` & `cobald-tardis-0.8.2/tests/adapters_t/batchsystems_t/test_htcondor.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/adapters_t/batchsystems_t/test_slurm.py` & `cobald-tardis-0.8.2/tests/adapters_t/batchsystems_t/test_slurm.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/adapters_t/sites_t/test_cloudstack.py` & `cobald-tardis-0.8.2/tests/adapters_t/sites_t/test_cloudstack.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/adapters_t/sites_t/test_fakesite.py` & `cobald-tardis-0.8.2/tests/adapters_t/sites_t/test_fakesite.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/adapters_t/sites_t/test_htcondorsiteadapter.py` & `cobald-tardis-0.8.2/tests/adapters_t/sites_t/test_htcondorsiteadapter.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/adapters_t/sites_t/test_kubernetes.py` & `cobald-tardis-0.8.2/tests/adapters_t/sites_t/test_kubernetes.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/adapters_t/sites_t/test_moab.py` & `cobald-tardis-0.8.2/tests/adapters_t/sites_t/test_moab.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/adapters_t/sites_t/test_openstack.py` & `cobald-tardis-0.8.2/tests/adapters_t/sites_t/test_openstack.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/adapters_t/sites_t/test_slurm.py` & `cobald-tardis-0.8.2/tests/adapters_t/sites_t/test_slurm.py`

 * *Files 4% similar despite different names*

```diff
@@ -300,15 +300,15 @@
             self.mock_executor.return_value.run_command.assert_called_with(
                 f'squeue -o "%A|%N|%T" -h -t all --job={job_id}'
             )
 
             self.mock_executor.reset_mock()
 
     @mock_executor_run_command("")
-    def test_resource_status_of_completed_jobs(self):
+    def test_resource_status_of_completed_jobs_w_empty_reply(self):
         response = run_async(
             self.slurm_adapter.resource_status,
             AttributeDict(
                 resource_id="1390065",
                 remote_resource_uuid="1351043",
             ),
         )
@@ -318,14 +318,64 @@
         self.mock_executor.return_value.run_command.assert_called_with(
             'squeue -o "%A|%N|%T" -h -t all --job=1351043'
         )
 
     @mock_executor_run_command(
         stdout="",
         raise_exception=CommandExecutionFailure(
+            message="Run command squeue --job=1351043 via SSHExecutor failed",
+            stdout="",
+            stderr="slurm_load_jobs error: Invalid job id specified",
+            exit_code=1,
+        ),
+    )
+    def test_resource_status_of_completed_jobs_w_raised_exception(self):
+        response = run_async(
+            self.slurm_adapter.resource_status,
+            AttributeDict(
+                resource_id="1390065",
+                remote_resource_uuid="1351043",
+            ),
+        )
+
+        self.assertEqual(response.resource_status, ResourceStatus.Deleted)
+
+        self.mock_executor.return_value.run_command.assert_called_with(
+            'squeue -o "%A|%N|%T" -h -t all --job=1351043'
+        )
+
+        # test that exception is re-raised if two or more job ids are specified,
+        # since Slurm does not fail in that case.
+
+        tasks = [
+            self.slurm_adapter.resource_status(
+                AttributeDict(
+                    resource_id="1390065",
+                    remote_resource_uuid="1351043",
+                ),
+            ),
+            self.slurm_adapter.resource_status(
+                AttributeDict(
+                    resource_id="1390066",
+                    remote_resource_uuid="1351044",
+                ),
+            ),
+        ]
+
+        with self.assertLogs(level=logging.WARNING):
+            with self.assertRaises(CommandExecutionFailure):
+                run_async(asyncio.gather, *tasks)
+
+        self.mock_executor.return_value.run_command.assert_called_with(
+            'squeue -o "%A|%N|%T" -h -t all --job=1351043,1351044'
+        )
+
+    @mock_executor_run_command(
+        stdout="",
+        raise_exception=CommandExecutionFailure(
             message="Failed", stdout="Failed", stderr="Failed", exit_code=2
         ),
     )
     def test_resource_status_update_failed(self):
         with self.assertLogs(level=logging.WARNING):
             with self.assertRaises(CommandExecutionFailure):
                 run_async(
```

### Comparing `cobald-tardis-0.8.1/tests/agents_t/test_batchsystemagent.py` & `cobald-tardis-0.8.2/tests/agents_t/test_batchsystemagent.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,17 +44,17 @@
         self.batch_system_adapter.get_utilisation.assert_called_with("test")
 
     def test_machine_meta_data_translation_mapping(self):
         machine_meta_data_translation_mock = PropertyMock(
             return_value=AttributeDict(Cores=1, Memory=1024, Disk=1024)
         )
 
-        type(
-            self.batch_system_adapter
-        ).machine_meta_data_translation_mapping = machine_meta_data_translation_mock
+        type(self.batch_system_adapter).machine_meta_data_translation_mapping = (
+            machine_meta_data_translation_mock
+        )
 
         self.assertEqual(
             AttributeDict(Cores=1, Memory=1024, Disk=1024),
             self.batch_system_agent.machine_meta_data_translation_mapping,
         )
 
         machine_meta_data_translation_mock.assert_called_once_with()
```

### Comparing `cobald-tardis-0.8.1/tests/agents_t/test_siteagent.py` & `cobald-tardis-0.8.2/tests/agents_t/test_siteagent.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/configuration_t/test_configuration.py` & `cobald-tardis-0.8.2/tests/configuration_t/test_configuration.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/configuration_t/test_utilities.py` & `cobald-tardis-0.8.2/tests/configuration_t/test_utilities.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/interfaces_t/test_batchsystemadapter.py` & `cobald-tardis-0.8.2/tests/interfaces_t/test_batchsystemadapter.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/interfaces_t/test_siteadapter.py` & `cobald-tardis-0.8.2/tests/interfaces_t/test_siteadapter.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/plugins_t/test_auditor.py` & `cobald-tardis-0.8.2/tests/plugins_t/test_auditor.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/plugins_t/test_elasticsearchmonitoring.py` & `cobald-tardis-0.8.2/tests/plugins_t/test_elasticsearchmonitoring.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/plugins_t/test_prometheusmonitoring.py` & `cobald-tardis-0.8.2/tests/plugins_t/test_prometheusmonitoring.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/plugins_t/test_sqliteregistry.py` & `cobald-tardis-0.8.2/tests/plugins_t/test_sqliteregistry.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/plugins_t/test_telegrafmonitoring.py` & `cobald-tardis-0.8.2/tests/plugins_t/test_telegrafmonitoring.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/resources_t/test_drone.py` & `cobald-tardis-0.8.2/tests/resources_t/test_drone.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/resources_t/test_dronestates.py` & `cobald-tardis-0.8.2/tests/resources_t/test_dronestates.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/resources_t/test_poolfactory.py` & `cobald-tardis-0.8.2/tests/resources_t/test_poolfactory.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/rest_t/app_t/test_crutd.py` & `cobald-tardis-0.8.2/tests/rest_t/app_t/test_crutd.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/rest_t/app_t/test_security.py` & `cobald-tardis-0.8.2/tests/rest_t/app_t/test_security.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/rest_t/hash_credentials_t/test_hash_credentials.py` & `cobald-tardis-0.8.2/tests/rest_t/hash_credentials_t/test_hash_credentials.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,14 @@
         self.app.command()(hash_credentials)
 
         self.runner = CliRunner()
 
     def test_hash_credentials(self):
         result = self.runner.invoke(self.app)
         self.assertNotEqual(result.exit_code, 0)
-        self.assertTrue("Error: Missing argument 'PASSWORD'." in result.stdout)
+        self.assertIn("Missing argument 'PASSWORD'.", result.stdout)
 
         result = self.runner.invoke(self.app, "test_password")
         self.assertEqual(result.exit_code, 0)
         # Hash is salted, therefore exact comparison is not possible
         self.assertTrue("$2b$12$" in result.stdout)
         self.assertEqual(60, len(result.stdout.strip()))
```

### Comparing `cobald-tardis-0.8.1/tests/rest_t/hash_credentials_t/test_main.py` & `cobald-tardis-0.8.2/tests/rest_t/hash_credentials_t/test_main.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/rest_t/routers_t/base_test_case_routers.py` & `cobald-tardis-0.8.2/tests/rest_t/routers_t/base_test_case_routers.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/rest_t/routers_t/test_resources.py` & `cobald-tardis-0.8.2/tests/rest_t/routers_t/test_resources.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/rest_t/routers_t/test_types.py` & `cobald-tardis-0.8.2/tests/rest_t/routers_t/test_types.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/rest_t/routers_t/test_user.py` & `cobald-tardis-0.8.2/tests/rest_t/routers_t/test_user.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/rest_t/test_service.py` & `cobald-tardis-0.8.2/tests/rest_t/test_service.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/utilities/utilities.py` & `cobald-tardis-0.8.2/tests/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/utilities_t/executors_t/test_shellexecutor.py` & `cobald-tardis-0.8.2/tests/utilities_t/executors_t/test_shellexecutor.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/utilities_t/executors_t/test_sshexecutor.py` & `cobald-tardis-0.8.2/tests/utilities_t/executors_t/test_sshexecutor.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/utilities_t/simulators_t/test_periodicvalue.py` & `cobald-tardis-0.8.2/tests/utilities_t/simulators_t/test_periodicvalue.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/utilities_t/simulators_t/test_randomgauss.py` & `cobald-tardis-0.8.2/tests/utilities_t/simulators_t/test_randomgauss.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/utilities_t/test_asyncbulkcall.py` & `cobald-tardis-0.8.2/tests/utilities_t/test_asyncbulkcall.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/utilities_t/test_asynccachemap.py` & `cobald-tardis-0.8.2/tests/utilities_t/test_asynccachemap.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/utilities_t/test_attributedict.py` & `cobald-tardis-0.8.2/tests/utilities_t/test_attributedict.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/utilities_t/test_pipeline.py` & `cobald-tardis-0.8.2/tests/utilities_t/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/utilities_t/test_staticmapping.py` & `cobald-tardis-0.8.2/tests/utilities_t/test_staticmapping.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.8.1/tests/utilities_t/test_utils.py` & `cobald-tardis-0.8.2/tests/utilities_t/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -161,14 +161,51 @@
                 AllocMem="0",
                 Memory="10000",
                 Features="site-124",
                 NodeHost="host-2",
             ),
         )
 
+    def test_csv_parser_cleaning(self):
+        littered_input = "\n".join(
+            [
+                "Site-Admins wish you happy holidays!",
+                "5545112||PENDING",
+                "Services will be unavailable.",
+                "5545113||PENDING",
+            ]
+        )
+
+        parsed_rows = csv_parser(
+            input_csv=littered_input,
+            fieldnames=("JobId", "Host", "State"),
+            replacements=dict(undefined=None),
+            delimiter="|",
+            skipinitialspace=True,
+            skiptrailingspace=True,
+        )
+
+        self.assertEqual(
+            next(parsed_rows),
+            dict(
+                JobId="5545112",
+                Host="",
+                State="PENDING",
+            ),
+        )
+
+        self.assertEqual(
+            next(parsed_rows),
+            dict(
+                JobId="5545113",
+                Host="",
+                State="PENDING",
+            ),
+        )
+
 
 class TestDisableLogging(TestCase):
     def test_disable_logging(self):
         with self.assertLogs(level=logging.CRITICAL):
             with disable_logging(logging.DEBUG):
                 logging.critical("Test")
```

