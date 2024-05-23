# Comparing `tmp/gink-0.20240521.1716315298.tar.gz` & `tmp/gink-0.20240523.1716450705.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gink-0.20240521.1716315298.tar", last modified: Tue May 21 18:15:01 2024, max compression
+gzip compressed data, was "gink-0.20240523.1716450705.tar", last modified: Thu May 23 07:51:50 2024, max compression
```

## Comparing `gink-0.20240521.1716315298.tar` & `gink-0.20240523.1716450705.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:15:01.871978 gink-0.20240521.1716315298/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-21 18:15:01.871978 gink-0.20240521.1716315298/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:15:01.855977 gink-0.20240521.1716315298/gink/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6055 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:15:01.859978 gink-0.20240521.1716315298/gink/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/behavior_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/change_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/claim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/clearance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/container_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/entry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/header_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/key_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/log_file_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/movement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/muid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/pair_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/sync_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/gink/builders/value_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:15:01.867977 gink-0.20240521.1716315298/gink/impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/abstract_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/addressable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/braid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/bundle_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/bundle_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/bundle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/container.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14405 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    57325 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/lmdb_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/log_backed_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/looping.py
--rw-r--r--   0 runner    (1001) docker     (127)    23274 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/selectable_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/websocket_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/wsgi_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/impl/wsgi_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:15:01.871978 gink-0.20240521.1716315298/gink/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_braid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_change_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_code_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_demo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_logbackedstore.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_websocket_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-21 18:14:56.000000 gink-0.20240521.1716315298/gink/tests/test_wsgi_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:15:01.871978 gink-0.20240521.1716315298/gink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-21 18:15:01.000000 gink-0.20240521.1716315298/gink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-21 18:15:01.000000 gink-0.20240521.1716315298/gink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:15:01.000000 gink-0.20240521.1716315298/gink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-21 18:15:01.000000 gink-0.20240521.1716315298/gink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 18:15:01.000000 gink-0.20240521.1716315298/gink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 18:15:01.871978 gink-0.20240521.1716315298/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-21 18:14:58.000000 gink-0.20240521.1716315298/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:50.630248 gink-0.20240523.1716450705/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-23 07:51:50.630248 gink-0.20240523.1716450705/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:50.614248 gink-0.20240523.1716450705/gink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7062 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:50.618248 gink-0.20240523.1716450705/gink/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/behavior_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/change_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/claim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/clearance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/container_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/entry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/header_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/key_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/log_file_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/movement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/muid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/pair_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/sync_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/gink/builders/value_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:50.622248 gink-0.20240523.1716450705/gink/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/abstract_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/addressable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/braid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/bundle_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/bundle_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/bundle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/container.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14405 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57325 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/lmdb_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/log_backed_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/looping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23274 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/selectable_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/wsgi_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/impl/wsgi_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:50.630248 gink-0.20240523.1716450705/gink/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_braid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_change_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_code_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_logbackedstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-23 07:51:43.000000 gink-0.20240523.1716450705/gink/tests/test_wsgi_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:51:50.630248 gink-0.20240523.1716450705/gink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-23 07:51:50.000000 gink-0.20240523.1716450705/gink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-23 07:51:50.000000 gink-0.20240523.1716450705/gink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:51:50.000000 gink-0.20240523.1716450705/gink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-23 07:51:50.000000 gink-0.20240523.1716450705/gink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 07:51:50.000000 gink-0.20240523.1716450705/gink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 07:51:50.630248 gink-0.20240523.1716450705/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-23 07:51:45.000000 gink-0.20240523.1716450705/setup.py
```

### Comparing `gink-0.20240521.1716315298/LICENSE` & `gink-0.20240523.1716450705/LICENSE`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/PKG-INFO` & `gink-0.20240523.1716450705/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240521.1716315298
+Version: 0.20240523.1716450705
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240521.1716315298/README.md` & `gink-0.20240523.1716450705/README.md`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/__init__.py` & `gink-0.20240523.1716450705/gink/__init__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/__main__.py` & `gink-0.20240523.1716450705/gink/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 #!/usr/bin/env python3
 """ command line interface for Gink """
 from logging import basicConfig, getLogger
 from sys import exit, stdin
 from re import fullmatch
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
+from typing import Optional, Tuple, Union
+from importlib import import_module
 
 from . import *
 from .impl.builders import BundleBuilder
 from .impl.selectable_console import SelectableConsole
 from .impl.utilities import get_identity
 from .impl.looping import loop
