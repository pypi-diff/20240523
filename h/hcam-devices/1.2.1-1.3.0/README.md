# Comparing `tmp/hcam_devices-1.2.1.tar.gz` & `tmp/hcam_devices-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcam_devices-1.2.1.tar", last modified: Mon Jan 22 20:02:10 2024, max compression
+gzip compressed data, was "hcam_devices-1.3.0.tar", last modified: Thu May 23 11:51:42 2024, max compression
```

## Comparing `hcam_devices-1.2.1.tar` & `hcam_devices-1.3.0.tar`

### file list

```diff
@@ -1,76 +1,79 @@
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-01-22 20:02:10.188837 hcam_devices-1.2.1/
--rw-r--r--   0 sl         (501) staff       (20)      166 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/AUTHORS.rst
--rw-r--r--   0 sl         (501) staff       (20)     3303 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/CONTRIBUTING.rst
--rw-r--r--   0 sl         (501) staff       (20)       89 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/HISTORY.rst
--rw-r--r--   0 sl         (501) staff       (20)     1077 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/LICENSE
--rw-r--r--   0 sl         (501) staff       (20)      344 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/MANIFEST.in
--rw-r--r--   0 sl         (501) staff       (20)     5601 2024-01-22 20:02:10.188922 hcam_devices-1.2.1/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     4587 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/README.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-01-22 20:02:10.178212 hcam_devices-1.2.1/hcam_devices/
--rw-r--r--   0 sl         (501) staff       (20)       96 2024-01-22 19:50:54.000000 hcam_devices-1.2.1/hcam_devices/__init__.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-01-22 20:02:10.179223 hcam_devices-1.2.1/hcam_devices/components/
--rw-r--r--   0 sl         (501) staff       (20)     5938 2024-01-18 16:41:09.000000 hcam_devices-1.2.1/hcam_devices/components/__init__.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-01-22 20:02:10.181624 hcam_devices-1.2.1/hcam_devices/devices/
--rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/devices/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     3228 2023-07-21 10:44:48.000000 hcam_devices-1.2.1/hcam_devices/devices/honeywell.py
--rw-r--r--   0 sl         (501) staff       (20)     9262 2023-09-15 13:10:44.000000 hcam_devices-1.2.1/hcam_devices/devices/meerstetter.py
--rw-r--r--   0 sl         (501) staff       (20)    22137 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/devices/newport.py
--rw-r--r--   0 sl         (501) staff       (20)    11601 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/devices/ngc.py
--rw-r--r--   0 sl         (501) staff       (20)     5308 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/devices/pdr900.py
--rw-r--r--   0 sl         (501) staff       (20)     4293 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/devices/properties.py
--rw-r--r--   0 sl         (501) staff       (20)     4075 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/devices/unichiller.py
--rw-r--r--   0 sl         (501) staff       (20)     9216 2023-09-15 01:03:14.000000 hcam_devices-1.2.1/hcam_devices/devices/zaber.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-01-22 20:02:10.182250 hcam_devices-1.2.1/hcam_devices/gtc/
--rw-r--r--   0 sl         (501) staff       (20)     4824 2023-08-02 10:18:22.000000 hcam_devices-1.2.1/hcam_devices/gtc/corba.py
--rw-r--r--   0 sl         (501) staff       (20)     3063 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/gtc/headers.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-01-22 20:02:10.183551 hcam_devices-1.2.1/hcam_devices/machines/
--rw-r--r--   0 sl         (501) staff       (20)     1285 2024-01-22 19:50:15.000000 hcam_devices-1.2.1/hcam_devices/machines/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     1366 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/machines/connections.yaml
--rw-r--r--   0 sl         (501) staff       (20)     1736 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/machines/controller.yaml
--rw-r--r--   0 sl         (501) staff       (20)     4776 2023-08-02 10:18:22.000000 hcam_devices-1.2.1/hcam_devices/machines/gtc.yaml
--rw-r--r--   0 sl         (501) staff       (20)     4205 2023-11-05 20:14:29.000000 hcam_devices-1.2.1/hcam_devices/machines/motors.yaml
--rw-r--r--   0 sl         (501) staff       (20)     1252 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/machines/sensor.yaml
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-01-22 20:02:10.185597 hcam_devices-1.2.1/hcam_devices/models/
--rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/models/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     5001 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/models/ccd.py
--rw-r--r--   0 sl         (501) staff       (20)     7826 2023-09-15 01:05:00.000000 hcam_devices-1.2.1/hcam_devices/models/compo.py
--rw-r--r--   0 sl         (501) staff       (20)     2979 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/models/flow_sensor.py
--rw-r--r--   0 sl         (501) staff       (20)     6197 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/models/meerstetter.py
--rw-r--r--   0 sl         (501) staff       (20)     8967 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/models/ngc.py
--rw-r--r--   0 sl         (501) staff       (20)     1292 2024-01-18 16:41:09.000000 hcam_devices-1.2.1/hcam_devices/models/rack.py
--rw-r--r--   0 sl         (501) staff       (20)     7943 2023-09-15 00:57:07.000000 hcam_devices-1.2.1/hcam_devices/models/slide.py
--rw-r--r--   0 sl         (501) staff       (20)     9611 2024-01-12 12:37:00.000000 hcam_devices-1.2.1/hcam_devices/models/telescope.py
--rw-r--r--   0 sl         (501) staff       (20)     1952 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/models/vac_gauge.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-01-22 20:02:10.186277 hcam_devices-1.2.1/hcam_devices/testing/
--rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/testing/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     1227 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/testing/axis.py
--rw-r--r--   0 sl         (501) staff       (20)     2989 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/testing/fakeserial.py
--rw-r--r--   0 sl         (501) staff       (20)     2634 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/testing/properties.py
--rw-r--r--   0 sl         (501) staff       (20)     1051 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/testing/sensors.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-01-22 20:02:10.186647 hcam_devices-1.2.1/hcam_devices/utils/
--rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/utils/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     3334 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/utils/filesystem.py
--rw-r--r--   0 sl         (501) staff       (20)    13737 2023-07-27 22:31:34.000000 hcam_devices-1.2.1/hcam_devices/utils/obsmodes.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-01-22 20:02:10.186953 hcam_devices-1.2.1/hcam_devices/wamp/
--rw-r--r--   0 sl         (501) staff       (20)    10895 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/wamp/__init__.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-01-22 20:02:10.187135 hcam_devices-1.2.1/hcam_devices/wamp/utils/
--rw-r--r--   0 sl         (501) staff       (20)     2708 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/hcam_devices/wamp/utils/__init__.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-01-22 20:02:10.179091 hcam_devices-1.2.1/hcam_devices.egg-info/
--rw-r--r--   0 sl         (501) staff       (20)     5601 2024-01-22 20:02:10.000000 hcam_devices-1.2.1/hcam_devices.egg-info/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     1739 2024-01-22 20:02:10.000000 hcam_devices-1.2.1/hcam_devices.egg-info/SOURCES.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2024-01-22 20:02:10.000000 hcam_devices-1.2.1/hcam_devices.egg-info/dependency_links.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2024-01-22 20:02:10.000000 hcam_devices-1.2.1/hcam_devices.egg-info/not-zip-safe
--rw-r--r--   0 sl         (501) staff       (20)      153 2024-01-22 20:02:10.000000 hcam_devices-1.2.1/hcam_devices.egg-info/requires.txt
--rw-r--r--   0 sl         (501) staff       (20)       13 2024-01-22 20:02:10.000000 hcam_devices-1.2.1/hcam_devices.egg-info/top_level.txt
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-01-22 20:02:10.188721 hcam_devices-1.2.1/scripts/
--rw-r--r--   0 sl         (501) staff       (20)     1784 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/scripts/do_wamp_call
--rw-r--r--   0 sl         (501) staff       (20)      760 2023-07-21 10:44:48.000000 hcam_devices-1.2.1/scripts/gtcserver
--rwxr-xr-x   0 sl         (501) staff       (20)      701 2023-07-21 10:44:48.000000 hcam_devices-1.2.1/scripts/hserver
--rwxr-xr-x   0 sl         (501) staff       (20)     7557 2024-01-18 16:41:09.000000 hcam_devices-1.2.1/scripts/hwlogger
--rwxr-xr-x   0 sl         (501) staff       (20)     6207 2024-01-18 16:41:09.000000 hcam_devices-1.2.1/scripts/hwserver
--rw-r--r--   0 sl         (501) staff       (20)      479 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/scripts/make_diagrams.py
--rw-r--r--   0 sl         (501) staff       (20)     1065 2023-07-21 10:44:48.000000 hcam_devices-1.2.1/scripts/show_telemetry
--rw-r--r--   0 sl         (501) staff       (20)     7513 2022-10-19 13:15:14.000000 hcam_devices-1.2.1/scripts/tcp_serial_bridge
--rw-r--r--   0 sl         (501) staff       (20)      535 2023-07-21 10:44:48.000000 hcam_devices-1.2.1/scripts/zaber_ascii
--rw-r--r--   0 sl         (501) staff       (20)      313 2024-01-22 20:02:10.189151 hcam_devices-1.2.1/setup.cfg
--rw-r--r--   0 sl         (501) staff       (20)     2512 2024-01-22 19:50:54.000000 hcam_devices-1.2.1/setup.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-05-23 11:51:42.628443 hcam_devices-1.3.0/
+-rw-r--r--   0 sl         (501) staff       (20)      166 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/AUTHORS.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3303 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 sl         (501) staff       (20)       89 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/HISTORY.rst
+-rw-r--r--   0 sl         (501) staff       (20)     1077 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/LICENSE
+-rw-r--r--   0 sl         (501) staff       (20)      344 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/MANIFEST.in
+-rw-r--r--   0 sl         (501) staff       (20)     5601 2024-05-23 11:51:42.628505 hcam_devices-1.3.0/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     4587 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/README.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-05-23 11:51:42.618998 hcam_devices-1.3.0/hcam_devices/
+-rw-r--r--   0 sl         (501) staff       (20)       96 2024-05-23 11:51:04.000000 hcam_devices-1.3.0/hcam_devices/__init__.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-05-23 11:51:42.619871 hcam_devices-1.3.0/hcam_devices/components/
+-rw-r--r--   0 sl         (501) staff       (20)     6818 2024-04-17 09:17:31.000000 hcam_devices-1.3.0/hcam_devices/components/__init__.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-05-23 11:51:42.621981 hcam_devices-1.3.0/hcam_devices/devices/
+-rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/devices/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     3228 2023-07-21 10:44:48.000000 hcam_devices-1.3.0/hcam_devices/devices/honeywell.py
+-rw-r--r--   0 sl         (501) staff       (20)     9262 2023-09-15 13:10:44.000000 hcam_devices-1.3.0/hcam_devices/devices/meerstetter.py
+-rw-r--r--   0 sl         (501) staff       (20)    22137 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/devices/newport.py
+-rw-r--r--   0 sl         (501) staff       (20)    11601 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/devices/ngc.py
+-rw-r--r--   0 sl         (501) staff       (20)     5308 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/devices/pdr900.py
+-rw-r--r--   0 sl         (501) staff       (20)     4293 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/devices/properties.py
+-rw-r--r--   0 sl         (501) staff       (20)     4075 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/devices/unichiller.py
+-rw-r--r--   0 sl         (501) staff       (20)     9216 2023-09-15 01:03:14.000000 hcam_devices-1.3.0/hcam_devices/devices/zaber.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-05-23 11:51:42.622391 hcam_devices-1.3.0/hcam_devices/gtc/
+-rw-r--r--   0 sl         (501) staff       (20)     4824 2023-08-02 10:18:22.000000 hcam_devices-1.3.0/hcam_devices/gtc/corba.py
+-rw-r--r--   0 sl         (501) staff       (20)     3063 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/gtc/headers.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-05-23 11:51:42.623384 hcam_devices-1.3.0/hcam_devices/machines/
+-rw-r--r--   0 sl         (501) staff       (20)     1285 2024-01-22 19:50:15.000000 hcam_devices-1.3.0/hcam_devices/machines/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     1366 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/machines/connections.yaml
+-rw-r--r--   0 sl         (501) staff       (20)     1736 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/machines/controller.yaml
+-rw-r--r--   0 sl         (501) staff       (20)     4776 2023-08-02 10:18:22.000000 hcam_devices-1.3.0/hcam_devices/machines/gtc.yaml
+-rw-r--r--   0 sl         (501) staff       (20)     4298 2024-03-05 14:26:52.000000 hcam_devices-1.3.0/hcam_devices/machines/motors.yaml
+-rw-r--r--   0 sl         (501) staff       (20)     1252 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/machines/sensor.yaml
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-05-23 11:51:42.625306 hcam_devices-1.3.0/hcam_devices/models/
+-rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/models/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     5001 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/models/ccd.py
+-rw-r--r--   0 sl         (501) staff       (20)     7826 2023-09-15 01:05:00.000000 hcam_devices-1.3.0/hcam_devices/models/compo.py
+-rw-r--r--   0 sl         (501) staff       (20)     2979 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/models/flow_sensor.py
+-rw-r--r--   0 sl         (501) staff       (20)     4095 2024-04-17 08:32:59.000000 hcam_devices-1.3.0/hcam_devices/models/gps.py
+-rw-r--r--   0 sl         (501) staff       (20)     1573 2024-04-17 11:37:58.000000 hcam_devices-1.3.0/hcam_devices/models/gtc_cooling.py
+-rw-r--r--   0 sl         (501) staff       (20)     6197 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/models/meerstetter.py
+-rw-r--r--   0 sl         (501) staff       (20)     9072 2024-05-23 11:48:52.000000 hcam_devices-1.3.0/hcam_devices/models/ngc.py
+-rw-r--r--   0 sl         (501) staff       (20)     1787 2024-04-17 08:12:54.000000 hcam_devices-1.3.0/hcam_devices/models/rack.py
+-rw-r--r--   0 sl         (501) staff       (20)     7943 2023-09-15 00:57:07.000000 hcam_devices-1.3.0/hcam_devices/models/slide.py
+-rw-r--r--   0 sl         (501) staff       (20)     9655 2024-05-20 12:18:07.000000 hcam_devices-1.3.0/hcam_devices/models/telescope.py
+-rw-r--r--   0 sl         (501) staff       (20)     1952 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/models/vac_gauge.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-05-23 11:51:42.625904 hcam_devices-1.3.0/hcam_devices/testing/
+-rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/testing/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     1227 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/testing/axis.py
+-rw-r--r--   0 sl         (501) staff       (20)     2989 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/testing/fakeserial.py
+-rw-r--r--   0 sl         (501) staff       (20)     2634 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/testing/properties.py
+-rw-r--r--   0 sl         (501) staff       (20)     1051 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/testing/sensors.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-05-23 11:51:42.626271 hcam_devices-1.3.0/hcam_devices/utils/
+-rw-r--r--   0 sl         (501) staff       (20)        0 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/utils/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     3334 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/utils/filesystem.py
+-rw-r--r--   0 sl         (501) staff       (20)    13737 2023-07-27 22:31:34.000000 hcam_devices-1.3.0/hcam_devices/utils/obsmodes.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-05-23 11:51:42.626545 hcam_devices-1.3.0/hcam_devices/wamp/
+-rw-r--r--   0 sl         (501) staff       (20)    11388 2024-04-17 08:32:38.000000 hcam_devices-1.3.0/hcam_devices/wamp/__init__.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-05-23 11:51:42.626774 hcam_devices-1.3.0/hcam_devices/wamp/utils/
+-rw-r--r--   0 sl         (501) staff       (20)     2708 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/hcam_devices/wamp/utils/__init__.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-05-23 11:51:42.619714 hcam_devices-1.3.0/hcam_devices.egg-info/
+-rw-r--r--   0 sl         (501) staff       (20)     5601 2024-05-23 11:51:42.000000 hcam_devices-1.3.0/hcam_devices.egg-info/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     1828 2024-05-23 11:51:42.000000 hcam_devices-1.3.0/hcam_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2024-05-23 11:51:42.000000 hcam_devices-1.3.0/hcam_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2024-05-23 11:51:42.000000 hcam_devices-1.3.0/hcam_devices.egg-info/not-zip-safe
+-rw-r--r--   0 sl         (501) staff       (20)      153 2024-05-23 11:51:42.000000 hcam_devices-1.3.0/hcam_devices.egg-info/requires.txt
+-rw-r--r--   0 sl         (501) staff       (20)       13 2024-05-23 11:51:42.000000 hcam_devices-1.3.0/hcam_devices.egg-info/top_level.txt
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-05-23 11:51:42.628340 hcam_devices-1.3.0/scripts/
+-rw-r--r--   0 sl         (501) staff       (20)     1784 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/scripts/do_wamp_call
+-rw-r--r--   0 sl         (501) staff       (20)      520 2024-03-07 12:33:21.000000 hcam_devices-1.3.0/scripts/gtc_archive_ingest
+-rw-r--r--   0 sl         (501) staff       (20)      760 2023-07-21 10:44:48.000000 hcam_devices-1.3.0/scripts/gtcserver
+-rwxr-xr-x   0 sl         (501) staff       (20)      701 2023-07-21 10:44:48.000000 hcam_devices-1.3.0/scripts/hserver
+-rwxr-xr-x   0 sl         (501) staff       (20)     9749 2024-05-20 13:29:03.000000 hcam_devices-1.3.0/scripts/hwlogger
+-rwxr-xr-x   0 sl         (501) staff       (20)     6585 2024-04-17 09:17:22.000000 hcam_devices-1.3.0/scripts/hwserver
+-rw-r--r--   0 sl         (501) staff       (20)      479 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/scripts/make_diagrams.py
+-rw-r--r--   0 sl         (501) staff       (20)     1065 2023-07-21 10:44:48.000000 hcam_devices-1.3.0/scripts/show_telemetry
+-rw-r--r--   0 sl         (501) staff       (20)     7513 2022-10-19 13:15:14.000000 hcam_devices-1.3.0/scripts/tcp_serial_bridge
+-rw-r--r--   0 sl         (501) staff       (20)      535 2023-07-21 10:44:48.000000 hcam_devices-1.3.0/scripts/zaber_ascii
+-rw-r--r--   0 sl         (501) staff       (20)      313 2024-05-23 11:51:42.628702 hcam_devices-1.3.0/setup.cfg
+-rw-r--r--   0 sl         (501) staff       (20)     2512 2024-05-23 11:51:04.000000 hcam_devices-1.3.0/setup.py
```

### Comparing `hcam_devices-1.2.1/CONTRIBUTING.rst` & `hcam_devices-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/LICENSE` & `hcam_devices-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/PKG-INFO` & `hcam_devices-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hcam_devices
-Version: 1.2.1
+Version: 1.3.0
 Summary: Device Communication via WAMP for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_devices
