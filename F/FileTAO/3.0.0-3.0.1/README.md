# Comparing `tmp/FileTAO-3.0.0.tar.gz` & `tmp/FileTAO-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FileTAO-3.0.0.tar", last modified: Tue Apr 30 03:15:26 2024, max compression
+gzip compressed data, was "FileTAO-3.0.1.tar", last modified: Wed May 22 22:44:25 2024, max compression
```

## Comparing `FileTAO-3.0.0.tar` & `FileTAO-3.0.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.004255 FileTAO-3.0.0/
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:25.996255 FileTAO-3.0.0/FileTAO.egg-info/
--rw-r--r--   0 phil      (1007) phil      (1008)    67427 2024-04-30 03:15:25.000000 FileTAO-3.0.0/FileTAO.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1007) phil      (1008)     2099 2024-04-30 03:15:25.000000 FileTAO-3.0.0/FileTAO.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1007) phil      (1008)        1 2024-04-30 03:15:25.000000 FileTAO-3.0.0/FileTAO.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1007) phil      (1008)       52 2024-04-30 03:15:25.000000 FileTAO-3.0.0/FileTAO.egg-info/entry_points.txt
--rw-rw-r--   0 phil      (1007) phil      (1008)      385 2024-04-30 03:15:25.000000 FileTAO-3.0.0/FileTAO.egg-info/requires.txt
--rw-rw-r--   0 phil      (1007) phil      (1008)       22 2024-04-30 03:15:25.000000 FileTAO-3.0.0/FileTAO.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1007) phil      (1008)     1069 2024-02-20 00:19:28.000000 FileTAO-3.0.0/LICENSE
--rw-r--r--   0 phil      (1007) phil      (1008)    67427 2024-04-30 03:15:26.004255 FileTAO-3.0.0/PKG-INFO
--rw-rw-r--   0 phil      (1007) phil      (1008)    65567 2024-04-29 21:23:35.000000 FileTAO-3.0.0/README.md
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:25.996255 FileTAO-3.0.0/neurons/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-3.0.0/neurons/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    21877 2024-04-30 03:12:19.000000 FileTAO-3.0.0/neurons/api.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    44346 2024-04-28 20:19:43.000000 FileTAO-3.0.0/neurons/miner.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    16973 2024-04-28 20:19:43.000000 FileTAO-3.0.0/neurons/validator.py
--rw-rw-r--   0 phil      (1007) phil      (1008)       38 2024-04-30 03:15:26.004255 FileTAO-3.0.0/setup.cfg
--rw-rw-r--   0 phil      (1007) phil      (1008)     3962 2024-04-26 15:16:51.000000 FileTAO-3.0.0/setup.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:25.996255 FileTAO-3.0.0/storage/
--rw-rw-r--   0 phil      (1007) phil      (1008)     2364 2024-04-27 21:32:42.000000 FileTAO-3.0.0/storage/__init__.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:25.996255 FileTAO-3.0.0/storage/api/
--rw-rw-r--   0 phil      (1007) phil      (1008)      179 2024-04-28 20:19:49.000000 FileTAO-3.0.0/storage/api/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     3431 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/api/base.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     4975 2024-04-28 20:19:49.000000 FileTAO-3.0.0/storage/api/delete_api.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     2552 2024-04-28 20:19:49.000000 FileTAO-3.0.0/storage/api/example.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5923 2024-04-28 20:19:49.000000 FileTAO-3.0.0/storage/api/retrieve_api.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     6841 2024-04-29 05:21:26.000000 FileTAO-3.0.0/storage/api/store_api.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     3991 2024-03-17 16:11:41.000000 FileTAO-3.0.0/storage/api/utils.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.000255 FileTAO-3.0.0/storage/cli/
--rw-rw-r--   0 phil      (1007) phil      (1008)     1199 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/cli/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     8728 2024-04-29 21:23:35.000000 FileTAO-3.0.0/storage/cli/cli.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     1602 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/cli/default_values.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     6742 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/cli/listcommand.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     2274 2024-03-17 16:11:41.000000 FileTAO-3.0.0/storage/cli/neuroncommand.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     9067 2024-04-29 21:23:35.000000 FileTAO-3.0.0/storage/cli/retrievecommand.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     4711 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/cli/statscommand.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     9471 2024-04-29 21:23:35.000000 FileTAO-3.0.0/storage/cli/storecommand.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     2136 2024-04-28 21:03:18.000000 FileTAO-3.0.0/storage/constants.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.000255 FileTAO-3.0.0/storage/indexer/
--rw-rw-r--   0 phil      (1007) phil      (1008)     8064 2024-04-30 03:12:19.000000 FileTAO-3.0.0/storage/indexer/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     8100 2024-04-30 03:12:19.000000 FileTAO-3.0.0/storage/indexer/endpoint.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    10255 2024-04-29 16:40:25.000000 FileTAO-3.0.0/storage/indexer/redis.py
--rw-rw-r--   0 phil      (1007) phil      (1008)      675 2024-04-27 21:32:42.000000 FileTAO-3.0.0/storage/indexer/sqlite.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.000255 FileTAO-3.0.0/storage/miner/
--rw-rw-r--   0 phil      (1007) phil      (1008)     1240 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/miner/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    10763 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/miner/config.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    15278 2024-02-22 21:12:16.000000 FileTAO-3.0.0/storage/miner/database.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     4204 2024-04-28 17:54:08.000000 FileTAO-3.0.0/storage/miner/run.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     4619 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/miner/set_weights.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    14477 2024-03-17 16:50:11.000000 FileTAO-3.0.0/storage/miner/utils.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.000255 FileTAO-3.0.0/storage/plot/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-03-17 16:11:41.000000 FileTAO-3.0.0/storage/plot/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     6672 2024-03-17 16:11:41.000000 FileTAO-3.0.0/storage/plot/utils.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     7921 2024-04-28 20:19:49.000000 FileTAO-3.0.0/storage/protocol.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.000255 FileTAO-3.0.0/storage/shared/
--rw-rw-r--   0 phil      (1007) phil      (1008)     1200 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/shared/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5413 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/shared/checks.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     7290 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/shared/ecc.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    17746 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/shared/merkle.py
--rw-rw-r--   0 phil      (1007) phil      (1008)      923 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/shared/subtensor.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     7992 2024-04-28 20:19:49.000000 FileTAO-3.0.0/storage/shared/utils.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     3436 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/shared/weights.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.004255 FileTAO-3.0.0/storage/validator/
--rw-rw-r--   0 phil      (1007) phil      (1008)     1514 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    14756 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/bonding.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    10538 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/challenge.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5864 2024-02-22 21:12:16.000000 FileTAO-3.0.0/storage/validator/cid.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    12139 2024-04-30 03:12:19.000000 FileTAO-3.0.0/storage/validator/config.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    43538 2024-04-28 20:19:49.000000 FileTAO-3.0.0/storage/validator/database.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     3113 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/dendrite.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     3211 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/validator/distribute.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    15435 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/validator/encryption.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     3046 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/validator/event.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     6223 2024-03-17 16:11:41.000000 FileTAO-3.0.0/storage/validator/forward.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     9417 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/network.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5072 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/validator/rebalance.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    16215 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/retrieve.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    12356 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/reward.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     8798 2024-03-17 16:11:41.000000 FileTAO-3.0.0/storage/validator/state.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    23047 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/store.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    32272 2024-04-28 17:54:08.000000 FileTAO-3.0.0/storage/validator/utils.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     8315 2024-02-20 00:19:28.000000 FileTAO-3.0.0/storage/validator/verify.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     6961 2024-04-26 15:16:51.000000 FileTAO-3.0.0/storage/validator/weights.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.004255 FileTAO-3.0.0/tests/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/__init__.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.004255 FileTAO-3.0.0/tests/integration/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/integration/__init__.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.004255 FileTAO-3.0.0/tests/unit/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/unit/__init__.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.004255 FileTAO-3.0.0/tests/unit/cli/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/unit/cli/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)      407 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/unit/cli/test_cli.py
--rw-rw-r--   0 phil      (1007) phil      (1008)      442 2024-03-17 16:11:41.000000 FileTAO-3.0.0/tests/unit/cli/test_neuroncommand.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-04-30 03:15:26.004255 FileTAO-3.0.0/tests/unit/validator/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/unit/validator/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)      863 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/unit/validator/test_challenge.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     1529 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/unit/validator/test_encryption.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     1118 2024-02-20 00:19:28.000000 FileTAO-3.0.0/tests/unit/validator/test_state.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.412089 FileTAO-3.0.1/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.412089 FileTAO-3.0.1/FileTAO.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    67421 2024-05-22 22:44:25.000000 FileTAO-3.0.1/FileTAO.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2099 2024-05-22 22:44:25.000000 FileTAO-3.0.1/FileTAO.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 22:44:25.000000 FileTAO-3.0.1/FileTAO.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2024-05-22 22:44:25.000000 FileTAO-3.0.1/FileTAO.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      379 2024-05-22 22:44:25.000000 FileTAO-3.0.1/FileTAO.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-05-22 22:44:25.000000 FileTAO-3.0.1/FileTAO.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1069 2024-03-31 17:54:51.000000 FileTAO-3.0.1/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    67421 2024-05-22 22:44:25.412089 FileTAO-3.0.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    65567 2024-05-22 14:48:44.000000 FileTAO-3.0.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.404089 FileTAO-3.0.1/neurons/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.1/neurons/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22328 2024-05-22 16:09:56.000000 FileTAO-3.0.1/neurons/api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45035 2024-05-22 15:11:25.000000 FileTAO-3.0.1/neurons/miner.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16973 2024-05-15 15:46:07.000000 FileTAO-3.0.1/neurons/validator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 22:44:25.412089 FileTAO-3.0.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3962 2024-05-15 15:46:07.000000 FileTAO-3.0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.404089 FileTAO-3.0.1/storage/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2364 2024-05-22 15:11:25.000000 FileTAO-3.0.1/storage/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.404089 FileTAO-3.0.1/storage/api/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      179 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/api/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3431 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/api/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4975 2024-05-22 14:50:05.000000 FileTAO-3.0.1/storage/api/delete_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2552 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/api/example.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5923 2024-05-22 15:12:18.000000 FileTAO-3.0.1/storage/api/retrieve_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6841 2024-05-22 14:50:25.000000 FileTAO-3.0.1/storage/api/store_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3991 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/api/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.404089 FileTAO-3.0.1/storage/cli/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1199 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/cli/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8728 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/cli/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1602 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/cli/default_values.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6742 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/cli/listcommand.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2274 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/cli/neuroncommand.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9067 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/cli/retrievecommand.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4711 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/cli/statscommand.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9471 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/cli/storecommand.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2136 2024-05-22 16:09:56.000000 FileTAO-3.0.1/storage/constants.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/storage/indexer/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8064 2024-05-22 15:03:32.000000 FileTAO-3.0.1/storage/indexer/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8056 2024-05-22 16:36:13.000000 FileTAO-3.0.1/storage/indexer/endpoint.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10255 2024-05-22 14:58:41.000000 FileTAO-3.0.1/storage/indexer/redis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/indexer/sqlite.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/storage/miner/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1240 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/miner/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10763 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/miner/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15278 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/miner/database.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4204 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/miner/run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4619 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/miner/set_weights.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14477 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/miner/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/storage/plot/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/plot/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6672 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/plot/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7921 2024-05-22 16:09:56.000000 FileTAO-3.0.1/storage/protocol.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/storage/shared/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1200 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/shared/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5413 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/shared/checks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7290 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/shared/ecc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17746 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/shared/merkle.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      923 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/shared/subtensor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7992 2024-05-22 14:53:20.000000 FileTAO-3.0.1/storage/shared/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3436 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/shared/weights.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/storage/validator/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1514 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14756 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/bonding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10538 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/challenge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5864 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/cid.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12139 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/validator/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43538 2024-05-22 15:13:14.000000 FileTAO-3.0.1/storage/validator/database.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3113 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/dendrite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/distribute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15435 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/encryption.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3046 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/event.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6223 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/forward.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9417 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/network.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5072 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/rebalance.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16215 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/retrieve.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12356 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/reward.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8798 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/state.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23047 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/store.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32272 2024-05-22 14:46:38.000000 FileTAO-3.0.1/storage/validator/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8315 2024-03-31 17:54:51.000000 FileTAO-3.0.1/storage/validator/verify.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6961 2024-05-15 15:46:07.000000 FileTAO-3.0.1/storage/validator/weights.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/tests/integration/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/integration/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.408089 FileTAO-3.0.1/tests/unit/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.412089 FileTAO-3.0.1/tests/unit/cli/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/cli/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      407 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/cli/test_cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      442 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/cli/test_neuroncommand.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 22:44:25.412089 FileTAO-3.0.1/tests/unit/validator/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/validator/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      863 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/validator/test_challenge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1529 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/validator/test_encryption.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1118 2024-03-31 17:54:51.000000 FileTAO-3.0.1/tests/unit/validator/test_state.py
```

### Comparing `FileTAO-3.0.0/FileTAO.egg-info/PKG-INFO` & `FileTAO-3.0.1/FileTAO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FileTAO
-Version: 3.0.0
+Version: 3.0.1
 Summary: Philanthropic storage for the masses. (FileTAO)
 Home-page: https://github.com/ifrit98/storage-subnet
 Author: philanthrope
 Author-email: ifrit98@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -21,25 +21,25 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=1.13.0
 Requires-Dist: bcrypt==3.2.0
