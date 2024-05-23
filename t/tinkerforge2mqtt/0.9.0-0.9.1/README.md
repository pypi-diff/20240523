# Comparing `tmp/tinkerforge2mqtt-0.9.0.tar.gz` & `tmp/tinkerforge2mqtt-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinkerforge2mqtt-0.9.0.tar", last modified: Mon May 20 09:24:35 2024, max compression
+gzip compressed data, was "tinkerforge2mqtt-0.9.1.tar", last modified: Thu May 23 15:13:17 2024, max compression
```

## Comparing `tinkerforge2mqtt-0.9.0.tar` & `tinkerforge2mqtt-0.9.1.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.156477 tinkerforge2mqtt-0.9.0/
--rw-rw-r--   0 jens      (1000) jens      (1000)      310 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/.editorconfig
--rw-rw-r--   0 jens      (1000) jens      (1000)      153 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/.flake8
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.148477 tinkerforge2mqtt-0.9.0/.github/
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.152477 tinkerforge2mqtt-0.9.0/.github/workflows/
--rw-rw-r--   0 jens      (1000) jens      (1000)     1670 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) jens      (1000)      116 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/.gitignore
--rw-r--r--   0 jens      (1000) jens      (1000)     3731 2024-05-20 09:24:35.156477 tinkerforge2mqtt-0.9.0/PKG-INFO
--rw-rw-r--   0 jens      (1000) jens      (1000)     2404 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/README.md
--rwxrwxr-x   0 jens      (1000) jens      (1000)     3159 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/cli.py
--rwxrwxr-x   0 jens      (1000) jens      (1000)     3089 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/dev-cli.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     4935 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/pyproject.toml
--rw-rw-r--   0 jens      (1000) jens      (1000)    75058 2024-05-20 08:34:35.000000 tinkerforge2mqtt-0.9.0/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)    11196 2024-05-20 08:34:00.000000 tinkerforge2mqtt-0.9.0/requirements.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)       38 2024-05-20 09:24:35.156477 tinkerforge2mqtt-0.9.0/setup.cfg
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.152477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/
--rw-rw-r--   0 jens      (1000) jens      (1000)      137 2024-05-20 09:16:15.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      178 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/__main__.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.152477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/
--rw-rw-r--   0 jens      (1000) jens      (1000)     1364 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     3981 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/discovering.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     2563 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/publish.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     1395 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/settings.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     2486 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/systemd.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      806 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/update_readme_history.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.152477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/
--rw-rw-r--   0 jens      (1000) jens      (1000)     2163 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      968 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/code_style.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     2472 2024-05-20 08:41:33.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/packaging.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     1520 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/testing.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      179 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/constants.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.152477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/
--rw-rw-r--   0 jens      (1000) jens      (1000)     1236 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     1949 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/brick_hat_zero.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     2848 2024-04-17 16:12:57.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_analog_in_v3.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     3638 2024-05-20 09:16:15.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_humidity_v2.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     2817 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_industrial_dual_relay.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     1998 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_motion_detector_v2.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     2332 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_solid_state_relay_v2.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     1903 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_temperature_v2.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     3677 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_voltage_current_v2.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.152477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map_utils/
--rw-rw-r--   0 jens      (1000) jens      (1000)        0 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map_utils/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     4214 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map_utils/base.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      566 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map_utils/generics.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.152477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_registry/
--rw-rw-r--   0 jens      (1000) jens      (1000)        0 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_registry/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     2664 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_registry/devices_handler.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.156477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/tests/
--rw-rw-r--   0 jens      (1000) jens      (1000)     1197 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/tests/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)      227 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     1478 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     1227 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/user_settings.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.156477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/utilities/
--rw-rw-r--   0 jens      (1000) jens      (1000)        0 2024-05-20 09:16:15.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) jens      (1000)     1283 2024-05-20 09:16:15.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/utilities/dew_point.py
-drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.156477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/
--rw-r--r--   0 jens      (1000) jens      (1000)     3731 2024-05-20 09:24:35.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) jens      (1000)     1808 2024-05-20 09:24:35.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)        1 2024-05-20 09:24:35.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)      125 2024-05-20 09:24:35.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)      270 2024-05-20 09:24:35.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) jens      (1000)       17 2024-05-20 09:24:35.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/top_level.txt
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-23 15:13:17.478400 tinkerforge2mqtt-0.9.1/
+-rw-rw-r--   0 jens      (1000) users      (100)      310 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.9.1/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.9.1/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-23 15:13:17.478400 tinkerforge2mqtt-0.9.1/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-23 15:13:17.478400 tinkerforge2mqtt-0.9.1/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1670 2024-05-23 15:12:24.000000 tinkerforge2mqtt-0.9.1/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      116 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.9.1/.gitignore
+-rw-r--r--   0 jens      (1000) users      (100)     3731 2024-05-23 15:13:17.478400 tinkerforge2mqtt-0.9.1/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     2404 2024-05-23 15:12:24.000000 tinkerforge2mqtt-0.9.1/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3159 2024-05-23 15:12:24.000000 tinkerforge2mqtt-0.9.1/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3089 2024-05-23 15:12:24.000000 tinkerforge2mqtt-0.9.1/dev-cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4935 2024-05-23 15:12:38.000000 tinkerforge2mqtt-0.9.1/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    75058 2024-05-23 15:12:24.000000 tinkerforge2mqtt-0.9.1/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    11196 2024-05-23 15:12:24.000000 tinkerforge2mqtt-0.9.1/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2024-05-23 15:13:17.478400 tinkerforge2mqtt-0.9.1/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-23 15:13:17.478400 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/
+-rw-rw-r--   0 jens      (1000) users      (100)      137 2024-05-23 15:12:24.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      178 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/__main__.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-23 15:13:17.478400 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_app/
+-rw-rw-r--   0 jens      (1000) users      (100)     1080 2024-05-23 15:12:24.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_app/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3981 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_app/discovering.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2563 2024-03-23 12:12:57.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_app/publish.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1395 2024-03-12 08:36:23.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_app/settings.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2486 2024-03-12 08:36:51.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_app/systemd.py
+-rw-rw-r--   0 jens      (1000) users      (100)      806 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_app/update_readme_history.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-23 15:13:17.478400 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_dev/
+-rw-rw-r--   0 jens      (1000) users      (100)     1879 2024-05-23 15:12:24.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_dev/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      968 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_dev/code_style.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2472 2024-05-23 15:12:24.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_dev/packaging.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1520 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_dev/testing.py
+-rw-rw-r--   0 jens      (1000) users      (100)      179 2024-03-10 18:32:00.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/constants.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-23 15:13:17.478400 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/
+-rw-rw-r--   0 jens      (1000) users      (100)     1236 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1999 2024-05-21 19:17:21.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/brick_hat_zero.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4237 2024-05-21 19:17:21.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/bricklet_analog_in_v3.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3723 2024-05-23 15:08:01.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/bricklet_humidity_v2.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2867 2024-05-21 19:17:21.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/bricklet_industrial_dual_relay.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2048 2024-05-21 19:17:21.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/bricklet_motion_detector_v2.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2382 2024-05-21 19:17:21.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/bricklet_solid_state_relay_v2.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1953 2024-05-21 19:17:21.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/bricklet_temperature_v2.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3727 2024-05-21 19:17:21.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/bricklet_voltage_current_v2.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-23 15:13:17.478400 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3649 2024-05-21 19:17:21.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map_utils/base.py
+-rw-rw-r--   0 jens      (1000) users      (100)      566 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map_utils/generics.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1689 2024-05-21 19:17:21.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map_utils/led_config.py
+-rw-rw-r--   0 jens      (1000) users      (100)      394 2024-05-21 19:17:21.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map_utils/utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-23 15:13:17.478400 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_registry/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_registry/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2664 2024-03-25 16:32:13.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_registry/devices_handler.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-23 15:13:17.478400 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)     1197 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      227 2024-03-10 18:32:00.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1478 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1227 2024-03-25 16:26:57.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/user_settings.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-23 15:13:17.478400 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2024-05-21 19:17:21.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1283 2024-05-21 19:17:21.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/utilities/dew_point.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-05-23 15:13:17.478400 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt.egg-info/
+-rw-r--r--   0 jens      (1000) users      (100)     3731 2024-05-23 15:13:17.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     1899 2024-05-23 15:13:17.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2024-05-23 15:13:17.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      125 2024-05-23 15:13:17.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      270 2024-05-23 15:13:17.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       17 2024-05-23 15:13:17.000000 tinkerforge2mqtt-0.9.1/tinkerforge2mqtt.egg-info/top_level.txt
```

### Comparing `tinkerforge2mqtt-0.9.0/.github/workflows/tests.yml` & `tinkerforge2mqtt-0.9.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/PKG-INFO` & `tinkerforge2mqtt-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinkerforge2mqtt
-Version: 0.9.0
+Version: 0.9.1
 Summary: Emit MQTT events from Tinkerforge devices
 Author-email: Jens Diemer <git@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/tinkerforge2mqtt
 Project-URL: Source, https://github.com/jedie/tinkerforge2mqtt
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `tinkerforge2mqtt-0.9.0/README.md` & `tinkerforge2mqtt-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/cli.py` & `tinkerforge2mqtt-0.9.1/cli.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/dev-cli.py` & `tinkerforge2mqtt-0.9.1/dev-cli.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/pyproject.toml` & `tinkerforge2mqtt-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/requirements.dev.txt` & `tinkerforge2mqtt-0.9.1/requirements.dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    ./dev-cli.py update
 #
-annotated-types==0.6.0 \
-    --hash=sha256:0641064de18ba7a25dee8f96403ebc39113d0cb953a01429249d5c7564666a43 \
-    --hash=sha256:563339e807e53ffd9c267e99fc6d9ea23eb8443c08f112651963e24e22f84a5d
+annotated-types==0.7.0 \
+    --hash=sha256:1f02e8b43a8fbbc3f3e0d4f0f4bfc8131bcb4eebe8849b8e5c773f3a1c582a53 \
+    --hash=sha256:aff07c09a53a08bc8cfccb9c85b05f1aa9a2a6f23728d790723543408344ce89
     # via pydantic
 arrow==1.3.0 \
     --hash=sha256:c728b120ebc00eb84e01882a6f5e7927a53960aa990ce7dd2b10f39005a67f80 \
     --hash=sha256:d4540617648cb5f895730f1ad8c82a65f2dad0166f57b75f3ca54759c4d67a85
     # via cookiecutter
 astor==0.8.1 \
     --hash=sha256:070a54e890cefb5b3739d19f30f5a5ec840ffc9c50ffa7d23cc9fc1a38ebbfc5 \
@@ -28,17 +28,17 @@
     --hash=sha256:959ea62a5b7b5123c5059758296122b57cd2585ae2ed1c0622c21b371ffdae06 \
     --hash=sha256:9637e4de1fb498310a56900b3e2043a206b03cb11c05422014b0302cbc814be3
     # via safety
 autoflake==2.3.1 \
     --hash=sha256:3ae7495db9084b7b32818b4140e6dc4fc280b712fb414f5b8fe57b0a8e85a840 \
     --hash=sha256:c98b75dc5b0a86459c4f01a1d32ac7eb4338ec4317a4469515ff1e687ecd909e
     # via manageprojects
-autopep8==2.1.0 \
-    --hash=sha256:1fa8964e4618929488f4ec36795c7ff12924a68b8bf01366c094fc52f770b6e7 \
-    --hash=sha256:2bb76888c5edbcafe6aabab3c47ba534f5a2c2d245c2eddced4a30c4b4946357
+autopep8==2.1.1 \
+    --hash=sha256:57c1026ee3ee40f57c5b93073b705f8e30aa52411fca33306d730274d2882bba \
+    --hash=sha256:bc9b267f14d358a9af574b95e95a661681c60a275ffce419ba5fb4eae9920bcc
     # via
     #   manageprojects
     #   tinkerforge2mqtt (pyproject.toml)
 backports-tarfile==1.1.1 \
     --hash=sha256:73e0179647803d3726d82e76089d01d8549ceca9bace469953fcb4d97cf2d417 \
     --hash=sha256:9c2ef9696cb73374f7164e17fc761389393ca76777036f5aad42e8b93fcd8009
     # via jaraco-context
@@ -932,17 +932,17 @@
     --hash=sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d \
     --hash=sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f
     # via cookiecutter
 readme-renderer==43.0 \
     --hash=sha256:1818dd28140813509eeed8d62687f7cd4f7bad90d4db586001c5dc09d4fde311 \
     --hash=sha256:19db308d86ecd60e5affa3b2a98f017af384678c63c88e5d4556a380e674f3f9
     # via twine
-requests==2.31.0 \
-    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
-    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
+requests==2.32.2 \
+    --hash=sha256:dd951ff5ecf3e3b3aa26b40703ba77495dab41da839ae72ef3c8e5d8e2433289 \
+    --hash=sha256:fc06670dd0ed212426dfeb94fc1b983d917c4f9847c863f313c9dfaaffb7c23c
     # via
     #   cookiecutter
     #   requests-toolbelt
     #   safety
     #   twine
 requests-toolbelt==1.0.0 \
     --hash=sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6 \
@@ -1135,13 +1135,13 @@
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==24.0 \
     --hash=sha256:ba0d021a166865d2265246961bec0152ff124de910c5cc39f1156ce3fa7c69dc \
     --hash=sha256:ea9bd1a847e8c5774a5777bb398c19e80bcd4e2aa16a4b301b718fe6f593aba2
     # via pip-tools
-setuptools==69.5.1 \
-    --hash=sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987 \
-    --hash=sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32
+setuptools==70.0.0 \
+    --hash=sha256:54faa7f2e8d2d11bcd2c07bed282eef1046b5c080d1c32add737d7b5817b1ad4 \
+    --hash=sha256:f211a66637b8fa059bb28183da127d4e86396c991a942b028c6650d4319c3fd0
     # via
     #   pip-tools
     #   safety
```

