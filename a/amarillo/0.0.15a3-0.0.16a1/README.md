# Comparing `tmp/amarillo-0.0.15a3.tar.gz` & `tmp/amarillo-0.0.16a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amarillo-0.0.15a3.tar", last modified: Fri Feb  2 12:54:41 2024, max compression
+gzip compressed data, was "amarillo-0.0.16a1.tar", last modified: Thu May 23 09:04:00 2024, max compression
```

## Comparing `amarillo-0.0.15a3.tar` & `amarillo-0.0.16a1.tar`

### file list

```diff
@@ -1,65 +1,87 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-02 12:54:41.894299 amarillo-0.0.15a3/
--rw-r--r--   0 user      (1000) user      (1000)    34523 2024-01-25 10:12:03.000000 amarillo-0.0.15a3/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)    42781 2024-02-02 12:54:41.894299 amarillo-0.0.15a3/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2362 2024-02-01 14:50:17.000000 amarillo-0.0.15a3/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-02 12:54:41.886299 amarillo-0.0.15a3/amarillo/
--rw-r--r--   0 user      (1000) user      (1000)       64 2024-02-01 14:41:03.000000 amarillo-0.0.15a3/amarillo/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     3728 2024-02-01 14:41:03.000000 amarillo-0.0.15a3/amarillo/configuration.py
--rw-r--r--   0 user      (1000) user      (1000)     4362 2024-02-01 14:45:16.000000 amarillo-0.0.15a3/amarillo/main.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-02 12:54:41.886299 amarillo-0.0.15a3/amarillo/models/
--rw-r--r--   0 user      (1000) user      (1000)      778 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/models/AgencyConf.py
--rw-r--r--   0 user      (1000) user      (1000)    11411 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/models/Carpool.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/models/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     1662 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/models/gtfs.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-02 12:54:41.886299 amarillo-0.0.15a3/amarillo/plugins/
--rw-r--r--   0 user      (1000) user      (1000)       64 2024-02-01 14:45:16.000000 amarillo-0.0.15a3/amarillo/plugins/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-02 12:54:41.886299 amarillo-0.0.15a3/amarillo/routers/
--rw-r--r--   0 user      (1000) user      (1000)        0 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/routers/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     3277 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/routers/agency.py
--rw-r--r--   0 user      (1000) user      (1000)     4159 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/routers/agencyconf.py
--rw-r--r--   0 user      (1000) user      (1000)     4967 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/routers/carpool.py
--rw-r--r--   0 user      (1000) user      (1000)     3097 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/routers/region.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-02 12:54:41.890299 amarillo-0.0.15a3/amarillo/services/
--rw-r--r--   0 user      (1000) user      (1000)        0 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      737 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/agencies.py
--rw-r--r--   0 user      (1000) user      (1000)     3867 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/agencyconf.py
--rw-r--r--   0 user      (1000) user      (1000)     2277 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/carpools.py
--rw-r--r--   0 user      (1000) user      (1000)      343 2024-02-01 14:41:03.000000 amarillo-0.0.15a3/amarillo/services/config.py
--rw-r--r--   0 user      (1000) user      (1000)     4400 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/gtfs.py
--rw-r--r--   0 user      (1000) user      (1000)      393 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/gtfs_constants.py
--rw-r--r--   0 user      (1000) user      (1000)     9879 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/gtfs_export.py
--rw-r--r--   0 user      (1000) user      (1000)     2225 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/gtfs_generator.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-02 12:54:41.890299 amarillo-0.0.15a3/amarillo/services/gtfsrt/
--rw-r--r--   0 user      (1000) user      (1000)        0 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/gtfsrt/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    12321 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/gtfsrt/gtfs_realtime_pb2.py
--rw-r--r--   0 user      (1000) user      (1000)     2526 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/gtfsrt/realtime_extension_pb2.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-02 12:54:41.890299 amarillo-0.0.15a3/amarillo/services/importing/
--rw-r--r--   0 user      (1000) user      (1000)        0 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/importing/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2069 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/importing/ride2go.py
--rw-r--r--   0 user      (1000) user      (1000)     1843 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/mocks.py
--rw-r--r--   0 user      (1000) user      (1000)      605 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/regions.py
--rw-r--r--   0 user      (1000) user      (1000)     1717 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/routing.py
--rw-r--r--   0 user      (1000) user      (1000)      603 2024-02-02 12:25:05.000000 amarillo-0.0.15a3/amarillo/services/secrets.py
--rw-r--r--   0 user      (1000) user      (1000)     8154 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/services/stops.py
--rw-r--r--   0 user      (1000) user      (1000)    16723 2024-02-01 14:43:41.000000 amarillo-0.0.15a3/amarillo/services/trips.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-02 12:54:41.894299 amarillo-0.0.15a3/amarillo/tests/
--rw-r--r--   0 user      (1000) user      (1000)        0 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/tests/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     1428 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/tests/no_test_carpool.py
--rw-r--r--   0 user      (1000) user      (1000)     3066 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/tests/sampledata.py
--rw-r--r--   0 user      (1000) user      (1000)     5287 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/tests/test_gtfs.py
--rw-r--r--   0 user      (1000) user      (1000)     1071 2024-02-01 14:40:53.000000 amarillo-0.0.15a3/amarillo/tests/test_stops_store.py
--rw-r--r--   0 user      (1000) user      (1000)      697 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/tests/test_trip_store.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-02 12:54:41.894299 amarillo-0.0.15a3/amarillo/utils/
--rw-r--r--   0 user      (1000) user      (1000)        0 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/utils/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       15 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/utils/container.py
--rw-r--r--   0 user      (1000) user      (1000)     1174 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/utils/utils.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-02 12:54:41.894299 amarillo-0.0.15a3/amarillo/views/
--rw-r--r--   0 user      (1000) user      (1000)      480 2024-02-01 14:40:29.000000 amarillo-0.0.15a3/amarillo/views/home.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-02 12:54:41.894299 amarillo-0.0.15a3/amarillo.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    42781 2024-02-02 12:54:41.000000 amarillo-0.0.15a3/amarillo.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1486 2024-02-02 12:54:41.000000 amarillo-0.0.15a3/amarillo.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2024-02-02 12:54:41.000000 amarillo-0.0.15a3/amarillo.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)      192 2024-02-02 12:54:41.000000 amarillo-0.0.15a3/amarillo.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       54 2024-02-02 12:54:41.000000 amarillo-0.0.15a3/amarillo.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)      580 2024-02-02 12:53:57.000000 amarillo-0.0.15a3/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)       38 2024-02-02 12:54:41.894299 amarillo-0.0.15a3/setup.cfg
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.352624 amarillo-0.0.16a1/
+-rw-r--r--   0 user      (1000) user      (1000)       72 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     3019 2024-05-23 09:04:00.352624 amarillo-0.0.16a1/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2342 2024-04-18 13:19:30.000000 amarillo-0.0.16a1/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.344624 amarillo-0.0.16a1/amarillo/
+-rw-r--r--   0 user      (1000) user      (1000)       64 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1878 2024-04-18 13:19:30.000000 amarillo-0.0.16a1/amarillo/configuration.py
+-rw-r--r--   0 user      (1000) user      (1000)     4883 2024-04-18 13:19:30.000000 amarillo-0.0.16a1/amarillo/main.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.344624 amarillo-0.0.16a1/amarillo/models/
+-rw-r--r--   0 user      (1000) user      (1000)    15306 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/models/Carpool.py
+-rw-r--r--   0 user      (1000) user      (1000)     1593 2024-04-22 12:53:17.000000 amarillo-0.0.16a1/amarillo/models/User.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/models/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.344624 amarillo-0.0.16a1/amarillo/plugins/
+-rw-r--r--   0 user      (1000) user      (1000)       64 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/plugins/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.344624 amarillo-0.0.16a1/amarillo/routers/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/routers/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3274 2024-04-22 12:53:17.000000 amarillo-0.0.16a1/amarillo/routers/agency.py
+-rw-r--r--   0 user      (1000) user      (1000)     6490 2024-05-22 12:53:49.000000 amarillo-0.0.16a1/amarillo/routers/carpool.py
+-rw-r--r--   0 user      (1000) user      (1000)     1582 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/routers/region.py
+-rw-r--r--   0 user      (1000) user      (1000)     2696 2024-04-22 12:53:17.000000 amarillo-0.0.16a1/amarillo/routers/users.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.348624 amarillo-0.0.16a1/amarillo/services/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/services/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      736 2024-04-18 13:19:30.000000 amarillo-0.0.16a1/amarillo/services/agencies.py
+-rw-r--r--   0 user      (1000) user      (1000)     2486 2024-05-03 11:45:54.000000 amarillo-0.0.16a1/amarillo/services/carpools.py
+-rw-r--r--   0 user      (1000) user      (1000)      391 2024-05-23 09:03:24.000000 amarillo-0.0.16a1/amarillo/services/config.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.348624 amarillo-0.0.16a1/amarillo/services/importing/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/services/importing/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2069 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/services/importing/ride2go.py
+-rw-r--r--   0 user      (1000) user      (1000)     1843 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/services/mocks.py
+-rw-r--r--   0 user      (1000) user      (1000)     5936 2024-05-22 12:53:49.000000 amarillo-0.0.16a1/amarillo/services/oauth2.py
+-rw-r--r--   0 user      (1000) user      (1000)      298 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/services/passwords.py
+-rw-r--r--   0 user      (1000) user      (1000)      604 2024-04-18 13:19:30.000000 amarillo-0.0.16a1/amarillo/services/regions.py
+-rw-r--r--   0 user      (1000) user      (1000)      450 2024-04-18 13:19:30.000000 amarillo-0.0.16a1/amarillo/services/secrets.py
+-rw-r--r--   0 user      (1000) user      (1000)     3884 2024-05-22 12:53:49.000000 amarillo-0.0.16a1/amarillo/services/users.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.348624 amarillo-0.0.16a1/amarillo/static/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.348624 amarillo-0.0.16a1/amarillo/static/conf/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.348624 amarillo-0.0.16a1/amarillo/static/conf/agency/
+-rw-r--r--   0 user      (1000) user      (1000)      162 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/conf/agency/frank.json
+-rw-r--r--   0 user      (1000) user      (1000)      162 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/conf/agency/goflux.json
+-rw-r--r--   0 user      (1000) user      (1000)      158 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/conf/agency/mentz.json
+-rw-r--r--   0 user      (1000) user      (1000)      152 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/conf/agency/mfdz.json
+-rw-r--r--   0 user      (1000) user      (1000)      146 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/conf/agency/mifaz.json
+-rw-r--r--   0 user      (1000) user      (1000)      150 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/conf/agency/mvv.json
+-rw-r--r--   0 user      (1000) user      (1000)      156 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/conf/agency/ride2go.json
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.352624 amarillo-0.0.16a1/amarillo/static/conf/region/
+-rw-r--r--   0 user      (1000) user      (1000)       52 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/conf/region/bb.json
+-rw-r--r--   0 user      (1000) user      (1000)       51 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/conf/region/bw.json
+-rw-r--r--   0 user      (1000) user      (1000)       51 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/conf/region/by.json
+-rw-r--r--   0 user      (1000) user      (1000)       51 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/conf/region/nrw.json
+-rw-r--r--   0 user      (1000) user      (1000)      253 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/conf/stop_sources.json
+-rw-r--r--   0 user      (1000) user      (1000)      294 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/config
+-rw-r--r--   0 user      (1000) user      (1000)      542 2024-04-18 13:19:30.000000 amarillo-0.0.16a1/amarillo/static/logging.conf
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.340624 amarillo-0.0.16a1/amarillo/static/static/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.352624 amarillo-0.0.16a1/amarillo/static/static/css/
+-rw-r--r--   0 user      (1000) user      (1000)      591 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/static/css/docs.css
+-rw-r--r--   0 user      (1000) user      (1000)     3029 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/static/css/theme.css
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.352624 amarillo-0.0.16a1/amarillo/static/static/img/
+-rw-r--r--   0 user      (1000) user      (1000)    17236 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/static/img/cloud.png
+-rw-r--r--   0 user      (1000) user      (1000)    15406 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/static/img/favicon.ico
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.340624 amarillo-0.0.16a1/amarillo/static/templates/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.352624 amarillo-0.0.16a1/amarillo/static/templates/home/
+-rw-r--r--   0 user      (1000) user      (1000)     2765 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/templates/home/index.html
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.352624 amarillo-0.0.16a1/amarillo/static/templates/shared/
+-rw-r--r--   0 user      (1000) user      (1000)     2830 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/static/templates/shared/layout.html
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.352624 amarillo-0.0.16a1/amarillo/tests/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/tests/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.352624 amarillo-0.0.16a1/amarillo/tests/__pycache__/
+-rw-r--r--   0 user      (1000) user      (1000)      151 2024-04-05 12:03:16.000000 amarillo-0.0.16a1/amarillo/tests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     2147 2024-04-05 12:03:16.000000 amarillo-0.0.16a1/amarillo/tests/__pycache__/sampledata.cpython-39.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     1438 2024-04-22 12:01:35.000000 amarillo-0.0.16a1/amarillo/tests/__pycache__/test_permissions.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     1428 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/tests/no_test_carpool.py
+-rw-r--r--   0 user      (1000) user      (1000)     3066 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/tests/sampledata.py
+-rw-r--r--   0 user      (1000) user      (1000)     1329 2024-04-22 12:53:17.000000 amarillo-0.0.16a1/amarillo/tests/test_permissions.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.352624 amarillo-0.0.16a1/amarillo/utils/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/utils/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)       15 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/utils/container.py
+-rw-r--r--   0 user      (1000) user      (1000)     2294 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/utils/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.352624 amarillo-0.0.16a1/amarillo/views/
+-rw-r--r--   0 user      (1000) user      (1000)      480 2024-03-07 15:14:39.000000 amarillo-0.0.16a1/amarillo/views/home.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 09:04:00.352624 amarillo-0.0.16a1/amarillo.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3019 2024-05-23 09:04:00.000000 amarillo-0.0.16a1/amarillo.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2020 2024-05-23 09:04:00.000000 amarillo-0.0.16a1/amarillo.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-05-23 09:04:00.000000 amarillo-0.0.16a1/amarillo.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)      248 2024-05-23 09:04:00.000000 amarillo-0.0.16a1/amarillo.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       54 2024-05-23 09:04:00.000000 amarillo-0.0.16a1/amarillo.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)      656 2024-05-23 09:03:51.000000 amarillo-0.0.16a1/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-05-23 09:04:00.352624 amarillo-0.0.16a1/setup.cfg
```

### Comparing `amarillo-0.0.15a3/README.md` & `amarillo-0.0.16a1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 ## Security
 
 All endpoints are protected by an API-Key in the HTTP header. 
 There is a special *admin* user. 
 For this user, the API-Key must be passed in as an environment variable when 
 Amarillo is started.
 