-Download-URL: https://github.com/HiPERCAM/hcam_devices/archive/v1.2.1.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_devices/archive/v1.3.0.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_devices
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_devices-1.2.1/README.rst` & `hcam_devices-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/components/__init__.py` & `hcam_devices-1.3.0/hcam_devices/components/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,38 @@
 from ..models.compo import Compo, CompoArms, CompoLens
 from ..models.meerstetter import Meerstetter
 from ..models.vac_gauge import VacGauge
 from ..models.ccd import CCDHead
 from ..models.ngc import NGC
 from ..models.telescope import GTC
 from ..models.rack import Rack
+from ..models.gps import GPS
+from ..models.gtc_cooling import GTCCooler
+
+
+class GTCCoolingComponent(ModelComponentMixin):
+    def __init__(self, config):
+        self._component_name = config.extra.get(
+            "name", str(self.__class__).replace("Component", "")
+        ).lower()
+        super(GTCCoolingComponent, self).__init__(config)
+        self.traceback_app = True
+        emulation_mode = config.extra.get("emulate")
+        self.model = GTCCooler(emulate=emulation_mode)
+
+
+class GPSComponent(ModelComponentMixin):
+    def __init__(self, config):
+        self._component_name = config.extra.get(
+            "name", str(self.__class__).replace("Component", "")
+        ).lower()
+        super(GPSComponent, self).__init__(config)
+        self.traceback_app = True
+        emulation_mode = config.extra.get("emulate")
+        self.model = GPS(emulate=emulation_mode)
 
 
 class RackComponent(ModelComponentMixin):
     def __init__(self, config):
         self._component_name = config.extra.get(
             "name", str(self.__class__).replace("Component", "")
         ).lower()