-Requires-Dist: bittensor==6.11.0
+Requires-Dist: bittensor==6.12.2
 Requires-Dist: redis==5.0.1
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: pyinstrument==4.6.1
 Requires-Dist: wandb==0.16.0
 Requires-Dist: morphys==1.0
 Requires-Dist: py-multibase==1.0.3
 Requires-Dist: py-multicodec==0.2.1
 Requires-Dist: py-multihash==2.0.1
 Requires-Dist: ipfs-cid==1.0.0
-Requires-Dist: python-jose==3.3.0
+Requires-Dist: pyjwt>=2.8.0
 Requires-Dist: passlib==1.7.4
 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: loguru==0.7.0
 Requires-Dist: pandas==2.2.0
 Provides-Extra: dev
 Requires-Dist: pytest==7.4.3; extra == "dev"
```

### Comparing `FileTAO-3.0.0/FileTAO.egg-info/SOURCES.txt` & `FileTAO-3.0.1/FileTAO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/LICENSE` & `FileTAO-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/PKG-INFO` & `FileTAO-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FileTAO
-Version: 3.0.0
+Version: 3.0.1
 Summary: Philanthropic storage for the masses. (FileTAO)
 Home-page: https://github.com/ifrit98/storage-subnet
 Author: philanthrope
 Author-email: ifrit98@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -21,25 +21,25 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=1.13.0
 Requires-Dist: bcrypt==3.2.0