+from .impl.wsgi_listener import WsgiListener
 
 parser: ArgumentParser = ArgumentParser(allow_abbrev=False)
 parser.add_argument("db_path", nargs="?", help="path to a database; created if doesn't exist")
 parser.add_argument("--verbosity", "-v", default="INFO", help="the log level to use, e.g. INFO or DEBUG")
 parser.add_argument("--format", default="lmdb", help="storage file format", choices=["lmdb", "binlog"])
 parser.add_argument("--set", help="set key/value in directory (default root) reading value from stdin")
 parser.add_argument("--get", help="get a value in the database (default root) and print to stdout")
@@ -33,14 +36,16 @@
 parser.add_argument("--show_bundles", action="store_true")
 parser.add_argument("--repr", action="store_true", help="show repr of stored value when using --get")
 parser.add_argument("--line_mode", action="store_true", help="read lines of input from stdin")
 parser.add_argument("--interactive", action="store_true", help="force interactive mode")
 parser.add_argument("--heartbeat_to", type=Path, help="write on console refresh (for debugging)")
 parser.add_argument("--identity", help="explicitly set identity to be associated with changes")
 parser.add_argument("--starts", help="include starting bundles when showing log", action="store_true")
+parser.add_argument("--wsgi", help="serve module.function via wsgi")
+parser.add_argument("--wsgi_listen_on", help="ip:port or port to listen on (defaults to *:8081)")
 args: Namespace = parser.parse_args()
 if args.show_arguments:
     print(args)
     exit(0)
 basicConfig(format="\r[%(asctime)s.%(msecs)03d %(name)s:%(levelname)s] %(message)s",
             level=args.verbosity, datefmt='%I:%M:%S')
 logger = getLogger()
@@ -126,35 +131,50 @@
     exit(0)
 
 if args.log:
     database.show_log(args.log, include_starts=args.starts)
     database.close()
     exit(0)
 
-if args.listen_on:
-    ip_addr = "*"
-    port = "8080"
-    if args.listen_on is True:
+def parse_listen_on(listen_on: Union[str, None, bool], ip_addr = "*", port = "8080") -> Tuple[str, str]:
+    if listen_on is True or listen_on is None:
         pass
-    elif ":" in args.listen_on:
-        ip_addr, port = args.listen_on.split(":")
-    elif fullmatch(r"\d+", args.listen_on):
-        port = args.listen_on
+    elif ":" in listen_on:
+        ip_addr, port = listen_on.split(":")
+    elif fullmatch(r"\d+", listen_on):
+        port = listen_on
     else:
-        ip_addr = args.listen_on
+        ip_addr = listen_on
     if ip_addr == "*":
         ip_addr = ""
+    return (ip_addr, port)
+
+wsgi_listener: Optional[WsgiListener] = None
+if args.wsgi:
+    match = fullmatch(r"([\w.]+)\.(\w+)", args.wsgi)
+    if not match:
+        raise ValueError(f"need to specify module.function, got '{args.wsgi}'")
+    module, function = match.groups()
+    imported = import_module(module)
+    app = getattr(imported, function, None)
+    if not app:
+        raise ValueError(f"{function} not found in {module}")
+    ip_addr, port = parse_listen_on(args.wsgi_listen_on, "*", "8081")
+    wsgi_listener = WsgiListener(app, ip_addr=ip_addr, port=int(port))
+
+if args.listen_on:
+    ip_addr, port = parse_listen_on(args.listen_on, "*", "8080")
     database.start_listening(ip_addr=ip_addr, port=port)
 
 for target in (args.connect_to or []):
     database.connect_to(target)
 
 if args.interactive:
     interactive = True
 elif args.line_mode:
     interactive = False
 else:
     interactive = stdin.isatty()
 
 console = SelectableConsole(locals(), interactive=interactive, heartbeat_to=args.heartbeat_to)
 