-The admin can create additional API-Keys in the `/agencyconf` endpoint. This 
+The admin can create additional API-Keys in the `/users` endpoint. This 
 endpoint is always available but not always shown in `/docs`, especially not
 when running in production. 
-The Swagger docs for `/agencyconf` can be seen on the MFDZ demo server. 
+The Swagger docs for `/users` can be seen on the MFDZ demo server. 
 
 Permissions work this way
 - the admin is allowed to call all operations on all resources. Only the admin
-  can create new API-Keys by POSTing an `AgencyConf` JSON object to `/agencyconf`. 
+  can create new API-Keys by POSTing an `users` JSON object to `/users`. 
 - API-Keys for agencies are allowed to POST/PUT/GET/DELETE their own 
   resources and GET some public resources.  
 
 ## Development
 
 ### GTFS-RT python bindings
```

### Comparing `amarillo-0.0.15a3/amarillo/main.py` & `amarillo-0.0.16a1/amarillo/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,22 @@
 import importlib
 import pkgutil
 
 import uvicorn
 import mimetypes
 from starlette.staticfiles import StaticFiles
 
+from amarillo.utils.utils import copy_static_files
+#this has to run before app.configuration is imported, otherwise we get validation error for config because the config file is not copied yet
+copy_static_files(["conf", "static", "templates", "logging.conf", "config"]) 
+
 import amarillo.plugins
 from amarillo.configuration import configure_services, configure_admin_token