### Comparing `tinkerforge2mqtt-0.9.0/requirements.txt` & `tinkerforge2mqtt-0.9.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/__init__.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_app/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 """
 
 import logging
 import sys
 
 import rich_click as click
 from rich import print  # noqa
-from rich.console import Console
-from rich.traceback import install as rich_traceback_install
 from rich_click import RichGroup
 
 from cli_base.autodiscover import import_all_files
 from cli_base.cli_tools.version_info import print_version
 
 import tinkerforge2mqtt
 from tinkerforge2mqtt import constants
@@ -45,18 +43,10 @@
     # Pseudo command, because the version always printed on every CLI call ;)
     sys.exit(0)
 
 
 def main():
     print_version(tinkerforge2mqtt)
 
-    console = Console()
-    rich_traceback_install(
-        width=console.size.width,  # full terminal width
-        show_locals=True,
-        suppress=[click],
-        max_frames=2,
-    )
-
     # Execute Click CLI:
     cli.name = './cli.py'
     cli()
```

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/discovering.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_app/discovering.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/publish.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_app/publish.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/settings.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_app/settings.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/systemd.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_app/systemd.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/update_readme_history.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_app/update_readme_history.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/__init__.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_dev/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 """
 
 import logging
 import sys
 
 import rich_click as click
 from bx_py_utils.path import assert_is_file
-from rich.console import Console
-from rich.traceback import install as rich_traceback_install
 from rich_click import RichGroup
 from typeguard import install_import_hook
 
 from cli_base.autodiscover import import_all_files
 from cli_base.cli_tools.dev_tools import run_coverage, run_tox, run_unittest_cli
 from cli_base.cli_tools.version_info import print_version
 
@@ -56,22 +54,14 @@
     # Pseudo command, because the version always printed on every CLI call ;)
     sys.exit(0)
 
 
 def main():
     print_version(tinkerforge2mqtt)
 
-    console = Console()
-    rich_traceback_install(
-        width=console.size.width,  # full terminal width
-        show_locals=True,
-        suppress=[click],
-        max_frames=8,
-    )
-
     if len(sys.argv) >= 2:
         # Check if we can just pass a command call to origin CLI:
         command = sys.argv[1]
         command_map = {
             'test': run_unittest_cli,
             'tox': run_tox,
             'coverage': run_coverage,
```

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/code_style.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_dev/code_style.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/packaging.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_dev/packaging.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/testing.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/cli_dev/testing.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/__init__.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/__init__.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/brick_hat_zero.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/brick_hat_zero.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from ha_services.mqtt4homeassistant.components.sensor import Sensor
 from tinkerforge.brick_hat_zero import BrickHATZero
 
 from tinkerforge2mqtt.device_map import register_map_class