-loop(console, database, context_manager=console)
+loop(console, database, wsgi_listener, context_manager=console)
```

### Comparing `gink-0.20240521.1716315298/gink/builders/behavior_pb2.py` & `gink-0.20240523.1716450705/gink/builders/behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/builders/bundle_pb2.py` & `gink-0.20240523.1716450705/gink/builders/bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/builders/change_pb2.py` & `gink-0.20240523.1716450705/gink/builders/change_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/builders/claim_pb2.py` & `gink-0.20240523.1716450705/gink/builders/claim_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/builders/clearance_pb2.py` & `gink-0.20240523.1716450705/gink/builders/clearance_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/builders/container_pb2.py` & `gink-0.20240523.1716450705/gink/builders/container_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/builders/entry_pb2.py` & `gink-0.20240523.1716450705/gink/builders/entry_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/builders/header_pb2.py` & `gink-0.20240523.1716450705/gink/builders/header_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/builders/key_pb2.py` & `gink-0.20240523.1716450705/gink/builders/key_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/builders/log_file_pb2.py` & `gink-0.20240523.1716450705/gink/builders/log_file_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/builders/movement_pb2.py` & `gink-0.20240523.1716450705/gink/builders/movement_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/builders/muid_pb2.py` & `gink-0.20240523.1716450705/gink/builders/muid_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/builders/pair_pb2.py` & `gink-0.20240523.1716450705/gink/builders/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/builders/sync_message_pb2.py` & `gink-0.20240523.1716450705/gink/builders/sync_message_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/builders/value_pb2.py` & `gink-0.20240523.1716450705/gink/builders/value_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/abstract_store.py` & `gink-0.20240523.1716450705/gink/impl/abstract_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/addressable.py` & `gink-0.20240523.1716450705/gink/impl/addressable.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/attribution.py` & `gink-0.20240523.1716450705/gink/impl/attribution.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/box.py` & `gink-0.20240523.1716450705/gink/impl/box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/braid.py` & `gink-0.20240523.1716450705/gink/impl/braid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/builders.py` & `gink-0.20240523.1716450705/gink/impl/builders.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/bundle_info.py` & `gink-0.20240523.1716450705/gink/impl/bundle_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/bundle_store.py` & `gink-0.20240523.1716450705/gink/impl/bundle_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/bundle_wrapper.py` & `gink-0.20240523.1716450705/gink/impl/bundle_wrapper.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/bundler.py` & `gink-0.20240523.1716450705/gink/impl/bundler.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/chain_tracker.py` & `gink-0.20240523.1716450705/gink/impl/chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/coding.py` & `gink-0.20240523.1716450705/gink/impl/coding.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/connection.py` & `gink-0.20240523.1716450705/gink/impl/connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/container.py` & `gink-0.20240523.1716450705/gink/impl/container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/database.py` & `gink-0.20240523.1716450705/gink/impl/database.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/deferred.py` & `gink-0.20240523.1716450705/gink/impl/deferred.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/directory.py` & `gink-0.20240523.1716450705/gink/impl/directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/graph.py` & `gink-0.20240523.1716450705/gink/impl/graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/group.py` & `gink-0.20240523.1716450705/gink/impl/group.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/key_set.py` & `gink-0.20240523.1716450705/gink/impl/key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/listener.py` & `gink-0.20240523.1716450705/gink/impl/listener.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/lmdb_store.py` & `gink-0.20240523.1716450705/gink/impl/lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/lmdb_utilities.py` & `gink-0.20240523.1716450705/gink/impl/lmdb_utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/log_backed_store.py` & `gink-0.20240523.1716450705/gink/impl/log_backed_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/looping.py` & `gink-0.20240523.1716450705/gink/impl/looping.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,24 +20,26 @@
         """ close the file object """
 
     def on_ready(self) -> Optional[Iterable[Selectable]]:
         """ what to call when selected """
 
 
 def loop(
-        *selectables: Selectable,
+        *selectables: Optional[Selectable],
         context_manager: ContextManager = nullcontext(),
         selector: Optional[BaseSelector] = None,
         until: GenericTimestamp = None,
         ) -> None:
     selector = selector or DefaultSelector()
+    assert isinstance(selector, BaseSelector)
     registered: Set[Selectable] = set()
     until_muts = None if until is None else resolve_timestamp(until)
 
-    def add(_selectables):
+    def add(_selectables: Iterable[Optional[Selectable]]):
+        assert isinstance(selector, BaseSelector)
         for selectable in _selectables:
             if selectable and selectable not in registered:
                 selector.register(selectable, EVENT_READ)
                 registered.add(selectable)
 
     add(selectables)
     with context_manager:
@@ -52,13 +54,15 @@
                     results = selectable.on_ready()
                     if results:
                         add(results)
                 except Finished:
                     selector.unregister(selectable)
                     selectable.close()
                     registered.remove(selectable)
+                    if selectable is context_manager:
+                        until_muts = 0
             else:
                 for selectable in registered:
                     if hasattr(selectable, "on_timeout"):
                         selectable.on_timeout()
         for selectable in registered:
             selector.unregister(selectable)
```

### Comparing `gink-0.20240521.1716315298/gink/impl/memory_store.py` & `gink-0.20240523.1716450705/gink/impl/memory_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/muid.py` & `gink-0.20240523.1716450705/gink/impl/muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/pair_map.py` & `gink-0.20240523.1716450705/gink/impl/pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/pair_set.py` & `gink-0.20240523.1716450705/gink/impl/pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/property.py` & `gink-0.20240523.1716450705/gink/impl/property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/selectable_console.py` & `gink-0.20240523.1716450705/gink/impl/selectable_console.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 from logging import getLogger
 from ctypes import c_int
 from fcntl import ioctl
 from termios import FIONREAD
 from pathlib import Path
 from datetime import datetime as DateTime
 