-from amarillo.routers import carpool, agency, agencyconf, region
+from amarillo.routers import carpool, agency, region, users
+import amarillo.services.oauth2 as oauth2
 from fastapi import FastAPI
 
 # https://pydantic-docs.helpmanual.io/usage/settings/
 from amarillo.views import home
 
 logging.config.fileConfig('logging.conf', disable_existing_loggers=False)
 logger = logging.getLogger("main")
@@ -63,45 +68,50 @@
                       "url": "https://amarillo.mfdz.de"
                   },
                   {
                       "description": "Dev server for development",
                       "url": "https://amarillo-dev.mfdz.de"
                   },
                   {
+                      "description": "Server for Mitanand project",
+                      "url": "https://mitanand.mfdz.de"
+                  },
+                  {
                       "description": "Localhost for development",
                       "url": "http://localhost:8000"
                   }
               ],
               redoc_url=None
               )
 
 app.include_router(carpool.router)
 app.include_router(agency.router)
-app.include_router(agencyconf.router)
+app.include_router(users.router)
 app.include_router(region.router)
+app.include_router(oauth2.router)
 
 
 def iter_namespace(ns_pkg):
      # Source: https://packaging.python.org/guides/creating-and-discovering-plugins/
     return pkgutil.iter_modules(ns_pkg.__path__, ns_pkg.__name__ + ".")
 
 def load_plugins():
     discovered_plugins = {
         name: importlib.import_module(name)
         for finder, name, ispkg
         in iter_namespace(amarillo.plugins)
     }
