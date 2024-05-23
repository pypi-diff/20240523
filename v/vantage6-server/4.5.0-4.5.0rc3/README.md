# Comparing `tmp/vantage6-server-4.5.0.tar.gz` & `tmp/vantage6-server-4.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-server-4.5.0.tar", last modified: Thu May 23 15:14:50 2024, max compression
+gzip compressed data, was "vantage6-server-4.5.0rc3.tar", last modified: Wed May 22 15:04:59 2024, max compression
```

## Comparing `vantage6-server-4.5.0.tar` & `vantage6-server-4.5.0rc3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:50.158666 vantage6-server-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-05-23 15:14:50.158666 vantage6-server-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:14:50.158666 vantage6-server-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:50.146666 vantage6-server-4.5.0/tests_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/tests_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/tests_server/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)   174927 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/tests_server/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:50.146666 vantage6-server-4.5.0/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:50.150666 vantage6-server-4.5.0/vantage6/server/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/__build__
--rw-r--r--   0 runner    (1001) docker     (127)    29923 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:50.150666 vantage6-server-4.5.0/vantage6/server/_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:50.150666 vantage6-server-4.5.0/vantage6/server/_data/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/_data/dev/fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/_data/dev/node_a.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/_data/dev/node_b.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/_data/dev/server.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/_data/example_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/_data/unittest_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/_data/unittest_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/algo_store_communication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:50.150666 vantage6-server-4.5.0/vantage6/server/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:50.150666 vantage6-server-4.5.0/vantage6/server/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/controller/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/mail_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:50.154666 vantage6-server-4.5.0/vantage6/server/model/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/algorithm_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/algorithm_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/authenticatable.py
--rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:50.154666 vantage6-server-4.5.0/vantage6/server/model/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/member.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/node_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/role.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/role_rule_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/study.py
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/task_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    18115 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:50.154666 vantage6-server-4.5.0/vantage6/server/resource/
--rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22244 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/algorithm_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    32870 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:50.158666 vantage6-server-4.5.0/vantage6/server/resource/common/
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/common/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19918 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/common/input_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/common/output_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/common/swagger_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    21884 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/node.py
--rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/port.py
--rw-r--r--   0 runner    (1001) docker     (127)    20554 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/recover.py
--rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    23751 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28647 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/study.py
--rw-r--r--   0 runner    (1001) docker     (127)    40748 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:50.158666 vantage6-server-4.5.0/vantage6/server/resource/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/ui/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    19467 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/vpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/resource/websocket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15348 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-23 15:14:32.000000 vantage6-server-4.5.0/vantage6/server/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:50.158666 vantage6-server-4.5.0/vantage6_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-05-23 15:14:50.000000 vantage6-server-4.5.0/vantage6_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-23 15:14:50.000000 vantage6-server-4.5.0/vantage6_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:14:50.000000 vantage6-server-4.5.0/vantage6_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 15:14:50.000000 vantage6-server-4.5.0/vantage6_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-23 15:14:50.000000 vantage6-server-4.5.0/vantage6_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-23 15:14:50.000000 vantage6-server-4.5.0/vantage6_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.553294 vantage6-server-4.5.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-22 15:04:59.553294 vantage6-server-4.5.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:04:59.553294 vantage6-server-4.5.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.541294 vantage6-server-4.5.0rc3/tests_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/tests_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/tests_server/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)   174647 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/tests_server/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.541294 vantage6-server-4.5.0rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.545294 vantage6-server-4.5.0rc3/vantage6/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)    29923 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.545294 vantage6-server-4.5.0rc3/vantage6/server/_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.545294 vantage6-server-4.5.0rc3/vantage6/server/_data/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_data/dev/fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_data/dev/node_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_data/dev/node_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_data/dev/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_data/example_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_data/unittest_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_data/unittest_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/algo_store_communication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.545294 vantage6-server-4.5.0rc3/vantage6/server/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.545294 vantage6-server-4.5.0rc3/vantage6/server/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/controller/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/mail_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.549294 vantage6-server-4.5.0rc3/vantage6/server/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/algorithm_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/algorithm_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/authenticatable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.549294 vantage6-server-4.5.0rc3/vantage6/server/model/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/node_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/role_rule_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/study.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/task_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18115 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.553294 vantage6-server-4.5.0rc3/vantage6/server/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22084 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/algorithm_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32870 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.553294 vantage6-server-4.5.0rc3/vantage6/server/resource/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/common/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19918 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/common/input_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/common/output_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/common/swagger_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21884 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20554 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/recover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23751 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28647 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/study.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40748 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.553294 vantage6-server-4.5.0rc3/vantage6/server/resource/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/ui/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19467 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/websocket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15348 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.553294 vantage6-server-4.5.0rc3/vantage6_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-22 15:04:59.000000 vantage6-server-4.5.0rc3/vantage6_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-22 15:04:59.000000 vantage6-server-4.5.0rc3/vantage6_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:59.000000 vantage6-server-4.5.0rc3/vantage6_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 15:04:59.000000 vantage6-server-4.5.0rc3/vantage6_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-22 15:04:59.000000 vantage6-server-4.5.0rc3/vantage6_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 15:04:59.000000 vantage6-server-4.5.0rc3/vantage6_server.egg-info/top_level.txt
```

### Comparing `vantage6-server-4.5.0/PKG-INFO` & `vantage6-server-4.5.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 4.5.0
+Version: 4.5.0rc3
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 4.5.0 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 4.5.0rc3 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-server-4.5.0/setup.py` & `vantage6-server-4.5.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/tests_server/test_models.py` & `vantage6-server-4.5.0rc3/tests_server/test_models.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/tests_server/test_resources.py` & `vantage6-server-4.5.0rc3/tests_server/test_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -3547,36 +3547,31 @@
         col.save()
         algo_store = AlgorithmStore(
             name="test", url="http://test.com", collaboration=col
         )
         algo_store.save()
         rule = Rule.get_by_("collaboration", Scope.ORGANIZATION, Operation.VIEW)
         headers = self.create_user_and_login(organization=org, rules=[rule])