-from tinkerforge2mqtt.device_map_utils.base import DeviceMapBase, print_exception_decorator
-
+from tinkerforge2mqtt.device_map_utils.base import DeviceMapBase
+from tinkerforge2mqtt.device_map_utils.utils import print_exception_decorator
 
 logger = logging.getLogger(__name__)
 
 
 @register_map_class()
 class BrickHATZeroMapper(DeviceMapBase):
     # https://www.tinkerforge.com/de/doc/Software/Bricks/HATZero_Brick_Python.html
```

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_humidity_v2.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/bricklet_humidity_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             state_class='measurement',
             unit_of_measurement='°C',
             suggested_display_precision=2,
         )
         self.dew_point = Sensor(
             device=self.mqtt_device,
             name='Dew Point Temperature',
-            uid='temperature',
+            uid='dew_point',
             device_class='temperature',
             state_class='measurement',
             unit_of_measurement='°C',
             suggested_display_precision=2,
         )
 
     @print_exception_decorator
@@ -87,14 +87,15 @@
         humidity = value / 100
         logger.info(f'Humidity callback: {humidity}% (UID: {self.device.uid_string})')
         self.humidity.set_state(humidity)
         self.humidity.publish(self.mqtt_client)
         self.set_and_publish_dew_point()
 
     def set_and_publish_dew_point(self):
-        dew_point = calculate_dew_point(
-            temperature=self.temperature.value,
-            humidity=self.humidity.value,
-        )
-        logger.info(f'Dew Point: {dew_point}°C (UID: {self.device.uid_string})')
-        self.dew_point.set_state(dew_point)
-        self.dew_point.publish(self.mqtt_client)
+        if self.temperature.value and self.humidity.value:
+            dew_point = calculate_dew_point(
+                temperature=self.temperature.value,
+                humidity=self.humidity.value,
+            )
+            logger.info(f'Dew Point: {dew_point}°C (UID: {self.device.uid_string})')
+            self.dew_point.set_state(dew_point)
+            self.dew_point.publish(self.mqtt_client)
```

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_industrial_dual_relay.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/bricklet_industrial_dual_relay.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 
 from ha_services.mqtt4homeassistant.components.switch import Switch
 from paho.mqtt.client import Client
 from tinkerforge.bricklet_industrial_dual_relay import BrickletIndustrialDualRelay
 
 from tinkerforge2mqtt.device_map import register_map_class