-    print(f"Discovered plugins: {list(discovered_plugins.keys())}")
+    logger.info(f"Discovered plugins: {list(discovered_plugins.keys())}")
 
     for name, module in discovered_plugins.items():
         if hasattr(module, "setup"):
-            print(f"Running setup function for {name}")
+            logger.info(f"Running setup function for {name}")
             module.setup(app)
 
-        else: print(f"Did not find setup function for {name}")
+        else: logger.info(f"Did not find setup function for {name}")
 
 def configure():
     configure_admin_token()
     configure_services()
     configure_routing()
     load_plugins()
```

### Comparing `amarillo-0.0.15a3/amarillo/models/Carpool.py` & `amarillo-0.0.16a1/amarillo/models/Carpool.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import time, date, datetime
 from pydantic import ConfigDict, BaseModel, Field, HttpUrl, EmailStr
 from typing import List, Union, Set, Optional, Tuple
 from datetime import time
 from pydantic import BaseModel, Field
 from geojson_pydantic.geometries import LineString
-from enum import Enum
+from enum import Enum, IntEnum
 
 NumType = Union[float, int]
 
 MAX_STOPS_PER_TRIP = 100
 
 class Weekday(str, Enum):
     monday = "monday"
@@ -20,14 +20,23 @@
     sunday = "sunday"
 
 class PickupDropoffType(str, Enum):
     pickup_and_dropoff = "pickup_and_dropoff"
     only_pickup = "only_pickup"
     only_dropoff = "only_dropoff"
 
