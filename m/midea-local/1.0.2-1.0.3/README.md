# Comparing `tmp/midea_local-1.0.2.tar.gz` & `tmp/midea_local-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midea_local-1.0.2.tar", last modified: Tue May 21 23:49:49 2024, max compression
+gzip compressed data, was "midea_local-1.0.3.tar", last modified: Thu May 23 17:42:57 2024, max compression
```

## Comparing `midea_local-1.0.2.tar` & `midea_local-1.0.3.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.253440 midea_local-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 23:49:45.000000 midea_local-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-21 23:49:49.253440 midea_local-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-21 23:49:45.000000 midea_local-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.253440 midea_local-1.0.2/midea_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-21 23:49:49.000000 midea_local-1.0.2/midea_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-21 23:49:49.000000 midea_local-1.0.2/midea_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 23:49:49.000000 midea_local-1.0.2/midea_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 23:49:49.000000 midea_local-1.0.2/midea_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 23:49:49.000000 midea_local-1.0.2/midea_local.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.241440 midea_local-1.0.2/midealocal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.241440 midea_local-1.0.2/midealocal/backports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/backports/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/crc8.py
--rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.241440 midea_local-1.0.2/midealocal/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.241440 midea_local-1.0.2/midealocal/devices/a1/
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/a1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/a1/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.241440 midea_local-1.0.2/midealocal/devices/ac/
--rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/ac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25127 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/ac/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.241440 midea_local-1.0.2/midealocal/devices/b0/
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/b0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/b0/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.241440 midea_local-1.0.2/midealocal/devices/b1/
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/b1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/b1/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.241440 midea_local-1.0.2/midealocal/devices/b3/
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/b3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/b3/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.241440 midea_local-1.0.2/midealocal/devices/b4/
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/b4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/b4/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.245440 midea_local-1.0.2/midealocal/devices/b6/
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/b6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/b6/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.245440 midea_local-1.0.2/midealocal/devices/bf/
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/bf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/bf/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.245440 midea_local-1.0.2/midealocal/devices/c2/
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/c2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/c2/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.245440 midea_local-1.0.2/midealocal/devices/c3/
--rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/c3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/c3/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.245440 midea_local-1.0.2/midealocal/devices/ca/
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/ca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/ca/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.245440 midea_local-1.0.2/midealocal/devices/cc/
--rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/cc/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.245440 midea_local-1.0.2/midealocal/devices/cd/
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/cd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/cd/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.245440 midea_local-1.0.2/midealocal/devices/ce/
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/ce/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.245440 midea_local-1.0.2/midealocal/devices/cf/
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/cf/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.245440 midea_local-1.0.2/midealocal/devices/da/
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/da/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/da/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.245440 midea_local-1.0.2/midealocal/devices/db/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/db/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.245440 midea_local-1.0.2/midealocal/devices/dc/
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/dc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/dc/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.249440 midea_local-1.0.2/midealocal/devices/e1/
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/e1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/e1/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.249440 midea_local-1.0.2/midealocal/devices/e2/
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/e2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/e2/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.249440 midea_local-1.0.2/midealocal/devices/e3/
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/e3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/e3/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.249440 midea_local-1.0.2/midealocal/devices/e6/
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/e6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/e6/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.249440 midea_local-1.0.2/midealocal/devices/e8/
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/e8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/e8/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.249440 midea_local-1.0.2/midealocal/devices/ea/
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/ea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/ea/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.249440 midea_local-1.0.2/midealocal/devices/ec/
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/ec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/ec/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.249440 midea_local-1.0.2/midealocal/devices/ed/
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/ed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/ed/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.249440 midea_local-1.0.2/midealocal/devices/fa/
--rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/fa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/fa/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.249440 midea_local-1.0.2/midealocal/devices/fb/
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/fb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/fb/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.249440 midea_local-1.0.2/midealocal/devices/fc/
--rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/fc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/fc/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.253440 midea_local-1.0.2/midealocal/devices/fd/
--rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/fd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/fd/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.253440 midea_local-1.0.2/midealocal/devices/x13/
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/x13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/x13/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.253440 midea_local-1.0.2/midealocal/devices/x26/
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/x26/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/x26/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.253440 midea_local-1.0.2/midealocal/devices/x34/
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/x34/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/x34/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:49:49.253440 midea_local-1.0.2/midealocal/devices/x40/
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/x40/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/devices/x40/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/discover.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/packet_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-05-21 23:49:45.000000 midea_local-1.0.2/midealocal/security.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 23:49:49.253440 midea_local-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-21 23:49:45.000000 midea_local-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 17:42:49.000000 midea_local-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-23 17:42:57.129418 midea_local-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-23 17:42:49.000000 midea_local-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midea_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-23 17:42:57.000000 midea_local-1.0.3/midea_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-23 17:42:57.000000 midea_local-1.0.3/midea_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:42:57.000000 midea_local-1.0.3/midea_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 17:42:57.000000 midea_local-1.0.3/midea_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 17:42:57.000000 midea_local-1.0.3/midea_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.117417 midea_local-1.0.3/midealocal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.117417 midea_local-1.0.3/midealocal/backports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/backports/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25027 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/crc8.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.117417 midea_local-1.0.3/midealocal/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.117417 midea_local-1.0.3/midealocal/devices/a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/a1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/a1/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.117417 midea_local-1.0.3/midealocal/devices/ac/
+-rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25127 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ac/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b0/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b1/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/b3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b3/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b4/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/b6/
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b6/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/bf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/bf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/bf/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/c2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/c2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/c2/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/c3/
+-rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/c3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/c3/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/ca/
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ca/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/cc/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/cd/
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/cd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/cd/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/ce/
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ce/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/cf/
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/cf/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/da/
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/da/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/da/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/db/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/db/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/dc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/dc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/dc/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/e1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e1/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/e2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e2/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/e3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e3/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/e6/
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e6/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/e8/
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e8/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/ea/
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ea/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/ec/
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ec/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/ed/
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ed/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fa/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midealocal/devices/fb/
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fb/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midealocal/devices/fc/
+-rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fc/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midealocal/devices/fd/
+-rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fd/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midealocal/devices/x13/
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x13/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midealocal/devices/x26/
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x26/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x26/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midealocal/devices/x34/
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x34/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x34/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midealocal/devices/x40/
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x40/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x40/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/discover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/packet_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:42:57.129418 midea_local-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-23 17:42:49.000000 midea_local-1.0.3/setup.py
```

### Comparing `midea_local-1.0.2/LICENSE` & `midea_local-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/PKG-INFO` & `midea_local-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midea-local
-Version: 1.0.2
+Version: 1.0.3
 Summary: Control your Midea M-Smart appliances via local area network
 Home-page: https://github.com/rokam/midea-local
 Author: rokam
 Author-email: lucas@mindello.com.br
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `midea_local-1.0.2/README.md` & `midea_local-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midea_local.egg-info/PKG-INFO` & `midea_local-1.0.3/midea_local.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midea-local
-Version: 1.0.2
+Version: 1.0.3
 Summary: Control your Midea M-Smart appliances via local area network
 Home-page: https://github.com/rokam/midea-local
 Author: rokam
 Author-email: lucas@mindello.com.br
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `midea_local-1.0.2/midea_local.egg-info/SOURCES.txt` & `midea_local-1.0.3/midea_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/backports/enum.py` & `midea_local-1.0.3/midealocal/backports/enum.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/cloud.py` & `midea_local-1.0.3/midealocal/cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
         ):
             appliances = {}
             for home in response.get("homeList") or []:
                 for room in home.get("roomList") or []:
                     for appliance in room.get("applianceList"):
                         try:
                             model_number = int(appliance.get("modelNumber", 0))