-Requires-Dist: bittensor==6.11.0
+Requires-Dist: bittensor==6.12.2
 Requires-Dist: redis==5.0.1
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: pyinstrument==4.6.1
 Requires-Dist: wandb==0.16.0
 Requires-Dist: morphys==1.0
 Requires-Dist: py-multibase==1.0.3
 Requires-Dist: py-multicodec==0.2.1
 Requires-Dist: py-multihash==2.0.1
 Requires-Dist: ipfs-cid==1.0.0
-Requires-Dist: python-jose==3.3.0
+Requires-Dist: pyjwt>=2.8.0
 Requires-Dist: passlib==1.7.4
 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: loguru==0.7.0
 Requires-Dist: pandas==2.2.0
 Provides-Extra: dev
 Requires-Dist: pytest==7.4.3; extra == "dev"
```

### Comparing `FileTAO-3.0.0/README.md` & `FileTAO-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/neurons/api.py` & `FileTAO-3.0.1/neurons/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,29 +271,34 @@
         return synapse
 
     async def store_blacklist(
         self, synapse: protocol.StoreUser
     ) -> typing.Tuple[bool, str]:
         # If debug mode, whitelist everything (NOT RECOMMENDED)
 
-        if self.config.api.open_access:
-            return False, "Open access: WARNING all whitelisted"
+        try:
 