+class YesNoEnum(IntEnum):
+    yes = 1
+    no = 2
+
+class LuggageSize(IntEnum):
+    small = 1
+    medium = 2
+    large = 3
+
 class StopTime(BaseModel):
     id: Optional[str] = Field(
         None,
         description="Optional Stop ID. If given, it should conform to the "
                     "IFOPT specification. For official transit stops, "
                     "it should be their official IFOPT. In Germany, this is "
                     "the DHID which is available via the 'zentrales "
@@ -106,15 +115,91 @@
         max_length=20,
         pattern='^[a-zA-Z0-9]+$',
         examples=["bb"])
     
     bbox: Tuple[NumType, NumType, NumType, NumType] = Field(
         description="Bounding box of the region. Format is [minLon, minLat, maxLon, maxLat]",
         examples=[[10.5,49.2,11.3,51.3]])
+    
+class RidesharingInfo(BaseModel):
+    number_free_seats: int = Field(
+        description="Number of free seats",
+        ge=0,
+        examples=[3])
+    
+    same_gender: Optional[YesNoEnum] = Field(
+        None, 
+        description="Trip only for same gender:"
+                    "1: Yes"
+                    "2: No",
+        examples=[1])
+    luggage_size: Optional[LuggageSize] = Field(
+        None, 
+        description="Size of the luggage:"
+                    "1: small"
+                    "2: medium"
+                    "3: large",
+        examples=[3])
+    animal_car: Optional[YesNoEnum] = Field(
+        None, 
+        description="Animals in Car allowed:"
+                    "1: Yes"
+                    "2: No",
+        examples=[2])
 
