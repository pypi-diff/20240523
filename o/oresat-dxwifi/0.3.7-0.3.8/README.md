# Comparing `tmp/oresat_dxwifi-0.3.7.tar.gz` & `tmp/oresat_dxwifi-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat_dxwifi-0.3.7.tar", last modified: Sat Apr 27 06:01:13 2024, max compression
+gzip compressed data, was "oresat_dxwifi-0.3.8.tar", last modified: Thu May 23 03:08:34 2024, max compression
```

## Comparing `oresat_dxwifi-0.3.7.tar` & `oresat_dxwifi-0.3.8.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:13.421373 oresat_dxwifi-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:13.405373 oresat_dxwifi-0.3.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:13.409373 oresat_dxwifi-0.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-27 06:01:13.421373 oresat_dxwifi-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2384 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/build-deb.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:13.405373 oresat_dxwifi-0.3.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:13.409373 oresat_dxwifi-0.3.7/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   100917 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/docs/images/hgs-browser.png
--rw-r--r--   0 runner    (1001) docker     (127)    90640 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/docs/images/olaf-browser.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/kill-olaf
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat-dxwifi-software-server.service
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat-mon-iface.service
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat-vcan-iface.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:13.413373 oresat_dxwifi-0.3.7/oresat_dxwifi/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 06:01:13.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:13.413373 oresat_dxwifi-0.3.7/oresat_dxwifi/camera/
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/camera/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/camera/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/camera/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/camera/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:13.413373 oresat_dxwifi-0.3.7/oresat_dxwifi/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/resources/temperature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:13.413373 oresat_dxwifi-0.3.7/oresat_dxwifi/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:13.413373 oresat_dxwifi-0.3.7/oresat_dxwifi/services/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/services/configs/camera_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/services/oresat_live.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:13.413373 oresat_dxwifi-0.3.7/oresat_dxwifi/services/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:13.413373 oresat_dxwifi-0.3.7/oresat_dxwifi/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/templates/oresat_live.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:13.413373 oresat_dxwifi-0.3.7/oresat_dxwifi/transmission/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/transmission/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:13.421373 oresat_dxwifi-0.3.7/oresat_dxwifi/transmission/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/transmission/configs/transmission_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/transmission/defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      661 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/transmission/startmonitor.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/transmission/transmission.py
--rw-r--r--   0 runner    (1001) docker     (127)  4381644 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/oresat_dxwifi/transmission/tx_module.so
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:01:13.421373 oresat_dxwifi-0.3.7/oresat_dxwifi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-27 06:01:13.000000 oresat_dxwifi-0.3.7/oresat_dxwifi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-27 06:01:13.000000 oresat_dxwifi-0.3.7/oresat_dxwifi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 06:01:13.000000 oresat_dxwifi-0.3.7/oresat_dxwifi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 06:01:13.000000 oresat_dxwifi-0.3.7/oresat_dxwifi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 06:01:13.000000 oresat_dxwifi-0.3.7/oresat_dxwifi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-27 06:01:13.000000 oresat_dxwifi-0.3.7/oresat_dxwifi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 06:01:13.421373 oresat_dxwifi-0.3.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      336 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/start-vcan
--rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-04-27 06:01:08.000000 oresat_dxwifi-0.3.7/startmonitor.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:34.578745 oresat_dxwifi-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:34.562745 oresat_dxwifi-0.3.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:34.566745 oresat_dxwifi-0.3.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-05-23 03:08:34.578745 oresat_dxwifi-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2384 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/build-deb.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:34.562745 oresat_dxwifi-0.3.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:34.570745 oresat_dxwifi-0.3.8/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   100917 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/docs/images/hgs-browser.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90640 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/docs/images/olaf-browser.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/kill-olaf
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat-dxwifi-software-server.service
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat-mon-iface.service
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat-vcan-iface.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:34.570745 oresat_dxwifi-0.3.8/oresat_dxwifi/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 03:08:34.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:34.570745 oresat_dxwifi-0.3.8/oresat_dxwifi/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/camera/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/camera/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/camera/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/camera/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:34.570745 oresat_dxwifi-0.3.8/oresat_dxwifi/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/resources/temperature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:34.570745 oresat_dxwifi-0.3.8/oresat_dxwifi/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:34.570745 oresat_dxwifi-0.3.8/oresat_dxwifi/services/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/services/configs/camera_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/services/oresat_live.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:34.570745 oresat_dxwifi-0.3.8/oresat_dxwifi/services/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:34.570745 oresat_dxwifi-0.3.8/oresat_dxwifi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/templates/oresat_live.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:34.574745 oresat_dxwifi-0.3.8/oresat_dxwifi/transmission/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/transmission/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:34.578745 oresat_dxwifi-0.3.8/oresat_dxwifi/transmission/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/transmission/configs/transmission_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/transmission/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      661 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/transmission/startmonitor.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/transmission/transmission.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4381644 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/oresat_dxwifi/transmission/tx_module.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:34.578745 oresat_dxwifi-0.3.8/oresat_dxwifi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-05-23 03:08:34.000000 oresat_dxwifi-0.3.8/oresat_dxwifi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-23 03:08:34.000000 oresat_dxwifi-0.3.8/oresat_dxwifi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 03:08:34.000000 oresat_dxwifi-0.3.8/oresat_dxwifi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-23 03:08:34.000000 oresat_dxwifi-0.3.8/oresat_dxwifi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-23 03:08:34.000000 oresat_dxwifi-0.3.8/oresat_dxwifi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-23 03:08:34.000000 oresat_dxwifi-0.3.8/oresat_dxwifi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 03:08:34.578745 oresat_dxwifi-0.3.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      336 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/start-vcan
+-rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-05-23 03:08:29.000000 oresat_dxwifi-0.3.8/startmonitor.sh
```

### Comparing `oresat_dxwifi-0.3.7/.github/workflows/pypi.yaml` & `oresat_dxwifi-0.3.8/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/.gitignore` & `oresat_dxwifi-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/LICENSE` & `oresat_dxwifi-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/PKG-INFO` & `oresat_dxwifi-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-dxwifi
-Version: 0.3.7
+Version: 0.3.8
 Summary: OreSat DxWiFi OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oresat_dxwifi-0.3.7/README.md` & `oresat_dxwifi-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/build-deb.sh` & `oresat_dxwifi-0.3.8/build-deb.sh`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/docs/images/hgs-browser.png` & `oresat_dxwifi-0.3.8/docs/images/hgs-browser.png`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/docs/images/olaf-browser.png` & `oresat_dxwifi-0.3.8/docs/images/olaf-browser.png`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi/__main__.py` & `oresat_dxwifi-0.3.8/oresat_dxwifi/__main__.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi/camera/CMakeLists.txt` & `oresat_dxwifi-0.3.8/oresat_dxwifi/camera/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi/camera/README.md` & `oresat_dxwifi-0.3.8/oresat_dxwifi/camera/README.md`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi/camera/frame.py` & `oresat_dxwifi-0.3.8/oresat_dxwifi/camera/frame.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi/camera/interface.py` & `oresat_dxwifi-0.3.8/oresat_dxwifi/camera/interface.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi/resources/temperature.py` & `oresat_dxwifi-0.3.8/oresat_dxwifi/resources/temperature.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi/services/oresat_live.py` & `oresat_dxwifi-0.3.8/oresat_dxwifi/services/oresat_live.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Oresat Live Camera Service"""
 
+import os
+import subprocess
+import time
 from enum import IntEnum
 from multiprocessing import Process
-import os, subprocess, time
 from yaml import safe_load
 
 from olaf import Service, logger
+
 from ..camera.interface import CameraInterface
 from ..transmission.transmission import Transmitter
 
 
 class State(IntEnum):
     OFF = 0
     BOOT = 1
@@ -47,19 +50,19 @@
     def __init__(self):
         """Initializes camera interface and sets state"""
         super().__init__()
         self.state = State.BOOT
 
         self.firmware_folder = "/lib/firmware/ath9k_htc"
         self.firmware_file = os.path.join(self.firmware_folder, "htc_9271-1.dev.0.fw")
-        
+
         self.IMAGE_OUPUT_DIRECTORY = "/oresat-live-output/frames"
 
         if not os.path.isdir(self.IMAGE_OUPUT_DIRECTORY):
-            os.mkdir(self.IMAGE_OUPUT_DIRECTORY)
+            os.makedirs(self.IMAGE_OUPUT_DIRECTORY, exist_ok=True)
 
         configs = self.load_configs()
 
         self.camera = CameraInterface(
             configs["width"],
             configs["height"],
             self.IMAGE_OUPUT_DIRECTORY,
@@ -95,42 +98,43 @@
 
         self.node.add_sdo_callbacks(
             self.STATE_INDEX,
             subindex=None,
             read_cb=self.on_state_read,
             write_cb=self.on_state_write,
         )
-        
+
         self.add_transmission_sdos()
 
     def add_transmission_sdos(self):
         self.node.add_sdo_callbacks(
             "transmission",
             subindex="bit_rate",
             read_cb=self.get_bit_rate,
             write_cb=self.update_bit_rate
         )
 
     def get_bit_rate(self):
         """returns the given bit rate of the transmission"""
         fw_file = subprocess.check_output(["readlink", self.firmware_file]).decode('ascii')
-        return int(fw_file.split(".")[0])
-    
+        fw_file = os.path.basename(fw_file)
+        return int(fw_file.split(".")[0].strip())
+
     def update_bit_rate(self, value: int):
         """Update the bit rate (by way of firmware blobs) of the transmission"""
         valid_rates = [1, 2, 5, 11, 12, 18, 36, 48, 54]
 
         if value not in valid_rates:
-            logger.warn(f"Bit rate of {value} is not valid. Valid Values: {valid_rates}")
+            logger.warning(f"Bit rate of {value} is not valid. Valid Values: {valid_rates}")
             return
 
         if self.get_bit_rate() == value:
             logger.info(f"Bit rate is already set to {value}")
             return
-        
+
         subprocess.call(["ln", "-sf", f"{value}.fw", self.firmware_file])
         subprocess.call(["rmmod", "ath9k_htc"])
         subprocess.call(["modprobe", "ath9k-htc"])
         time.sleep(2)
         self.start_monitor()
 
     def on_end(self) -> None:
```

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif` & `oresat_dxwifi-0.3.8/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi/templates/oresat_live.html` & `oresat_dxwifi-0.3.8/oresat_dxwifi/templates/oresat_live.html`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi/transmission/configs/transmission_configs.yaml` & `oresat_dxwifi-0.3.8/oresat_dxwifi/transmission/configs/transmission_configs.yaml`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi/transmission/defaults.py` & `oresat_dxwifi-0.3.8/oresat_dxwifi/transmission/defaults.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi/transmission/startmonitor.sh` & `oresat_dxwifi-0.3.8/oresat_dxwifi/transmission/startmonitor.sh`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi/transmission/transmission.py` & `oresat_dxwifi-0.3.8/oresat_dxwifi/transmission/transmission.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi/transmission/tx_module.so` & `oresat_dxwifi-0.3.8/oresat_dxwifi/transmission/tx_module.so`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi.egg-info/PKG-INFO` & `oresat_dxwifi-0.3.8/oresat_dxwifi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-dxwifi
-Version: 0.3.7
+Version: 0.3.8
 Summary: OreSat DxWiFi OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oresat_dxwifi-0.3.7/oresat_dxwifi.egg-info/SOURCES.txt` & `oresat_dxwifi-0.3.8/oresat_dxwifi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/pyproject.toml` & `oresat_dxwifi-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.7/startmonitor.sh` & `oresat_dxwifi-0.3.8/startmonitor.sh`

 * *Files identical despite different names*