-from tinkerforge2mqtt.device_map_utils.base import DeviceMapBase, print_exception_decorator
-
+from tinkerforge2mqtt.device_map_utils.base import DeviceMapBase
+from tinkerforge2mqtt.device_map_utils.utils import print_exception_decorator
 
 logger = logging.getLogger(__name__)
 
 
 @register_map_class()
 class BrickletIndustrialDualRelayMapper(DeviceMapBase):
     # https://www.tinkerforge.com/de/doc/Software/Bricklets/IndustrialDualRelay_Bricklet_Python.html
```

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_motion_detector_v2.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/bricklet_motion_detector_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from ha_services.mqtt4homeassistant.components.binary_sensor import BinarySensor
 from tinkerforge.bricklet_motion_detector_v2 import BrickletMotionDetectorV2
 
 from tinkerforge2mqtt.device_map import register_map_class
-from tinkerforge2mqtt.device_map_utils.base import DeviceMapBase, print_exception_decorator
-
+from tinkerforge2mqtt.device_map_utils.base import DeviceMapBase
+from tinkerforge2mqtt.device_map_utils.utils import print_exception_decorator
 
 logger = logging.getLogger(__name__)
 
 
 @register_map_class()
 class BrickletMotionDetectorV2Mapper(DeviceMapBase):
     # https://www.tinkerforge.com/de/doc/Software/Bricklets/MotionDetectorV2_Bricklet_Python.html
```

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_solid_state_relay_v2.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/bricklet_solid_state_relay_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 
 from ha_services.mqtt4homeassistant.components.switch import Switch
 from paho.mqtt.client import Client
 from tinkerforge.bricklet_solid_state_relay_v2 import BrickletSolidStateRelayV2
 
 from tinkerforge2mqtt.device_map import register_map_class