+    car_model: Optional[str] = Field(
+        None,
+        description="Car model",
+        min_length=1,
+        max_length=48,
+        examples=["Golf"])
+    car_brand: Optional[str] = Field(
+        None,
+        description="Car brand",
+        min_length=1,
+        max_length=48,
+        examples=["VW"])
+    
+    creation_date: datetime = Field(
+        description="Date when trip was created",
+        examples=["2022-02-13T20:20:39+00:00"])
+    
+    smoking: Optional[YesNoEnum] = Field(
+        None, 
+        description="Smoking allowed:"
+                    "1: Yes"
+                    "2: No",
+        examples=[2])
+    
+    payment_method: Optional[str] = Field(
+        None,
+        description="Method of payment",
+        min_length=1,
+        max_length=48)
+
+class Driver(BaseModel):
+    driver_id: Optional[str] = Field(
+        None,
+        description="Identifies the driver.",
+        min_length=1,
+        max_length=256,
+        pattern='^[a-zA-Z0-9_-]+$',
+        examples=["789"])
+    profile_picture: Optional[HttpUrl] = Field(
+        None,
+        description="URL that contains the profile picture",
+        examples=["https://mfdz.de/driver/789/picture"])
+    rating: Optional[int] = Field(
+        None,
+        description="Rating of the driver from 1 to 5."
+                    "0 no rating yet",
+        ge=0,
+        le=5,
+        examples=[5])
+    
 class Agency(BaseModel):
     id: str = Field(
         description="ID of the agency.",
         min_length=1,
         max_length=20,
         pattern='^[a-zA-Z0-9]+$',
         examples=["mfdz"])
@@ -191,14 +276,25 @@
     agency: str = Field(
         description="Short one string name of the agency, used as a namespace "
                     "for ids.",
         min_length=1,
         max_length=20,
         pattern='^[a-zA-Z0-9]+$',
         examples=["mfdz"])
+    
+    driver: Optional[Driver] = Field(
+        None, 
+        description="Driver data", 
+        examples=["""
+                {
+                    "driver_id": "123", 
+                    "profile_picture": "https://mfdz.de/driver/789/picture",
+                    "rating": 5
+                }
+                """])
 
     deeplink: HttpUrl = Field(
         description="Link to an information page providing detail information "
                     "for this offer, and, especially, an option to book the "
                     "trip/contact the driver.",
         examples=["https://mfdz.de/trip/103361"])
 
@@ -241,26 +337,53 @@
         description="Date when the trip will start, in case it is a one-time "
                     "trip. For recurring trips, specify weekdays. "
                     "Note, that when for different weekdays different "
                     "departureTimes apply, multiple carpool offers should be "
                     "published.",
         examples=['A single date 2022-04-04 or a list of weekdays ["saturday", '
                 '"sunday"]'])
-
+    route_color: Optional[str] = Field(
+        None,
+        pattern='^([0-9A-Fa-f]{6})$',
+        description="Route color designation that matches public facing material. "
+                    "The color difference between route_color and route_text_color "
+                    "should provide sufficient contrast when viewed on a black and "
+                    "white screen.",
+        examples=["0039A6"])
+    route_text_color: Optional[str] = Field(
+        None,
+        pattern='^([0-9A-Fa-f]{6})$',
+        description="Legible color to use for text drawn against a background of "
+                    "route_color. The color difference between route_color and "
+                    "route_text_color should provide sufficient contrast when "
+                    "viewed on a black and white screen.",
+        examples=["D4D2D2"])
     path: Optional[LineString] = Field(
         None, description="Optional route geometry as json LineString.")
     
     lastUpdated: Optional[datetime] = Field(
         None,
         description="LastUpdated should reflect the last time, the user "
                     "providing this offer, made an update or confirmed, "
                     "the offer is still valid. Note that this service might "
                     "purge outdated offers (e.g. older than 180 days). If not "
                     "passed, the service may assume 'now'",
         examples=["2022-02-13T20:20:39+00:00"])