-                        except ValueError:
+                        except (ValueError, TypeError):
                             model_number = 0
                         device_info = {
                             "name": appliance.get("name"),
                             "type": int(appliance.get("type"), 16),
                             "sn": (
                                 self._security.aes_decrypt(appliance.get("sn"))
                                 if appliance.get("sn")
```

### Comparing `midea_local-1.0.2/midealocal/crc8.py` & `midea_local-1.0.3/midealocal/crc8.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/device.py` & `midea_local-1.0.3/midealocal/device.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/__init__.py` & `midea_local-1.0.3/midealocal/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/a1/__init__.py` & `midea_local-1.0.3/midealocal/devices/a1/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/a1/message.py` & `midea_local-1.0.3/midealocal/devices/a1/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/ac/__init__.py` & `midea_local-1.0.3/midealocal/devices/ac/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/ac/message.py` & `midea_local-1.0.3/midealocal/devices/ac/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/b0/__init__.py` & `midea_local-1.0.3/midealocal/devices/b0/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/b0/message.py` & `midea_local-1.0.3/midealocal/devices/b0/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/b1/__init__.py` & `midea_local-1.0.3/midealocal/devices/b1/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/b1/message.py` & `midea_local-1.0.3/midealocal/devices/b1/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/b3/__init__.py` & `midea_local-1.0.3/midealocal/devices/b3/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/b3/message.py` & `midea_local-1.0.3/midealocal/devices/b3/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/b4/__init__.py` & `midea_local-1.0.3/midealocal/devices/b4/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/b4/message.py` & `midea_local-1.0.3/midealocal/devices/b4/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/b6/__init__.py` & `midea_local-1.0.3/midealocal/devices/b6/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/b6/message.py` & `midea_local-1.0.3/midealocal/devices/b6/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/bf/__init__.py` & `midea_local-1.0.3/midealocal/devices/bf/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/bf/message.py` & `midea_local-1.0.3/midealocal/devices/bf/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/c2/__init__.py` & `midea_local-1.0.3/midealocal/devices/c2/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/c2/message.py` & `midea_local-1.0.3/midealocal/devices/c2/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/c3/__init__.py` & `midea_local-1.0.3/midealocal/devices/c3/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/c3/message.py` & `midea_local-1.0.3/midealocal/devices/c3/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/ca/__init__.py` & `midea_local-1.0.3/midealocal/devices/ca/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/ca/message.py` & `midea_local-1.0.3/midealocal/devices/ca/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/cc/__init__.py` & `midea_local-1.0.3/midealocal/devices/cc/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/cc/message.py` & `midea_local-1.0.3/midealocal/devices/cc/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/cd/__init__.py` & `midea_local-1.0.3/midealocal/devices/cd/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/cd/message.py` & `midea_local-1.0.3/midealocal/devices/cd/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/ce/__init__.py` & `midea_local-1.0.3/midealocal/devices/ce/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/ce/message.py` & `midea_local-1.0.3/midealocal/devices/ce/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/cf/__init__.py` & `midea_local-1.0.3/midealocal/devices/cf/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/cf/message.py` & `midea_local-1.0.3/midealocal/devices/cf/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/da/__init__.py` & `midea_local-1.0.3/midealocal/devices/da/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/da/message.py` & `midea_local-1.0.3/midealocal/devices/da/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/db/__init__.py` & `midea_local-1.0.3/midealocal/devices/db/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/db/message.py` & `midea_local-1.0.3/midealocal/devices/db/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/dc/__init__.py` & `midea_local-1.0.3/midealocal/devices/dc/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/dc/message.py` & `midea_local-1.0.3/midealocal/devices/dc/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/e1/__init__.py` & `midea_local-1.0.3/midealocal/devices/e1/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/e1/message.py` & `midea_local-1.0.3/midealocal/devices/e1/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/e2/__init__.py` & `midea_local-1.0.3/midealocal/devices/e2/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/e2/message.py` & `midea_local-1.0.3/midealocal/devices/e2/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/e3/__init__.py` & `midea_local-1.0.3/midealocal/devices/e3/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/e3/message.py` & `midea_local-1.0.3/midealocal/devices/e3/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/e6/__init__.py` & `midea_local-1.0.3/midealocal/devices/e6/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/e6/message.py` & `midea_local-1.0.3/midealocal/devices/e6/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/e8/__init__.py` & `midea_local-1.0.3/midealocal/devices/e8/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/e8/message.py` & `midea_local-1.0.3/midealocal/devices/e8/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/ea/__init__.py` & `midea_local-1.0.3/midealocal/devices/ea/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/ea/message.py` & `midea_local-1.0.3/midealocal/devices/ea/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/ec/__init__.py` & `midea_local-1.0.3/midealocal/devices/ec/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/ec/message.py` & `midea_local-1.0.3/midealocal/devices/ec/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/ed/__init__.py` & `midea_local-1.0.3/midealocal/devices/ed/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/ed/message.py` & `midea_local-1.0.3/midealocal/devices/ed/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/fa/__init__.py` & `midea_local-1.0.3/midealocal/devices/fa/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/fa/message.py` & `midea_local-1.0.3/midealocal/devices/fa/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/fb/__init__.py` & `midea_local-1.0.3/midealocal/devices/fb/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/fb/message.py` & `midea_local-1.0.3/midealocal/devices/fb/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/fc/__init__.py` & `midea_local-1.0.3/midealocal/devices/fc/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/fc/message.py` & `midea_local-1.0.3/midealocal/devices/fc/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/fd/__init__.py` & `midea_local-1.0.3/midealocal/devices/fd/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/fd/message.py` & `midea_local-1.0.3/midealocal/devices/fd/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/x13/__init__.py` & `midea_local-1.0.3/midealocal/devices/x13/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/x13/message.py` & `midea_local-1.0.3/midealocal/devices/x13/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/x26/__init__.py` & `midea_local-1.0.3/midealocal/devices/x26/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/x26/message.py` & `midea_local-1.0.3/midealocal/devices/x26/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/x34/__init__.py` & `midea_local-1.0.3/midealocal/devices/x34/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/x34/message.py` & `midea_local-1.0.3/midealocal/devices/x34/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/x40/__init__.py` & `midea_local-1.0.3/midealocal/devices/x40/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/devices/x40/message.py` & `midea_local-1.0.3/midealocal/devices/x40/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/discover.py` & `midea_local-1.0.3/midealocal/discover.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/message.py` & `midea_local-1.0.3/midealocal/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/packet_builder.py` & `midea_local-1.0.3/midealocal/packet_builder.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/midealocal/security.py` & `midea_local-1.0.3/midealocal/security.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.2/setup.py` & `midea_local-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 requires = ["aiohttp", "ifaddr", "pycryptodome"]
 
 setuptools.setup(
     name="midea-local",
-    version="1.0.2",
+    version="1.0.3",
     author="rokam",
     author_email="lucas@mindello.com.br",
     description="Control your Midea M-Smart appliances via local area network",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rokam/midea-local",
```