+from .looping import Finished
+
 class SelectableConsole(InteractiveInterpreter):
 
     def __init__(self, locals, interactive: bool, heartbeat_to: Optional[Path]=None):
         """ Line mode (non-interactive), if specified, or if not using a TTY.
         """
         super().__init__(locals)
         self._interactive = interactive
         self._buffer: List[str] = []
         self._input: TextIO = stdin
         self._output: TextIO = stderr
         self._settings: Optional[list] = None
         self._prompt = "python+gink> "
         self._logger = getLogger(self.__class__.__name__)
-        self._ended = False
         self._c_int = c_int()
         self._heartbeat_to = open(heartbeat_to, "a") if heartbeat_to else None
 
-    def is_active(self) -> bool:
-        return not self._ended
+    def close(self):
+        pass
 
     def fileno(self) -> int:
       return self._input.fileno()
 
     def __enter__(self):
         if self._settings is None and self._interactive:
             fd = self._input.fileno()
@@ -58,14 +59,16 @@
                   self.on_character(self._input.read(1))
             else:
                 self.on_line(input())
         except KeyboardInterrupt:
             self.write("\nKeyboardInterrupt\n")
         except StopIteration:
             pass
+        except EOFError:
+            raise Finished()
 
     def on_line(self, line):
         result = self.runsource(line)
         if result is True:
             self._logger.warning("multi-line input not yet implemented")
 
     def on_timeout(self):
```

### Comparing `gink-0.20240521.1716315298/gink/impl/sequence.py` & `gink-0.20240523.1716450705/gink/impl/sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/tuples.py` & `gink-0.20240523.1716450705/gink/impl/tuples.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/typedefs.py` & `gink-0.20240523.1716450705/gink/impl/typedefs.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/utilities.py` & `gink-0.20240523.1716450705/gink/impl/utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/watcher.py` & `gink-0.20240523.1716450705/gink/impl/watcher.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/websocket_connection.py` & `gink-0.20240523.1716450705/gink/impl/websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/wsgi_connection.py` & `gink-0.20240523.1716450705/gink/impl/wsgi_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/impl/wsgi_listener.py` & `gink-0.20240523.1716450705/gink/impl/wsgi_listener.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_box.py` & `gink-0.20240523.1716450705/gink/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_braid.py` & `gink-0.20240523.1716450705/gink/tests/test_braid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_chain_tracker.py` & `gink-0.20240523.1716450705/gink/tests/test_chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_change_set_info.py` & `gink-0.20240523.1716450705/gink/tests/test_change_set_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_code_values.py` & `gink-0.20240523.1716450705/gink/tests/test_code_values.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_container.py` & `gink-0.20240523.1716450705/gink/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_database.py` & `gink-0.20240523.1716450705/gink/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_demo.py` & `gink-0.20240523.1716450705/gink/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_directory.py` & `gink-0.20240523.1716450705/gink/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_graph.py` & `gink-0.20240523.1716450705/gink/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_key_set.py` & `gink-0.20240523.1716450705/gink/tests/test_key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_lmdb_store.py` & `gink-0.20240523.1716450705/gink/tests/test_lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_logbackedstore.py` & `gink-0.20240523.1716450705/gink/tests/test_logbackedstore.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_muid.py` & `gink-0.20240523.1716450705/gink/tests/test_muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_names.py` & `gink-0.20240523.1716450705/gink/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_pair_map.py` & `gink-0.20240523.1716450705/gink/tests/test_pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_pair_set.py` & `gink-0.20240523.1716450705/gink/tests/test_pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_property.py` & `gink-0.20240523.1716450705/gink/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_role.py` & `gink-0.20240523.1716450705/gink/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_sequence.py` & `gink-0.20240523.1716450705/gink/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_store.py` & `gink-0.20240523.1716450705/gink/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_websocket_connection.py` & `gink-0.20240523.1716450705/gink/tests/test_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink/tests/test_wsgi_server.py` & `gink-0.20240523.1716450705/gink/tests/test_wsgi_server.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/gink.egg-info/PKG-INFO` & `gink-0.20240523.1716450705/gink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240521.1716315298
+Version: 0.20240523.1716450705
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240521.1716315298/gink.egg-info/SOURCES.txt` & `gink-0.20240523.1716450705/gink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gink-0.20240521.1716315298/setup.py` & `gink-0.20240523.1716450705/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name='gink',
-    version='0.20240521.1716315298',
+    version='0.20240523.1716450705',
     description='a system for storing data structures in lmdb',
     url='https://github.com/x5e/gink',
     author='Darin McGill',
     author_email="gink@darinmcgill.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         "Intended Audience :: Developers",
```