+    additional_ridesharing_info: Optional[RidesharingInfo] = Field(
+        None, 
+        description="Extension of GRFS to the GTFS standard", 
+        examples=["""
+                {
+                    "number_free_seats": 2, 
+                    "creation_date": "2022-02-13T20:20:39+00:00", 
+                    "same_gender": 2,
+                    "smoking": 1,
+                    "luggage_size": 3
+                }
+                """])
     model_config = ConfigDict(json_schema_extra={
         "title": "Carpool",   
         # description ...
         "example":
             """
                 {
                   "id": "1234",
```

### Comparing `amarillo-0.0.15a3/amarillo/routers/agency.py` & `amarillo-0.0.16a1/amarillo/routers/agency.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 import time
 from typing import List
 
 from fastapi import APIRouter, HTTPException, status, Depends
 
 from amarillo.models.Carpool import Carpool, Agency
-from amarillo.routers.agencyconf import verify_api_key, verify_admin_api_key, verify_permission_for_same_agency_or_admin
+from amarillo.models.User import User
+from amarillo.services.oauth2 import get_current_user, verify_permission
 # TODO should move this to service
 from amarillo.routers.carpool import store_carpool, delete_agency_carpools_older_than
 from amarillo.services.agencies import AgencyService
 from amarillo.services.importing.ride2go import import_ride2go
 from amarillo.utils.container import container
 from fastapi.responses import FileResponse
 
@@ -28,15 +29,15 @@
             description="Find agency by ID",
             # TODO next to the status codes are "Links". There is nothing shown now.
             # Either show something there, or hide the Links, or do nothing.
             responses={ 
                 status.HTTP_404_NOT_FOUND: {"description": "Agency not found"},
             },
             )
-async def get_agency(agency_id: str, admin_api_key: str = Depends(verify_api_key)) -> Agency:
+async def get_agency(agency_id: str, requesting_user: User = Depends(get_current_user)) -> Agency:
     agencies: AgencyService = container['agencies']
     agency = agencies.get_agency(agency_id)
     agency_exists = agency is not None
 
     if not agency_exists:
         message = f"Agency with id {agency_id} does not exist."
         logger.error(message)
@@ -48,24 +49,25 @@
 
 # TODO add push batch endpoint
 
 @router.post("/{agency_id}/sync",
              operation_id="sync",
              summary="Synchronizes all carpool offers",
              response_model=List[Carpool],
+             response_model_exclude_none=True,
              responses={
                  status.HTTP_200_OK: {
                      "description": "Carpool created"},
                  status.HTTP_404_NOT_FOUND: {
                      "description": "Agency does not exist"},
                  status.HTTP_500_INTERNAL_SERVER_ERROR: {
                      "description": "Import error"}
              })
-async def sync(agency_id: str, requesting_agency_id: str = Depends(verify_api_key)) -> List[Carpool]:
-    await verify_permission_for_same_agency_or_admin(agency_id, requesting_agency_id)
+async def sync(agency_id: str, requesting_user: User = Depends(get_current_user)) -> List[Carpool]:
+    verify_permission(f"{agency_id}:sync")
 
     if agency_id == "ride2go":
         import_function = import_ride2go
     else:
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=f"Agency does not exist or does not support sync.")
```

### Comparing `amarillo-0.0.15a3/amarillo/routers/region.py` & `amarillo-0.0.16a1/amarillo/routers/region.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import logging
 import time
 from typing import List
 
 from fastapi import APIRouter, HTTPException, status, Depends
 
 from amarillo.models.Carpool import Region
-from amarillo.routers.agencyconf import verify_admin_api_key
 from amarillo.services.regions import RegionService
 from amarillo.utils.container import container
-from fastapi.responses import FileResponse
 
 logger = logging.getLogger(__name__)
 
 router = APIRouter(
     prefix="/region",
     tags=["region"]
 )
@@ -41,48 +39,17 @@
 async def get_region(region_id: str) -> Region:
     region = _assert_region_exists(region_id)
     logger.info(f"Get region {region_id}.")
 
     return region
 
 def _assert_region_exists(region_id: str) -> Region:
-    regions: regionService = container['regions']
+    regions: RegionService = container['regions']
     region = regions.get_region(region_id)
     region_exists = region is not None
 
     if not region_exists:
         message = f"Region with id {region_id} does not exist."
         logger.error(message)
         raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
 
     return region
-
-@router.get("/{region_id}/gtfs", 
-    summary="Return GTFS Feed for this region",
-    response_description="GTFS-Feed (zip-file)",
-    response_class=FileResponse,
-    responses={
-                status.HTTP_404_NOT_FOUND: {"description": "Region not found"},
-        }
-    )
-async def get_file(region_id: str, user: str = Depends(verify_admin_api_key)):
-    _assert_region_exists(region_id)
-    return FileResponse(f'data/gtfs/amarillo.{region_id}.gtfs.zip')
-
-@router.get("/{region_id}/gtfs-rt",
-    summary="Return GTFS-RT Feed for this region",
-    response_description="GTFS-RT-Feed",
-    response_class=FileResponse,
-    responses={
-                status.HTTP_404_NOT_FOUND: {"description": "Region not found"},
-                status.HTTP_400_BAD_REQUEST: {"description": "Bad request, e.g. because format is not supported, i.e. neither protobuf nor json."}
-        }
-    )
-async def get_file(region_id: str, format: str = 'protobuf', user: str = Depends(verify_admin_api_key)):
-    _assert_region_exists(region_id)
-    if format == 'json':
-        return FileResponse(f'data/gtfs/amarillo.{region_id}.gtfsrt.json')
-    elif format == 'protobuf':
-        return FileResponse(f'data/gtfs/amarillo.{region_id}.gtfsrt.pbf')
-    else:
-        message = "Specified format is not supported, i.e. neither protobuf nor json."
-        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=message)
```

### Comparing `amarillo-0.0.15a3/amarillo/services/agencies.py` & `amarillo-0.0.16a1/amarillo/services/agencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 # because the (updated) agencies are needed in the enhancer
 # as well.
 
 class AgencyService:
 
     def __init__(self):
         self.agencies: Dict[str, Agency] = {}
-
-        for agency_file_name in glob('conf/agency/*.json'):
+        for agency_file_name in glob('data/agency/*.json'):
             with open(agency_file_name) as agency_file:
                 dict = json.load(agency_file)
                 agency = Agency(**dict)
                 agency_id = agency.id
                 self.agencies[agency_id] = agency
 
     def get_agency(self, agency_id: str) -> Agency:
```

### Comparing `amarillo-0.0.15a3/amarillo/services/carpools.py` & `amarillo-0.0.16a1/amarillo/services/carpools.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,19 @@
         Iterates over all carpools and deletes those which are outdated
         """
         for key in list(self.carpools.keys()):
             cp = self.carpools.get(key)
             if cp and self.is_outdated(cp):
                 logger.info("Purge outdated offer %s", key)
                 self.delete(cp.agency, cp.id)
+                try:
+                    from amarillo.plugins.metrics import trips_deleted_counter
+                    trips_deleted_counter.inc()
+                except ImportError:
+                    pass
 
     def get(self, agency_id: str, carpool_id: str):
         return self.carpools.get(f"{agency_id}:{carpool_id}")
 
     def get_all_ids(self):
         return list(self.carpools)
```

### Comparing `amarillo-0.0.15a3/amarillo/services/importing/ride2go.py` & `amarillo-0.0.16a1/amarillo/services/importing/ride2go.py`

 * *Files identical despite different names*

### Comparing `amarillo-0.0.15a3/amarillo/services/mocks.py` & `amarillo-0.0.16a1/amarillo/services/mocks.py`

 * *Files identical despite different names*

### Comparing `amarillo-0.0.15a3/amarillo/services/regions.py` & `amarillo-0.0.16a1/amarillo/services/regions.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from amarillo.models.Carpool import Region
 
 
 class RegionService:
 
     def __init__(self):
         self.regions: Dict[str, Region] = {}
-
-        for region_file_name in glob('conf/region/*.json'):
+        for region_file_name in glob('data/region/*.json'):
             with open(region_file_name) as region_file:
                 dict = json.load(region_file)
                 region = Region(**dict)
                 region_id = region.id
                 self.regions[region_id] = region
 
     def get_region(self, region_id: str) -> Region:
```

### Comparing `amarillo-0.0.15a3/amarillo/tests/no_test_carpool.py` & `amarillo-0.0.16a1/amarillo/tests/no_test_carpool.py`

 * *Files identical despite different names*

### Comparing `amarillo-0.0.15a3/amarillo/tests/sampledata.py` & `amarillo-0.0.16a1/amarillo/tests/sampledata.py`

 * *Files identical despite different names*

### Comparing `amarillo-0.0.15a3/pyproject.toml` & `amarillo-0.0.16a1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "amarillo"
-version = "0.0.15a3"
+version = "0.0.16a1"
 description = "Aggregates and enhances carpooling-offers and publishes them as GTFS(-RT)"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["amarillo", "ridesharing", "carpooling", "gtfs", "gtfs-rt"]
 dependencies = [
     "fastapi[all]==0.109.0",
     "geopandas==0.14",
@@ -12,11 +12,14 @@
     "pydantic[dotenv]==2.4.2",
     "protobuf==3.20.3",
     "starlette~=0.35",
     "requests==2.31.0",
     "pyproj==3.6.1",
     "geojson-pydantic==1.0.1",
     "watchdog==3.0.0",
+    "python-jose[cryptography]",
+    "bcrypt==4.0.1",
+    "passlib[bcrypt]"
 ]
 
 [tool.setuptools.packages]
 find = {}
```