-        if synapse.dendrite.hotkey in self.config.api.blacklisted_hotkeys:
-            return True, f"Hotkey {synapse.dendrite.hotkey} blacklisted."
+            if self.config.api.open_access:
+                return False, "Open access: WARNING all whitelisted"
 
-        # If explicitly whitelisted hotkey, allow.
-        if synapse.dendrite.hotkey in self.config.api.whitelisted_hotkeys:
-            return False, f"Hotkey {synapse.dendrite.hotkey} whitelisted."
-
-        # Otherwise, reject.
-        return (
-            True,
-            f"Hotkey {synapse.dendrite.hotkey} not whitelisted or in top n% stake.",
-        )
+            if synapse.dendrite.hotkey in self.config.api.blacklisted_hotkeys:
+                return True, f"Hotkey {synapse.dendrite.hotkey} blacklisted."
+
+            # If explicitly whitelisted hotkey, allow.
+            if synapse.dendrite.hotkey in self.config.api.whitelisted_hotkeys:
+                return False, f"Hotkey {synapse.dendrite.hotkey} whitelisted."
+
+            # Otherwise, reject.
+            return (
+                True,
+                f"Hotkey {synapse.dendrite.hotkey} not whitelisted or in top n% stake.",
+            )
+
+        except Exception as e:
+                 return True, f"Unhandled exception api store blacklist_fn [{e}], assuming True"
 
     async def store_priority(self, synapse: protocol.StoreUser) -> float:
         if self.config.api.open_access or synapse.dendrite.hotkey in self.config.api.whitelisted_hotkeys:
             return 1.0
 
         caller_uid = self.metagraph.hotkeys.index(
             synapse.dendrite.hotkey
@@ -357,27 +362,31 @@
             else user_encryption_payload
         )
         return synapse
 
     async def retrieve_blacklist(
         self, synapse: protocol.RetrieveUser
     ) -> typing.Tuple[bool, str]:
-        # If debug mode, whitelist everything (NOT RECOMMENDED)
-        if self.config.api.open_access:
-            return False, "Open access: WARNING all whitelisted"
 
-        # If explicitly whitelisted hotkey, allow.
-        if synapse.dendrite.hotkey in self.config.api.whitelisted_hotkeys:
-            return False, f"Hotkey {synapse.dendrite.hotkey} whitelisted."
-
-        # Otherwise, reject.
-        return (
-            True,
-            f"Hotkey {synapse.dendrite.hotkey} not whitelisted or in top n% stake.",
-        )
+        try:
+            if self.config.api.open_access:
+                return False, "Open access: WARNING all whitelisted"
+
+            # If explicitly whitelisted hotkey, allow.
+            if synapse.dendrite.hotkey in self.config.api.whitelisted_hotkeys:
+                return False, f"Hotkey {synapse.dendrite.hotkey} whitelisted."
+
+            # Otherwise, reject.
+            return (
+                True,
+                f"Hotkey {synapse.dendrite.hotkey} not whitelisted or in top n% stake.",
+            )
+
+        except Exception as e:
+                 return True, f"Unhandled exception checking api retrieve blacklist_fn [{e}], assuming True"
 
     async def retrieve_priority(self, synapse: protocol.RetrieveUser) -> float:
         if self.config.api.open_access or synapse.dendrite.hotkey in self.config.api.whitelisted_hotkeys:
             return 1.0
 
         caller_uid = self.metagraph.hotkeys.index(
             synapse.dendrite.hotkey
@@ -425,27 +434,31 @@
         synapse.deleted = True
 
         return synapse
 
     async def delete_blacklist(
         self, synapse: protocol.DeleteUser
     ) -> typing.Tuple[bool, str]:
-        # If debug mode, whitelist everything (NOT RECOMMENDED)
-        if self.config.api.open_access:
-            return False, "Open access: WARNING all whitelisted"
 
-        # If explicitly whitelisted hotkey, allow.
-        if synapse.dendrite.hotkey in self.config.api.whitelisted_hotkeys:
-            return False, f"Hotkey {synapse.dendrite.hotkey} whitelisted."
-
-        # Otherwise, reject.
-        return (
-            True,
-            f"Hotkey {synapse.dendrite.hotkey} not whitelisted or in top n% stake.",
-        )
+        try:
+            if self.config.api.open_access:
+                return False, "Open access: WARNING all whitelisted"
+
+            # If explicitly whitelisted hotkey, allow.
+            if synapse.dendrite.hotkey in self.config.api.whitelisted_hotkeys:
+                return False, f"Hotkey {synapse.dendrite.hotkey} whitelisted."
+
+            # Otherwise, reject.
+            return (
+                True,
+                f"Hotkey {synapse.dendrite.hotkey} not whitelisted or in top n% stake.",
+            )
+
+        except Exception as e:
+                 return True, f"Unhandled exception checking api delete blacklist_fn [{e}], assuming True"
 
     async def delete_priority(self, synapse: protocol.DeleteUser) -> float:
         if self.config.api.open_access or synapse.dendrite.hotkey in self.config.api.whitelisted_hotkeys:
             return 1.0
 
         caller_uid = self.metagraph.hotkeys.index(
             synapse.dendrite.hotkey
```

### Comparing `FileTAO-3.0.0/neurons/miner.py` & `FileTAO-3.0.1/neurons/miner.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,38 +349,42 @@
         entities can participate in communication or transactions.
         """
         try:
             self.request_log = log_request(synapse, self.request_log)
         except Exception as e:
             bt.logging.error(f"Error logging request: {e}")
 
-        caller = synapse.dendrite.hotkey
-        if caller in self.config.blacklist.blacklist_hotkeys:
-            return True, f"Hotkey {caller} in blacklist."
-        elif caller in self.config.blacklist.whitelist_hotkeys:
-            return False, f"Hotkey {caller} in whitelist."
-
-        if caller not in self.rate_limiters:
-            self.rate_limiters[caller] = RateLimiter(
-                self.config.miner.max_requests_per_window,
-                self.config.miner.rate_limit_window,
-            )
-
-        if not self.rate_limiters[caller].is_allowed(caller):
-            window = self.config.miner.max_requests_per_window
-            blocks = self.config.miner.rate_limit_window
-            reason = f"Caller {caller} rate limited. Exceeded {window} requests in {blocks} blocks."
-            return True, reason
-
-        if caller not in self.metagraph.hotkeys:
-            bt.logging.trace(f"Blacklisting unrecognized hotkey {caller}")
-            return True, "Unrecognized hotkey"
+        try:
+            caller = synapse.dendrite.hotkey
+            if caller in self.config.blacklist.blacklist_hotkeys:
+                return True, f"Hotkey {caller} in blacklist."
+            elif caller in self.config.blacklist.whitelist_hotkeys:
+                return False, f"Hotkey {caller} in whitelist."
+
+            if caller not in self.rate_limiters:
+                self.rate_limiters[caller] = RateLimiter(
+                    self.config.miner.max_requests_per_window,
+                    self.config.miner.rate_limit_window,
+                )
+
+            if not self.rate_limiters[caller].is_allowed(caller):
+                window = self.config.miner.max_requests_per_window
+                blocks = self.config.miner.rate_limit_window
+                reason = f"Caller {caller} rate limited. Exceeded {window} requests in {blocks} blocks."
+                return True, reason
+
+            if caller not in self.metagraph.hotkeys:
+                bt.logging.trace(f"Blacklisting unrecognized hotkey {caller}")
+                return True, "Unrecognized hotkey"
+
+            bt.logging.trace(f"Not Blacklisting recognized hotkey {caller}")
+            return False, "Hotkey recognized!"
 
-        bt.logging.trace(f"Not Blacklisting recognized hotkey {caller}")
-        return False, "Hotkey recognized!"
+        except Exception as e:
+                 return True, f"Unhandled exception checking store blacklist_fn [{e}], assuming True"
 
     def store_priority_fn(self, synapse: storage.protocol.Store) -> float:
         """
         Assigns a priority to a given synapse based on the stake of the calling entity
         in the metagraph. This function is crucial for prioritizing network requests
         and ensuring that higher-stake entities are given precedence in processing.
 
@@ -436,38 +440,43 @@
         entities can participate in communication or transactions.
         """
         try:
             self.request_log = log_request(synapse, self.request_log)
         except Exception as e:
             bt.logging.error(f"Error logging request: {e}")
 
-        caller = synapse.dendrite.hotkey
-        if caller in self.config.blacklist.blacklist_hotkeys:
-            return True, f"Hotkey {caller} in blacklist."
-        elif caller in self.config.blacklist.whitelist_hotkeys:
-            return False, f"Hotkey {caller} in whitelist."
-
-        if caller not in self.rate_limiters:
-            self.rate_limiters[caller] = RateLimiter(
-                self.config.miner.max_requests_per_window,
-                self.config.miner.rate_limit_window,
-            )
-
-        if not self.rate_limiters[caller].is_allowed(caller):
-            window = self.config.miner.max_requests_per_window
-            blocks = self.config.miner.rate_limit_window
-            reason = f"Caller {caller} rate limited. Exceeded {window} requests in {blocks} blocks."
-            return True, reason
-
-        if caller not in self.metagraph.hotkeys:
-            bt.logging.trace(f"Blacklisting unrecognized hotkey {caller}")
-            return True, "Unrecognized hotkey"
+        try:
+            caller = synapse.dendrite.hotkey
+            if caller in self.config.blacklist.blacklist_hotkeys:
+                return True, f"Hotkey {caller} in blacklist."
+            elif caller in self.config.blacklist.whitelist_hotkeys:
+                return False, f"Hotkey {caller} in whitelist."
+
+            if caller not in self.rate_limiters:
+                self.rate_limiters[caller] = RateLimiter(
+                    self.config.miner.max_requests_per_window,
+                    self.config.miner.rate_limit_window,
+                )
+
+            if not self.rate_limiters[caller].is_allowed(caller):
+                window = self.config.miner.max_requests_per_window
+                blocks = self.config.miner.rate_limit_window
+                reason = f"Caller {caller} rate limited. Exceeded {window} requests in {blocks} blocks."
+                return True, reason
+
+            if caller not in self.metagraph.hotkeys:
+                bt.logging.trace(f"Blacklisting unrecognized hotkey {caller}")
+                return True, "Unrecognized hotkey"
+
+            bt.logging.trace(f"Not Blacklisting recognized hotkey {caller}")
+            return False, "Hotkey recognized!"
+
+        except Exception as e:
+                 return True, f"Unhandled exception checking challenge blacklist_fn [{e}], assuming True"
 
-        bt.logging.trace(f"Not Blacklisting recognized hotkey {caller}")
-        return False, "Hotkey recognized!"
 
     def challenge_priority_fn(self, synapse: storage.protocol.Challenge) -> float:
         """
         Assigns a priority to a given synapse based on the stake of the calling entity
         in the metagraph. This function is crucial for prioritizing network requests
         and ensuring that higher-stake entities are given precedence in processing.
 
@@ -523,38 +532,42 @@
         entities can participate in communication or transactions.
         """
         try:
             self.request_log = log_request(synapse, self.request_log)
         except Exception as e:
             bt.logging.error(f"Error logging request: {e}")
 
-        caller = synapse.dendrite.hotkey
-        if caller in self.config.blacklist.blacklist_hotkeys:
-            return True, f"Hotkey {caller} in blacklist."
-        elif caller in self.config.blacklist.whitelist_hotkeys:
-            return False, f"Hotkey {caller} in whitelist."
-
-        if caller not in self.rate_limiters:
-            self.rate_limiters[caller] = RateLimiter(
-                self.config.miner.max_requests_per_window,
-                self.config.miner.rate_limit_window,
-            )
-
-        if not self.rate_limiters[caller].is_allowed(caller):
-            window = self.config.miner.max_requests_per_window
-            blocks = self.config.miner.rate_limit_window
-            reason = f"Caller {caller} rate limited. Exceeded {window} requests in {blocks} blocks."
-            return True, reason
-
-        if caller not in self.metagraph.hotkeys:
-            bt.logging.trace(f"Blacklisting unrecognized hotkey {caller}")
-            return True, "Unrecognized hotkey"
+        try:
+            caller = synapse.dendrite.hotkey
+            if caller in self.config.blacklist.blacklist_hotkeys:
+                return True, f"Hotkey {caller} in blacklist."
+            elif caller in self.config.blacklist.whitelist_hotkeys:
+                return False, f"Hotkey {caller} in whitelist."
+
+            if caller not in self.rate_limiters:
+                self.rate_limiters[caller] = RateLimiter(
+                    self.config.miner.max_requests_per_window,
+                    self.config.miner.rate_limit_window,
+                )
+
+            if not self.rate_limiters[caller].is_allowed(caller):
+                window = self.config.miner.max_requests_per_window
+                blocks = self.config.miner.rate_limit_window
+                reason = f"Caller {caller} rate limited. Exceeded {window} requests in {blocks} blocks."
+                return True, reason
+
+            if caller not in self.metagraph.hotkeys:
+                bt.logging.trace(f"Blacklisting unrecognized hotkey {caller}")
+                return True, "Unrecognized hotkey"
 
-        bt.logging.trace(f"Not Blacklisting recognized hotkey {caller}")
-        return False, "Hotkey recognized!"
+            bt.logging.trace(f"Not Blacklisting recognized hotkey {caller}")
+            return False, "Hotkey recognized!"
+
+        except Exception as e:
+                 return True, f"Unhandled exception checking retrieve blacklist_fn [{e}], assuming True"
 
     def retrieve_priority_fn(self, synapse: storage.protocol.Retrieve) -> float:
         """
         Assigns a priority to a given synapse based on the stake of the calling entity
         in the metagraph. This function is crucial for prioritizing network requests
         and ensuring that higher-stake entities are given precedence in processing.
```

### Comparing `FileTAO-3.0.0/neurons/validator.py` & `FileTAO-3.0.1/neurons/validator.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/setup.py` & `FileTAO-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/__init__.py` & `FileTAO-3.0.1/storage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         return (self.major, self.minor, self.patch) < (
             other.major,
             other.minor,
             other.patch,
         )
 
 
-__version__ = "3.0.0"
+__version__ = "3.0.1"
 version = StorageVersion.from_string(__version__)
 __spec_version__ = version.to_spec_version()
 
 # Import all submodules.
 from . import protocol
 from . import validator
 from . import miner
```

### Comparing `FileTAO-3.0.0/storage/api/base.py` & `FileTAO-3.0.1/storage/api/base.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/api/delete_api.py` & `FileTAO-3.0.1/storage/api/delete_api.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/api/example.py` & `FileTAO-3.0.1/storage/api/example.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/api/retrieve_api.py` & `FileTAO-3.0.1/storage/api/retrieve_api.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/api/store_api.py` & `FileTAO-3.0.1/storage/api/store_api.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/api/utils.py` & `FileTAO-3.0.1/storage/api/utils.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/cli/__init__.py` & `FileTAO-3.0.1/storage/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/cli/cli.py` & `FileTAO-3.0.1/storage/cli/cli.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/cli/default_values.py` & `FileTAO-3.0.1/storage/cli/default_values.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/cli/listcommand.py` & `FileTAO-3.0.1/storage/cli/listcommand.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/cli/neuroncommand.py` & `FileTAO-3.0.1/storage/cli/neuroncommand.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/cli/retrievecommand.py` & `FileTAO-3.0.1/storage/cli/retrievecommand.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/cli/statscommand.py` & `FileTAO-3.0.1/storage/cli/statscommand.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/cli/storecommand.py` & `FileTAO-3.0.1/storage/cli/storecommand.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/constants.py` & `FileTAO-3.0.1/storage/constants.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/indexer/__init__.py` & `FileTAO-3.0.1/storage/indexer/__init__.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/indexer/endpoint.py` & `FileTAO-3.0.1/storage/indexer/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import pandas as pd
 import datetime
 import time
 import threading
 import uvicorn
 
-from typing import List, Dict, Union
+from typing import List, Union
 from time import time
 from pydantic import BaseModel
 from fastapi import FastAPI
-from redis import asyncio as aioredis
 
 from .sqlite import query
 
 app = FastAPI()
 
 class MinerStatItem(BaseModel):
     TIMESTAMP: str
```

### Comparing `FileTAO-3.0.0/storage/indexer/redis.py` & `FileTAO-3.0.1/storage/indexer/redis.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/indexer/sqlite.py` & `FileTAO-3.0.1/storage/indexer/sqlite.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/miner/__init__.py` & `FileTAO-3.0.1/storage/miner/__init__.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/miner/config.py` & `FileTAO-3.0.1/storage/miner/config.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/miner/database.py` & `FileTAO-3.0.1/storage/miner/database.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/miner/run.py` & `FileTAO-3.0.1/storage/miner/run.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/miner/set_weights.py` & `FileTAO-3.0.1/storage/miner/set_weights.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/miner/utils.py` & `FileTAO-3.0.1/storage/miner/utils.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/plot/utils.py` & `FileTAO-3.0.1/storage/plot/utils.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/protocol.py` & `FileTAO-3.0.1/storage/protocol.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/shared/__init__.py` & `FileTAO-3.0.1/storage/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/shared/checks.py` & `FileTAO-3.0.1/storage/shared/checks.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/shared/ecc.py` & `FileTAO-3.0.1/storage/shared/ecc.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/shared/merkle.py` & `FileTAO-3.0.1/storage/shared/merkle.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/shared/subtensor.py` & `FileTAO-3.0.1/storage/shared/subtensor.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/shared/utils.py` & `FileTAO-3.0.1/storage/shared/utils.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/shared/weights.py` & `FileTAO-3.0.1/storage/shared/weights.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/__init__.py` & `FileTAO-3.0.1/storage/validator/__init__.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/bonding.py` & `FileTAO-3.0.1/storage/validator/bonding.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/challenge.py` & `FileTAO-3.0.1/storage/validator/challenge.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/cid.py` & `FileTAO-3.0.1/storage/validator/cid.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/config.py` & `FileTAO-3.0.1/storage/validator/config.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/database.py` & `FileTAO-3.0.1/storage/validator/database.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/dendrite.py` & `FileTAO-3.0.1/storage/validator/dendrite.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/distribute.py` & `FileTAO-3.0.1/storage/validator/distribute.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/encryption.py` & `FileTAO-3.0.1/storage/validator/encryption.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/event.py` & `FileTAO-3.0.1/storage/validator/event.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/forward.py` & `FileTAO-3.0.1/storage/validator/forward.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/network.py` & `FileTAO-3.0.1/storage/validator/network.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/rebalance.py` & `FileTAO-3.0.1/storage/validator/rebalance.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/retrieve.py` & `FileTAO-3.0.1/storage/validator/retrieve.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/reward.py` & `FileTAO-3.0.1/storage/validator/reward.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/state.py` & `FileTAO-3.0.1/storage/validator/state.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/store.py` & `FileTAO-3.0.1/storage/validator/store.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/utils.py` & `FileTAO-3.0.1/storage/validator/utils.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/verify.py` & `FileTAO-3.0.1/storage/validator/verify.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/storage/validator/weights.py` & `FileTAO-3.0.1/storage/validator/weights.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/tests/unit/validator/test_challenge.py` & `FileTAO-3.0.1/tests/unit/validator/test_challenge.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/tests/unit/validator/test_encryption.py` & `FileTAO-3.0.1/tests/unit/validator/test_encryption.py`

 * *Files identical despite different names*

### Comparing `FileTAO-3.0.0/tests/unit/validator/test_state.py` & `FileTAO-3.0.1/tests/unit/validator/test_state.py`

 * *Files identical despite different names*