```

### Comparing `hcam_devices-1.2.1/hcam_devices/devices/honeywell.py` & `hcam_devices-1.3.0/hcam_devices/devices/honeywell.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/devices/meerstetter.py` & `hcam_devices-1.3.0/hcam_devices/devices/meerstetter.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/devices/newport.py` & `hcam_devices-1.3.0/hcam_devices/devices/newport.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/devices/ngc.py` & `hcam_devices-1.3.0/hcam_devices/devices/ngc.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/devices/pdr900.py` & `hcam_devices-1.3.0/hcam_devices/devices/pdr900.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/devices/properties.py` & `hcam_devices-1.3.0/hcam_devices/devices/properties.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/devices/unichiller.py` & `hcam_devices-1.3.0/hcam_devices/devices/unichiller.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/devices/zaber.py` & `hcam_devices-1.3.0/hcam_devices/devices/zaber.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/gtc/corba.py` & `hcam_devices-1.3.0/hcam_devices/gtc/corba.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/gtc/headers.py` & `hcam_devices-1.3.0/hcam_devices/gtc/headers.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/machines/__init__.py` & `hcam_devices-1.3.0/hcam_devices/machines/__init__.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/machines/connections.yaml` & `hcam_devices-1.3.0/hcam_devices/machines/connections.yaml`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/machines/controller.yaml` & `hcam_devices-1.3.0/hcam_devices/machines/controller.yaml`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/machines/gtc.yaml` & `hcam_devices-1.3.0/hcam_devices/machines/gtc.yaml`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/machines/motors.yaml` & `hcam_devices-1.3.0/hcam_devices/machines/motors.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -75,24 +75,25 @@
                   - name: inpos
                     on entry: |
                       current = target
                     transitions:
                       - target: outpos
                         event: positionSet
                         action: target = event.position
+                        guard: event.position != current
+                        # dummy transition back to ourselves if we get a move command
+                      - target: inpos
+                        event: move
                   - name: outpos
                     transitions:
                       - target: moving
                         event: move
                         guard: device.move(target)
                         action: |
                           moving = True
-                      - target: inpos
-                        priority: 1
-                        guard: device.on_target()
                   - name: moving
                     transitions:
                       - target: moving
                         guard: after(poll_time)
                         action: |
                           try:
                               current, moving = device.poll()
```