-
-        # list. We expect to find all stores without specified collaboration and this one
+        # list
         results = self.app.get("/api/algorithmstore", headers=headers)
-        all_stores = AlgorithmStore.get()
-        num_stores_to_find = (
-            len([store for store in all_stores if store.collaboration_id is None]) + 1
-        )
         self.assertEqual(results.status_code, HTTPStatus.OK)
-        self.assertEqual(len(results.json["data"]), num_stores_to_find)
+        self.assertEqual(len(results.json["data"]), 1)
         # single record
         results = self.app.get(f"/api/algorithmstore/{algo_store.id}", headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
         # view with another organization within the same collaboration
         headers = self.create_user_and_login(organization=org2, rules=[rule])
         results = self.app.get(
             "/api/algorithmstore",
             headers=headers,
             query_string={"collaboration_id": col.id},
         )
         self.assertEqual(results.status_code, HTTPStatus.OK)
-        self.assertEqual(len(results.json["data"]), num_stores_to_find)
+        self.assertEqual(len(results.json["data"]), 1)
         results = self.app.get(f"/api/algorithmstore/{algo_store.id}", headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
         # try to view with organization permissions but not member of
         # collaboration
         org3 = Organization()
         org3.save()
```

### Comparing `vantage6-server-4.5.0/vantage6/server/__init__.py` & `vantage6-server-4.5.0rc3/vantage6/server/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/_data/dev/fixtures.yaml` & `vantage6-server-4.5.0rc3/vantage6/server/_data/dev/fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/_data/dev/node_a.yaml` & `vantage6-server-4.5.0rc3/vantage6/server/_data/dev/node_a.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/_data/dev/node_b.yaml` & `vantage6-server-4.5.0rc3/vantage6/server/_data/dev/node_b.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/_data/dev/server.yaml` & `vantage6-server-4.5.0rc3/vantage6/server/_data/dev/server.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/_data/example_fixtures.yaml` & `vantage6-server-4.5.0rc3/vantage6/server/_data/example_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/_data/unittest_config.yaml` & `vantage6-server-4.5.0rc3/vantage6/server/_data/unittest_config.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/_data/unittest_fixtures.yaml` & `vantage6-server-4.5.0rc3/vantage6/server/_data/unittest_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/_version.py` & `vantage6-server-4.5.0rc3/vantage6/server/_version.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "__build__")) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (4, 5, 0, "final", __build__, 0)
+version_info = (4, 5, 0, "candidate", __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {"alpha": "a", "beta": "b", "candidate": "rc", "final": ""}
 version = f"{version_info[0]}.{version_info[1]}.{version_info[2]}"
 pre_release = (
     ""
     if version_info[3] == "final"
```

### Comparing `vantage6-server-4.5.0/vantage6/server/algo_store_communication.py` & `vantage6-server-4.5.0rc3/vantage6/server/algo_store_communication.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/cli/server.py` & `vantage6-server-4.5.0rc3/vantage6/server/cli/server.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/context.py` & `vantage6-server-4.5.0rc3/vantage6/server/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/controller/fixture.py` & `vantage6-server-4.5.0rc3/vantage6/server/controller/fixture.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/db.py` & `vantage6-server-4.5.0rc3/vantage6/server/db.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/default_roles.py` & `vantage6-server-4.5.0rc3/vantage6/server/default_roles.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/globals.py` & `vantage6-server-4.5.0rc3/vantage6/server/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/mail_service.py` & `vantage6-server-4.5.0rc3/vantage6/server/mail_service.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/__init__.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/algorithm_port.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/algorithm_port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/algorithm_store.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/algorithm_store.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/authenticatable.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/authenticatable.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/base.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/base.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/collaboration.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/common/utils.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/common/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/member.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/member.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/node.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/node_config.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/node_config.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/organization.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/permission.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/role.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/rule.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/run.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/run.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/study.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/study.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/task.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/task.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/task_database.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/task_database.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/model/user.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/permission.py` & `vantage6-server-4.5.0rc3/vantage6/server/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/__init__.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/algorithm_store.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/algorithm_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,20 +195,15 @@
                 )
             )
 
         # filter based on permissions
         if not self.r_col.v_glo.can():
             collab_ids = [c.id for c in auth_org.collaborations]
             if self.r_col.v_org.can():