-from tinkerforge2mqtt.device_map_utils.base import DeviceMapBase, print_exception_decorator
-
+from tinkerforge2mqtt.device_map_utils.base import DeviceMapBase
+from tinkerforge2mqtt.device_map_utils.utils import print_exception_decorator
 
 logger = logging.getLogger(__name__)
 
 
 @register_map_class()
 class BrickletSolidStateRelayV2Mapper(DeviceMapBase):
     # https://www.tinkerforge.com/de/doc/Software/Bricklets/SolidStateRelayV2_Bricklet_Python.html
```

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_temperature_v2.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/bricklet_temperature_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from ha_services.mqtt4homeassistant.components.sensor import Sensor
 from tinkerforge.bricklet_temperature_v2 import BrickletTemperatureV2
 
 from tinkerforge2mqtt.device_map import register_map_class
-from tinkerforge2mqtt.device_map_utils.base import DeviceMapBase, print_exception_decorator
-
+from tinkerforge2mqtt.device_map_utils.base import DeviceMapBase
+from tinkerforge2mqtt.device_map_utils.utils import print_exception_decorator
 
 logger = logging.getLogger(__name__)
 
 
 @register_map_class()
 class BrickletTemperatureV2Mapper(DeviceMapBase):
     # https://www.tinkerforge.com/de/doc/Software/Bricks/HATZero_Brick_Python.html
```

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_voltage_current_v2.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map/bricklet_voltage_current_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from ha_services.mqtt4homeassistant.components.sensor import Sensor
 from tinkerforge.bricklet_voltage_current_v2 import BrickletVoltageCurrentV2
 
 from tinkerforge2mqtt.device_map import register_map_class