### Comparing `hcam_devices-1.2.1/hcam_devices/machines/sensor.yaml` & `hcam_devices-1.3.0/hcam_devices/machines/sensor.yaml`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/models/ccd.py` & `hcam_devices-1.3.0/hcam_devices/models/ccd.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/models/compo.py` & `hcam_devices-1.3.0/hcam_devices/models/compo.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/models/flow_sensor.py` & `hcam_devices-1.3.0/hcam_devices/models/flow_sensor.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/models/meerstetter.py` & `hcam_devices-1.3.0/hcam_devices/models/meerstetter.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/models/ngc.py` & `hcam_devices-1.3.0/hcam_devices/models/ngc.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,20 +81,22 @@
             return False
 
         for key in output:
             msg = output[key]
             self.log.info("cmd {}: {}".format(key, msg))
         return True
 
-    def start_ngc_server(self):
+    def start_ngc_server(self, gui=False):
         """
         Run commands necessary to bring up the ESO NGC server
         """
         try:
-            output = self._dev.start_ngc_sw()
+            # wamp calls supply args as str, so force type
+            gui = bool(gui)
+            output = self._dev.start_ngc_sw(gui=gui)
         except Exception as e:
             self.log.error('could not start NGC software: ' + str(e))
             return False
 
         for key in output:
             msg = output[key]
             self.log.info("cmd {}: {}".format(key, msg))
```

### Comparing `hcam_devices-1.2.1/hcam_devices/models/rack.py` & `hcam_devices-1.3.0/hcam_devices/models/rack.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,45 +8,64 @@
     TelescopeServer = None
 
 
 class FakeServer(object):
     def getCabinetTemperature1(self):
         return 20.0
 
+    def getCabinetTemperature2(self):
+        return 21.0
+
     def getCabinetTemperature3(self):
         return 22.0
 
 
 class Rack(object):
     # add any extra methods you want exposed here
     extra_rpc_calls = ()
     log = Logger()
     settable_attributes = ()
 
     def __init__(self, emulate=True):
         print("emulation mode: ", emulate)
-        if emulate:
-            self._server = FakeServer()
-        else:
-            self._server = TelescopeServer()
+        self.emulate = emulate
+        self.try_connect()
 
         # no state machine needed
         self.machines = {}
 
+    def try_connect(self):
+        try:
+            if self.emulate:
+                self._server = FakeServer()
+            else:
+                self._server = TelescopeServer()
+        except:
+            self._server = None
+            return False
+        return True
+
+    def disconnect(self):
+        self._server = None
+
     def telemetry(self):
         """
         Called periodically to provide a telemetry package
         """
         ts = Time.now()
         try:
             temp_top = self._server.getCabinetTemperature1()
+            temp_middle = self._server.getCabinetTemperature2()
             temp_bottom = self._server.getCabinetTemperature3()
         except Exception:
             temp_bottom = None
+            temp_middle = None
             temp_top = None
+            self.try_connect()
 
         return dict(
             timestamp=ts,
             rack_temp_bottom=temp_bottom,
+            rack_temp_middle=temp_middle,
             rack_temp_top=temp_top,
             state={},
         )
```

### Comparing `hcam_devices-1.2.1/hcam_devices/models/slide.py` & `hcam_devices-1.3.0/hcam_devices/models/slide.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/models/telescope.py` & `hcam_devices-1.3.0/hcam_devices/models/telescope.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     def getTelescopeParams(self):
         hdr = Header()
         hdr["RADEG"] = (self.ra, "RA (degrees)")
         hdr["DECDEG"] = (self.dec, "DEC (degrees)")
         hdr["INSTRPA"] = (22.1, "Rotator PA")
         hdr["ROTATOR"] = (200.1, "Rotator MA")
         hdr["M2UZ"] = (self.focus, "Focus offset")
+        hdr["LST"] = (2.3, "Sidereal Time")
         return hdr.tostring(sep=";").split(";")[:-1]
 
     @property
     def focus(self):
         # fix so focus changes take 1s for 0.05mm changes
         required_time = abs(self.focus_offset / 0.05)
         if (time.time() - self._last_focus) > required_time:
```

### Comparing `hcam_devices-1.2.1/hcam_devices/models/vac_gauge.py` & `hcam_devices-1.3.0/hcam_devices/models/vac_gauge.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/testing/axis.py` & `hcam_devices-1.3.0/hcam_devices/testing/axis.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/testing/fakeserial.py` & `hcam_devices-1.3.0/hcam_devices/testing/fakeserial.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/testing/properties.py` & `hcam_devices-1.3.0/hcam_devices/testing/properties.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/testing/sensors.py` & `hcam_devices-1.3.0/hcam_devices/testing/sensors.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/utils/filesystem.py` & `hcam_devices-1.3.0/hcam_devices/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/utils/obsmodes.py` & `hcam_devices-1.3.0/hcam_devices/utils/obsmodes.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices/wamp/__init__.py` & `hcam_devices-1.3.0/hcam_devices/wamp/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,106 +6,118 @@
 from twisted.internet.defer import inlineCallbacks
 from twisted.internet.task import LoopingCall
 from twisted.internet import reactor
 from twisted.logger import Logger
 from twisted.internet.error import ReactorNotRunning
 
 
-@wamp.error(u"com.hipercam.runtimeerror")
+@wamp.error("com.hipercam.runtimeerror")
 class HipercamRuntimeError(Exception):
     """
     An application specific exception that is decorated with a WAMP URI,
     and hence can be automapped by Autobahn.
     """
+
     pass
 
 
 TELEMETRY_DELAY = 2
 HEARTBEAT_DELAY = 300
 
 
 class WrapperComponentMixin(ApplicationSession):
     """
     A mixin class for a WAMP component that wraps others.
     """
+
     log = Logger()
 
     def onUserError(self, fail, msg):
         self.log.error(msg)
 
     @inlineCallbacks
     def onJoin(self, details):
 
-        self.telemetry_topic = 'hipercam.{}.telemetry'.format(self._component_name)
+        self.telemetry_topic = "hipercam.{}.telemetry".format(self._component_name)
 
-        self.log.info("{} joined WAMP session: realm={}, session={}".format(
-            self._component_name, details.realm, details.session
-        ))
+        self.log.info(
+            "{} joined WAMP session: realm={}, session={}".format(
+                self._component_name, details.realm, details.session
+            )
+        )
 
         def make_pass_through(to_topic):
             def inner(*args):
                 self.publish(to_topic, *args)
+
             return inner
 
         # pass through topics
         for name in self.model.pass_through_topics:
-            topic = 'hipercam.{}.{}'.format(
-                self._component_name, name
-            )
+            topic = "hipercam.{}.{}".format(self._component_name, name)
             to_topic = self.model.pass_through_topics[name]
             yield self.subscribe(make_pass_through(to_topic), topic)
-            self.log.info('{} is passing messages on {} to {}'.format(
-                self._component_name, topic, to_topic
-            ))
+            self.log.info(
+                "{} is passing messages on {} to {}".format(
+                    self._component_name, topic, to_topic
+                )
+            )
 
         # subscribe to all the telemetry channels
         for channel_id in self.model.subscribed_channels:
             channel = self.model.subscribed_channels[channel_id]
-            topic = channel + '.telemetry'
+            topic = channel + ".telemetry"
             yield self.subscribe(self.model.on_received_telemetry, topic)