-                q = q.filter(
-                    or_(
-                        db.AlgorithmStore.collaboration_id.in_(collab_ids),
-                        db.AlgorithmStore.collaboration_id.is_(None),
-                    )
-                )
+                q = q.filter(db.AlgorithmStore.collaboration_id.in_(collab_ids))
             else:
                 return {
                     "msg": "You lack the permission to do that!"
                 }, HTTPStatus.UNAUTHORIZED
 
         # paginate the results
         try:
```

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/collaboration.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/common/auth_helper.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/common/auth_helper.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/common/input_schema.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/common/input_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/common/output_schema.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/common/output_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/common/swagger_templates.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/common/swagger_templates.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/event.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/event.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/health.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/health.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/node.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/organization.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/port.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/recover.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/recover.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/role.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/rule.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/run.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/run.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/stats.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/stats.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/study.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/study.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/task.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/task.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/token.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/token.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/ui/column.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/ui/column.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/user.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/version.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/vpn.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/vpn.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/resource/websocket_test.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/websocket_test.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/utils.py` & `vantage6-server-4.5.0rc3/vantage6/server/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6/server/websockets.py` & `vantage6-server-4.5.0rc3/vantage6/server/websockets.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.5.0/vantage6_server.egg-info/PKG-INFO` & `vantage6-server-4.5.0rc3/vantage6_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 4.5.0
+Version: 4.5.0rc3
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 4.5.0 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 4.5.0rc3 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-server-4.5.0/vantage6_server.egg-info/SOURCES.txt` & `vantage6-server-4.5.0rc3/vantage6_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