-from tinkerforge2mqtt.device_map_utils.base import DeviceMapBase, print_exception_decorator
-
+from tinkerforge2mqtt.device_map_utils.base import DeviceMapBase
+from tinkerforge2mqtt.device_map_utils.utils import print_exception_decorator
 
 logger = logging.getLogger(__name__)
 
 
 @register_map_class()
 class BrickletVoltageCurrentV2Mapper(DeviceMapBase):
     # https://www.tinkerforge.com/de/doc/Software/Bricklets/VoltageCurrentV2_Bricklet_Python.html
```

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map_utils/base.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map_utils/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,25 @@
 import abc
 import logging
-from functools import wraps
 
 from ha_services.mqtt4homeassistant.components.sensor import Sensor
 from ha_services.mqtt4homeassistant.device import MainMqttDevice, MqttDevice
 from paho.mqtt.client import Client
 from rich import print  # noqa
-from rich.console import Console
 from tinkerforge.ip_connection import Device
 
 from tinkerforge2mqtt.device_map_utils.generics import iter_interest_functions
+from tinkerforge2mqtt.device_map_utils.led_config import BrickletLedConfigSelect
+from tinkerforge2mqtt.device_map_utils.utils import print_exception_decorator
 from tinkerforge2mqtt.user_settings import UserSettings
 
 
 logger = logging.getLogger(__name__)
 
 
-def print_exception_decorator(func):
-
-    @wraps(func)
-    def func_wrapper(*args, **kwargs):
-        try:
-            return func(*args, **kwargs)
-        except Exception as err:
-            console = Console()
-            console.print_exception(show_locals=True)
-            raise SystemExit from err
-
-    return func_wrapper
-
-
 class DeviceMapBase(abc.ABC):
     device_identifier: int
 
     @abc.abstractmethod
     def __init__(
         self,
         *,
@@ -71,20 +57,15 @@
                 state_class='measurement',
                 unit_of_measurement='°C',
                 suggested_display_precision=0,
             )
             logger.info(f'Sensor: {self.chip_temperature_sensor}')
 
         if hasattr(self.device, 'get_status_led_config'):
-            self.led_config_sensor = Sensor(
-                device=self.mqtt_device,
-                name='LED Config',
-                uid='led_config',
-                device_class='enum',
-            )
+            self.led_config_sensor = BrickletLedConfigSelect(device=self.device, mqtt_device=self.mqtt_device)
             logger.info(f'Sensor: {self.led_config_sensor}')
 
     @abc.abstractmethod
     def setup_callbacks(self):
         pass
 
     def iter_known_functions(self, device: Device):
@@ -101,19 +82,16 @@
         if get_chip_temperature := getattr(self.device, 'get_chip_temperature', None):
             value = get_chip_temperature()
             logger.debug(f'{self.device.DEVICE_DISPLAY_NAME} chip temperature: {value}°C')
             self.chip_temperature_sensor.set_state(state=value)
             self.chip_temperature_sensor.publish(self.mqtt_client)
             logger.info(f'Chip temperature: {value}°C: {self.chip_temperature_sensor}')
 
-        if get_status_led_config := getattr(self.device, 'get_status_led_config', None):
-            value = get_status_led_config()
-            logger.info(f'{self.device.DEVICE_DISPLAY_NAME} status LED config: {value}')
-            self.led_config_sensor.set_state(state=value)
-            self.led_config_sensor.publish(self.mqtt_client)
+        if hasattr(self, 'led_config_sensor'):
+            self.led_config_sensor.poll(self.mqtt_client)
 
         self.main_mqtt_device.poll_and_publish(self.mqtt_client)
 
     def get_sw_version(self) -> str:
         api_version = self.device.get_api_version()
         sw_version = '.'.join(str(number) for number in api_version)
         return sw_version
```

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map_utils/generics.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_map_utils/generics.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_registry/devices_handler.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/device_registry/devices_handler.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/tests/__init__.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/tests/test_project_setup.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/user_settings.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/user_settings.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/utilities/dew_point.py` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt/utilities/dew_point.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/PKG-INFO` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinkerforge2mqtt
-Version: 0.9.0
+Version: 0.9.1
 Summary: Emit MQTT events from Tinkerforge devices
 Author-email: Jens Diemer <git@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/tinkerforge2mqtt
 Project-URL: Source, https://github.com/jedie/tinkerforge2mqtt
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/SOURCES.txt` & `tinkerforge2mqtt-0.9.1/tinkerforge2mqtt.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 tinkerforge2mqtt/device_map/bricklet_motion_detector_v2.py
 tinkerforge2mqtt/device_map/bricklet_solid_state_relay_v2.py
 tinkerforge2mqtt/device_map/bricklet_temperature_v2.py
 tinkerforge2mqtt/device_map/bricklet_voltage_current_v2.py
 tinkerforge2mqtt/device_map_utils/__init__.py
 tinkerforge2mqtt/device_map_utils/base.py
 tinkerforge2mqtt/device_map_utils/generics.py
+tinkerforge2mqtt/device_map_utils/led_config.py
+tinkerforge2mqtt/device_map_utils/utils.py
 tinkerforge2mqtt/device_registry/__init__.py
 tinkerforge2mqtt/device_registry/devices_handler.py
 tinkerforge2mqtt/tests/__init__.py
 tinkerforge2mqtt/tests/test_doctests.py
 tinkerforge2mqtt/tests/test_project_setup.py
 tinkerforge2mqtt/utilities/__init__.py
 tinkerforge2mqtt/utilities/dew_point.py
```