-            self.log.info("{} subscribed to topic {}".format(
-                self._component_name, topic)
+            self.log.info(
+                "{} subscribed to topic {}".format(self._component_name, topic)
             )
 
         # install a heartbeat logger
         self._tick_no = 0
         self._tick_loop = LoopingCall(self._tick)
         self._tick_loop.start(HEARTBEAT_DELAY)
 
         # begin publishing telemetry
         self._telemetry_publisher = LoopingCall(self._publish_telemetry)
         self._telemetry_publisher.start(TELEMETRY_DELAY)
-        self.log.info("{} started publishing telemetry on topic {}".format(self._component_name, self.telemetry_topic))
+        self.log.info(
+            "{} started publishing telemetry on topic {}".format(
+                self._component_name, self.telemetry_topic
+            )
+        )
 
     def _tick(self):
         self._tick_no += 1
-        self.log.info('{} is alive [tick {}]'.format(
-            self._component_name, self._tick_no))
+        self.log.info(
+            "{} is alive [tick {}]".format(self._component_name, self._tick_no)
+        )
 
     @inlineCallbacks
     def _publish_telemetry(self):
-        pub_options = PublishOptions(
-            acknowledge=True,
-            exclude_me=True
-        )
+        pub_options = PublishOptions(acknowledge=True, exclude_me=True)
         package = pickle.dumps(self.model.telemetry())
-        publication = yield self.publish(self.telemetry_topic, package, options=pub_options)
-        self.log.debug("Published telemetry to {} with publication ID {}".format(
-            self.telemetry_topic, publication.id))
+        publication = yield self.publish(
+            self.telemetry_topic, package, options=pub_options
+        )
+        self.log.debug(
+            "Published telemetry to {} with publication ID {}".format(
+                self.telemetry_topic, publication.id
+            )
+        )
 
     def onLeave(self, details):
         self.log.info("Session closed: {details}", details=details)
         self.disconnect()
 
     def onDisconnect(self):
         self.log.info("Connection closed")
-        if hasattr(self, '_tick_loop') and self._tick_loop:
+        if hasattr(self, "_tick_loop") and self._tick_loop:
             self._tick_loop.stop()
             self._tick_loop = None
-        if hasattr(self, '_telemetry_publisher') and self._telemetry_publisher:
+        if hasattr(self, "_telemetry_publisher") and self._telemetry_publisher:
             self._telemetry_publisher.stop()
             self._telemetry_publisher = None
         try:
             reactor.stop()
         except ReactorNotRunning:
             pass
 
@@ -117,110 +129,130 @@
     Telemetry is regularly published, and a tick is published regularly
     to check if the component is alive.
 
     In addition, the component subscribes to topics for each settable
     attribute of the model, and registers RPC calls for any defined
     methods on the model, and all state transitions of the model.
     """
+
     log = Logger()
 
     def onUserError(self, fail, msg):
         self.log.error(msg)
 
     @inlineCallbacks
     def onJoin(self, details):
 
-        self.telemetry_topic = 'hipercam.{}.telemetry'.format(self._component_name)
+        self.telemetry_topic = "hipercam.{}.telemetry".format(self._component_name)
 
-        self.log.info("{} joined WAMP session: realm={}, session={}".format(
-            self._component_name, details.realm, details.session
-        ))
+        self.log.info(
+            "{} joined WAMP session: realm={}, session={}".format(
+                self._component_name, details.realm, details.session
+            )
+        )
 
         # start a looping call step state machines on
         # needs to be on a tigher loop than poll times in the machines,
         # of order 1s. Since there are many machines in a model,
         # we work out the loop time here
         nmachines = len(self.model.machines)
         if nmachines > 0:
-            loop_time = 0.3/nmachines
+            loop_time = 0.3 / nmachines
             self._machine_loop = LoopingCall(self._forward_step_statemachines)
             self._machine_loop.start(loop_time)
 
         # add any Looping calls defined in the model
         self._model_looping_calls = []
-        if hasattr(self.model, 'extra_looping_calls'):
+        if hasattr(self.model, "extra_looping_calls"):
             for call in self.model.extra_looping_calls:
                 interval = self.model.extra_looping_calls[call]
                 function = getattr(self.model, call)
                 loop = LoopingCall(function)
                 self._model_looping_calls.append(loop)
                 loop.start(interval)
 
         # register all triggers of state transistions as RPC callbacks
         def make_trigger(machine, event):
             # use this factory function to avoid statemachine
             # being returned from trigger (it cannot be pickled)
             def f(**event_parameters):
                 allowed_events = machine.statechart.events_for(machine.configuration)
                 if event not in allowed_events:
-                    raise HipercamRuntimeError('unsupported state transition on {}\n{} not in {}'.format(
-                                        self._component_name, event, ",".join(allowed_events)
-                                    ))
+                    raise HipercamRuntimeError(
+                        "unsupported state transition on {}\n{} not in {}".format(
+                            self._component_name, event, ",".join(allowed_events)
+                        )
+                    )
                 machine.queue(event, **event_parameters)
+
             return f
 
         for machine_name in self.model.machines:
-            self.log.info('registering state transition triggers')
+            self.log.info("registering state transition triggers")
             machine = self.model.machines[machine_name]
             events = machine.statechart.events_for()
-            self.log.info('registering {} for {}'.format(events, machine_name))
+            self.log.info("registering {} for {}".format(events, machine_name))
             for event in events:
-                rpc_name = 'hipercam.{}.rpc.{}.{}'.format(
+                rpc_name = "hipercam.{}.rpc.{}.{}".format(
                     self._component_name, machine_name, event
                 )
                 trigger = make_trigger(machine, event)
                 yield self.register(trigger, rpc_name)
-                self.log.info("{} registered procedure {}".format(self._component_name, rpc_name))
+                self.log.info(
+                    "{} registered procedure {}".format(self._component_name, rpc_name)
+                )
 
         # add additional RPC calls
         for method_name in self.model.extra_rpc_calls:
             trigger_function = getattr(self.model, method_name)
-            rpc_name = 'hipercam.{}.rpc.{}'.format(
-                self._component_name, method_name
-            )
+            rpc_name = "hipercam.{}.rpc.{}".format(self._component_name, method_name)
             yield self.register(trigger_function, rpc_name)
-            self.log.info("{} registered procedure {}".format(self._component_name, rpc_name))
+            self.log.info(
+                "{} registered procedure {}".format(self._component_name, rpc_name)
+            )
 
         # subscribe to channels corresponding to settable attributes
 
         # needs a factory function because of scopes
         # see https://eev.ee/blog/2011/04/24/gotcha-python-scoping-closures/
         def make_setter(attr):
             def setter(val):
                 setattr(self.model, attr, val)
+
             return setter
 
         for i in range(len(self.model.settable_attributes)):
             # declared inside loop so it has proper scope for capture in callback
             attr = str(self.model.settable_attributes[i])
-            topic = 'hipercam.{}.{}'.format(
-                self._component_name, attr
-            )
+            topic = "hipercam.{}.{}".format(self._component_name, attr)
             yield self.subscribe(make_setter(attr), topic)
-            self.log.info("{} registered settable attribute {} on topic {}".format(self._component_name, attr, topic))
+            self.log.info(
+                "{} registered settable attribute {} on topic {}".format(
+                    self._component_name, attr, topic
+                )
+            )
 
         # install a heartbeat logger
         self._tick_no = 0
         self._tick_loop = LoopingCall(self._tick)
         self._tick_loop.start(HEARTBEAT_DELAY)
 
         # begin publishing telemetry
         self._telemetry_publisher = LoopingCall(self._publish_telemetry)
-        self._telemetry_publisher.start(TELEMETRY_DELAY)
-        self.log.info("{} started publishing telemetry on topic {}".format(self._component_name, self.telemetry_topic))
+        delay = (
+            self.model.telemetry_delay
+            if hasattr(self.model, "telemetry_delay")
+            else TELEMETRY_DELAY
+        )
+        self._telemetry_publisher.start(delay)
+        self.log.info(
+            "{} started publishing telemetry on topic {}".format(
+                self._component_name, self.telemetry_topic
+            )
+        )
 
     def _forward_step_statemachines(self):
         """
         Step each state machine in the model forward.
 
         Needs to be on a tight control loop, because if this loops
         slower than poll times in the state machines, unusual
@@ -235,44 +267,47 @@
         """
         for machine_name in self.model.machines:
             machine = self.model.machines[machine_name]
             machine.execute()
 
     def _tick(self):
         self._tick_no += 1
-        self.log.info('{} is alive [tick {}]'.format(
-            self._component_name, self._tick_no))
+        self.log.info(
+            "{} is alive [tick {}]".format(self._component_name, self._tick_no)
+        )
 
     @inlineCallbacks
     def _publish_telemetry(self):
-        pub_options = PublishOptions(
-            acknowledge=True,
-            exclude_me=True
-        )
+        pub_options = PublishOptions(acknowledge=True, exclude_me=True)
         package = pickle.dumps(self.model.telemetry())
-        publication = yield self.publish(self.telemetry_topic, package, options=pub_options)
-        self.log.debug("Published telemetry to {} with publication ID {}".format(
-            self.telemetry_topic, publication.id))
+        publication = yield self.publish(
+            self.telemetry_topic, package, options=pub_options
+        )
+        self.log.debug(
+            "Published telemetry to {} with publication ID {}".format(
+                self.telemetry_topic, publication.id
+            )
+        )
 
     def onLeave(self, details):
         self.log.info("Session closed: {details}", details=details)
         self.disconnect()
 
     def onDisconnect(self):
         self.log.info("Connection closed")
-        if hasattr(self, '_model_looping_calls') and self._model_looping_calls:
+        if hasattr(self, "_model_looping_calls") and self._model_looping_calls:
             for call in self._model_looping_calls:
                 call.stop()
             self._model_looping_calls = None
-        if hasattr(self, '_tick_loop') and self._tick_loop:
+        if hasattr(self, "_tick_loop") and self._tick_loop:
             self._tick_loop.stop()
             self._tick_loop = None
-        if hasattr(self, '_telemetry_publisher') and self._telemetry_publisher:
+        if hasattr(self, "_telemetry_publisher") and self._telemetry_publisher:
             self._telemetry_publisher.stop()
             self._telemetry_publisher = None
-        if hasattr(self, '_machine_loop') and self._machine_loop:
+        if hasattr(self, "_machine_loop") and self._machine_loop:
             self._machine_loop.stop()
             self._machine_loop = None
         try:
             reactor.stop()
         except ReactorNotRunning:
             pass
```

### Comparing `hcam_devices-1.2.1/hcam_devices/wamp/utils/__init__.py` & `hcam_devices-1.3.0/hcam_devices/wamp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/hcam_devices.egg-info/PKG-INFO` & `hcam_devices-1.3.0/hcam_devices.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hcam-devices
-Version: 1.2.1
+Version: 1.3.0
 Summary: Device Communication via WAMP for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_devices
-Download-URL: https://github.com/HiPERCAM/hcam_devices/archive/v1.2.1.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_devices/archive/v1.3.0.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_devices
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_devices-1.2.1/hcam_devices.egg-info/SOURCES.txt` & `hcam_devices-1.3.0/hcam_devices.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 hcam_devices/machines/gtc.yaml
 hcam_devices/machines/motors.yaml
 hcam_devices/machines/sensor.yaml
 hcam_devices/models/__init__.py
 hcam_devices/models/ccd.py
 hcam_devices/models/compo.py
 hcam_devices/models/flow_sensor.py
+hcam_devices/models/gps.py
+hcam_devices/models/gtc_cooling.py
 hcam_devices/models/meerstetter.py
 hcam_devices/models/ngc.py
 hcam_devices/models/rack.py
 hcam_devices/models/slide.py
 hcam_devices/models/telescope.py
 hcam_devices/models/vac_gauge.py
 hcam_devices/testing/__init__.py
@@ -48,14 +50,15 @@
 hcam_devices/testing/sensors.py
 hcam_devices/utils/__init__.py
 hcam_devices/utils/filesystem.py
 hcam_devices/utils/obsmodes.py
 hcam_devices/wamp/__init__.py
 hcam_devices/wamp/utils/__init__.py
 scripts/do_wamp_call
+scripts/gtc_archive_ingest
 scripts/gtcserver
 scripts/hserver
 scripts/hwlogger
 scripts/hwserver
 scripts/make_diagrams.py
 scripts/show_telemetry
 scripts/tcp_serial_bridge
```

### Comparing `hcam_devices-1.2.1/scripts/do_wamp_call` & `hcam_devices-1.3.0/scripts/do_wamp_call`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/scripts/gtcserver` & `hcam_devices-1.3.0/scripts/gtcserver`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/scripts/hserver` & `hcam_devices-1.3.0/scripts/hserver`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/scripts/hwlogger` & `hcam_devices-1.3.0/scripts/hwlogger`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,55 @@
 #! /usr/bin/env python
 #
 # This is open-source software licensed under a BSD license.
 # Please see the file LICENSE.txt for details.
 #
 import pickle
+import math
+from queue import Queue
 
+import pandas as pd
 from autobahn.twisted.component import Component, run
 from autobahn.twisted.wamp import ApplicationSession
 from influxdb import InfluxDBClient
 from twisted.internet import threads
 from twisted.internet.defer import inlineCallbacks
 from twisted.logger import Logger
 from twisted.internet.task import LoopingCall
 
 HEARTBEAT_DELAY = 15
 
 
+class TelemetryWriter:
+    def __init__(self, num_retries=10):
+        self._client = InfluxDBClient(host="pulsar.shef.ac.uk", port=8086)
+        self._client.switch_database("hipercam")
+        self._retries_remaining = num_retries
+        # we use a threadsafe queue to store data points for writing
+        self._data_queue = Queue()
+
+    def put(self, points):
+        self._data_queue.put(points)
+
+    def write_points(self):
+        points = self._data_queue.get()
+        while self._retries_remaining > 0:
+            try:
+                self._client.write_points(points, time_precision="ms")
+            except Exception as e:
+                self._retries_remaining -= 1
+                continue
+            else:
+                self._retries_remaining = 10
+                break
+        if self._retries_remaining == 0:
+            raise Exception("cannot write to DB, retries exhausted")
+        self._data_queue.task_done()
+
+
 class TelemetryLogger(ApplicationSession):
     log = Logger()
 
     def onJoin(self, details):
         print("session ready")
         self.topic_callbacks = {
             "hipercam.ccd1.telemetry": self.log_ccd1_telemetry,
@@ -32,108 +62,141 @@
             "hipercam.pressure3.telemetry": self.log_ccd3_pressure_telemetry,
             "hipercam.pressure4.telemetry": self.log_ccd4_pressure_telemetry,
             "hipercam.pressure5.telemetry": self.log_ccd5_pressure_telemetry,
             "hipercam.slide.telemetry": self.log_slide_telemetry,
             "hipercam.compo.telemetry": self.log_compo_telemetry,
             "hipercam.autoguider.telemetry": self.log_ag_telemetry,
             "hipercam.rack.telemetry": self.log_rack_telemetry,
+            "hipercam.gps.telemetry": self.log_gps_telemetry,
+            "hipercam.chiller.telemetry": self.log_chiller_telemetry,
         }
-        self._client = InfluxDBClient(host="pulsar.shef.ac.uk", port=8086)
-        self._client.switch_database("hipercam")
         self._points = []  # list of dictionaries containing data to write
-        self._bulk_limit = 10  # a write is triggered once we have this many points
-        self._retries_remaining = (
-            10  # will attempt to write data numerous times before giving up
-        )
+        self._bulk_limit = 50  # a write is triggered once we have this many points
+        # writer class
+        self._writer = TelemetryWriter()
+
         # subscribe to telemetry topics
         for topic in self.topic_callbacks:
             callback = self.topic_callbacks[topic]
             self.subscribe(callback, topic)
 
         self._tick_no = 0
         self._tick_loop = LoopingCall(self._tick)
         self._tick_loop.start(HEARTBEAT_DELAY)
 
     def _tick(self):
         self._tick_no += 1
         self.log.info("hwlogger is alive [tick {}]".format(self._tick_no))
 
-    def update_db(self):
-        """
-        Update influx DB
-        """
-        try:
-            self.log.debug("attempting write")
-            result = self._client.write_points(self._points, time_precision="ms")
-        except Exception as err:
-            self.log.warn(f"failed writing batch of data (will retry): {err}")
-            result = False
-
-        self.log.debug("updated DB")
-        if result:
-            self._points = []
-            self._retries_remaining = 10
-        elif self._retries_remaining > 0:
-            self._retries_remaining -= 1
-        else:
-            self.points = []
-            self.retries_remainining = 10
-            self.log.error(
-                "could not write data to DB, giving up. this batch of data is lost!"
-            )
-
     @inlineCallbacks
     def log_telemetry(self, point):
         """
-        asynchronous database update
+        asynchronous database update, with retries
         """
-        self.log.debug("logging telemetry")
-        # if we haven't reached threshold for update, add to queue
-        if len(self._points) < self._bulk_limit:
-            self._points.append(point)
-            return
-
-        # we've reached bulk threshold, update_db
         try:
-            self.log.debug("logging telemetry to DB")
-            yield threads.deferToThread(self.update_db)
+            self.log.debug("logging telemetry")
+            # add this point
+            if not self.is_empty(point):
+                self._points.append(point)
+
+                # if we haven't reached threshold for update, add to queue
+                if len(self._points) < self._bulk_limit:
+                    return
+
+                # we've reached bulk threshold, add to database queue
+                self.log.debug("logging telemetry to DB")
+                self._writer.put(self._points)
+                self._points = []
+                try:
+                    yield threads.deferToThread(self._writer.write_points)
+                except Exception as e:
+                    self.log.warn(f"cannot write to DB: {e}\n this data is lost")
+                finally:
+                    self.log.debug("data written to DB")
         except Exception as e:
-            self.log.error(str(e))
+            self.log.warn(str(e))
+            
 
     def preprocess_telemetry(self, data):
         telemetry = pickle.loads(data)
         ts = telemetry.pop("timestamp")
         ts.precision = 2
         return ts.iso, telemetry
 
     def process_field(self, field):
         if hasattr(field, "value"):
             return field.value
         return field
 
+    def _is_not_null(self, value):
+        is_none = value is None
+        # check for empty strings or None
+        if isinstance(value, str):
+            return not value or is_none
+        # numeric values could be NaN or None - check None first
+        if is_none:
+            return False
+        # not a string or None
+        return not math.isnan(value)
+
+    def is_empty(self, point):
+        # check if all points are None or NaN
+        # first change None to NaN
+        try:
+            fields = point["fields"]
+            fields = [
+                field if self._is_not_null(field) else None for field in fields.values()
+            ]
+            return all([v is None for v in fields])
+        except Exception as err:
+            self.log.error(f"cannot check if point is empty: {err}")
+            return True
+
     def make_point(self, data, measurement):
         point = {}
         point["measurement"] = measurement
         ts, telemetry = self.preprocess_telemetry(data)
         point["time"] = ts
         # set fields to telemetry
         point["fields"] = {k: self.process_field(v) for (k, v) in telemetry.items()}
         return point
 
+    def dump_points(self):
+        df = pd.json_normalize(self._points)
+        df.to_csv("dump.csv", index=True)
+
     def log_ccd_telemetry(self, ccd, data):
         try:
             point = self.make_point(data, ccd)
             self.log.debug(f"point made with timestamp {point['time']}")
         except Exception as err:
             self.log.error(f"cannot process telemetry for {ccd}: {err}")
         else:
             # don't log pressure twice!
             point["fields"].pop("pressure")
             self.log_telemetry(point)
 
+    def log_gps_telemetry(self, data):
+        try:
+            point = self.make_point(data, "gps")
+            del point["fields"]["state"]
+        except Exception as err:
+            self.log.error(f"cannot process GPS telemetry: {err}")
+        else:
+            self.log_telemetry(point)
+
+    def log_chiller_telemetry(self, data):
+        try:
+            point = self.make_point(data, "chiller")
+            del point["fields"]["state"]
+        except Exception as err:
+            self.log.error(f"cannot process Chiller telemetry: {err}")
+        else:
+            self.log_telemetry(point)
+
     def log_rack_telemetry(self, data):
         try:
             point = self.make_point(data, "rack")
         except Exception as err:
             self.log.error(f"cannot process rack telemetry: {err}")
         else:
             # only want temperatures
```

### Comparing `hcam_devices-1.2.1/scripts/hwserver` & `hcam_devices-1.3.0/scripts/hwserver`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     MeerstetterComponent,
     CompoComponent,
     CompoArmComponent,
     CompoLensComponent,
     FocalPlaneSlideComponent,
     FlowSensorComponent,
     RackComponent,
+    GPSComponent,
+    GTCCoolingComponent,
 )
 
 parser = argparse.ArgumentParser()
 parser.add_argument(
     "-e", "--emulate", help="use emulated hardware", action="store_true"
 )
 args = parser.parse_args()
@@ -236,14 +238,28 @@
 rack = Component(
     transports=transport_cfg,
     realm="realm1",
     session_factory=RackComponent,
     extra=dict(name="rack", emulate=EMULATE),
 )
 
+gps = Component(
+    transports=transport_cfg,
+    realm="realm1",
+    session_factory=GPSComponent,
+    extra=dict(name="gps", emulate=EMULATE),
+)
+
+chiller = Component(
+    transports=transport_cfg,
+    realm="realm1",
+    session_factory=GTCCoolingComponent,
+    extra=dict(name="chiller", emulate=EMULATE),
+)
+
 components = [
     ccd1,
     ccd2,
     ccd3,
     ccd4,
     ccd5,
     p1,
@@ -255,14 +271,16 @@
     ms2,
     flow,
     slide,
     compo_lens,
     compo_arms,
     compo,
     rack,
+    gps,
+    chiller,
 ]
 # run each component in it's own Python process
 if __name__ == "__main__":
     freeze_support()
     pool_size = len(components)
     with Pool(pool_size) as pool:
         try:
```

### Comparing `hcam_devices-1.2.1/scripts/show_telemetry` & `hcam_devices-1.3.0/scripts/show_telemetry`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/scripts/tcp_serial_bridge` & `hcam_devices-1.3.0/scripts/tcp_serial_bridge`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/scripts/zaber_ascii` & `hcam_devices-1.3.0/scripts/zaber_ascii`

 * *Files identical despite different names*

### Comparing `hcam_devices-1.2.1/setup.py` & `hcam_devices-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,21 +38,21 @@
     fname
     for fname in glob.glob(os.path.join("scripts", "*"))
     if os.path.basename(fname) != "README.rst"
 ]
 
 setup(
     name="hcam_devices",
-    version="1.2.1",
+    version="1.3.0",
     description="Device Communication via WAMP for HiPerCAM",
     long_description=readme + "\n\n" + history,
     author="Stuart Littlefair",
     author_email="s.littlefair@shef.ac.uk",
     url="https://github.com/HiPERCAM/hcam_devices",
-    download_url="https://github.com/HiPERCAM/hcam_devices/archive/v1.2.1.tar.gz",
+    download_url="https://github.com/HiPERCAM/hcam_devices/archive/v1.3.0.tar.gz",
     packages=[
         "hcam_devices",
         "hcam_devices.gtc",
         "hcam_devices.devices",
         "hcam_devices.components",
         "hcam_devices.machines",
         "hcam_devices.models",
```

