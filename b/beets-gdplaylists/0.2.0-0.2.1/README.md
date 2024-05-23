# Comparing `tmp/beets_gdplaylists-0.2.0.tar.gz` & `tmp/beets_gdplaylists-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beets_gdplaylists-0.2.0.tar", last modified: Wed May 22 20:48:26 2024, max compression
+gzip compressed data, was "beets_gdplaylists-0.2.1.tar", last modified: Thu May 23 20:34:41 2024, max compression
```

## Comparing `beets_gdplaylists-0.2.0.tar` & `beets_gdplaylists-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:48:26.709548 beets_gdplaylists-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-22 20:48:26.709548 beets_gdplaylists-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:48:26.709548 beets_gdplaylists-0.2.0/beets_gdplaylists.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-22 20:48:26.000000 beets_gdplaylists-0.2.0/beets_gdplaylists.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-22 20:48:26.000000 beets_gdplaylists-0.2.0/beets_gdplaylists.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:48:26.000000 beets_gdplaylists-0.2.0/beets_gdplaylists.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 20:48:26.000000 beets_gdplaylists-0.2.0/beets_gdplaylists.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 20:48:26.000000 beets_gdplaylists-0.2.0/beets_gdplaylists.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:48:26.701548 beets_gdplaylists-0.2.0/beetsplug/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:48:26.705548 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/gdplex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:48:26.709548 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1971-10-24.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1971-11-20.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1971-12-09.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1971-12-10.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1972-09-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1972-09-09.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1972-09-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1972-10-17.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1972-10-18.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1972-10-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1973-06-22.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1973-06-24.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1973-06-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1973-10-29.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1973-10-30.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1974-05-17.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1974-05-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1974-05-21.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1977-05-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1977-05-04.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1977-10-01.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1977-10-02.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1979-12-04.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1979-12-09.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1985-04-27.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1985-04-28.yml
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:48:26.709548 beets_gdplaylists-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-22 20:48:18.000000 beets_gdplaylists-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:34:41.974075 beets_gdplaylists-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-23 20:34:41.974075 beets_gdplaylists-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:34:41.974075 beets_gdplaylists-0.2.1/beets_gdplaylists.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-23 20:34:41.000000 beets_gdplaylists-0.2.1/beets_gdplaylists.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-23 20:34:41.000000 beets_gdplaylists-0.2.1/beets_gdplaylists.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:34:41.000000 beets_gdplaylists-0.2.1/beets_gdplaylists.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-23 20:34:41.000000 beets_gdplaylists-0.2.1/beets_gdplaylists.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 20:34:41.000000 beets_gdplaylists-0.2.1/beets_gdplaylists.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:34:41.962075 beets_gdplaylists-0.2.1/beetsplug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:34:41.966075 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/gdplex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:34:41.974075 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1969-11-02.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1969-12-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1971-10-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1971-11-20.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1971-12-09.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1971-12-10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1972-09-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1972-09-09.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1972-09-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1972-10-17.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1972-10-18.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1972-10-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1973-06-22.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1973-06-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1973-06-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1973-09-07.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1973-09-08.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1973-10-29.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1973-10-30.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1974-02-22.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1974-02-23.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1974-05-17.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1974-05-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1974-05-21.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1977-05-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1977-05-04.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1977-05-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1977-10-01.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1977-10-02.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1978-04-15.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1978-04-18.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1979-12-04.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1979-12-09.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1983-04-15.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1983-04-25.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1983-04-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1984-04-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1984-04-20.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1985-04-27.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1985-04-28.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1987-03-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1987-03-27.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1990-06-23.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1990-07-18.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1990-07-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:34:41.974075 beets_gdplaylists-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-23 20:34:28.000000 beets_gdplaylists-0.2.1/setup.py
```

### Comparing `beets_gdplaylists-0.2.0/LICENSE` & `beets_gdplaylists-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/PKG-INFO` & `beets_gdplaylists-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-gdplaylists
-Version: 0.2.0
+Version: 0.2.1
 Summary: beets plugin to create Grateful Dead playlists
 Author-email: Ross Hendry <rhendry@gmail.com>
 Project-URL: Repository, https://github.com/chooban/beets-gogd
 Keywords: beets,grateful dead,plex,playlists
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `beets_gdplaylists-0.2.0/beets_gdplaylists.egg-info/PKG-INFO` & `beets_gdplaylists-0.2.1/beets_gdplaylists.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-gdplaylists
-Version: 0.2.0
+Version: 0.2.1
 Summary: beets plugin to create Grateful Dead playlists
 Author-email: Ross Hendry <rhendry@gmail.com>
 Project-URL: Repository, https://github.com/chooban/beets-gogd
 Keywords: beets,grateful dead,plex,playlists
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/gdplex.py` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/gdplex.py`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1971-10-24.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1971-10-24.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1971-11-20.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1971-11-20.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1971-12-09.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1971-12-09.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1971-12-10.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1971-12-10.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1972-09-03.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1972-09-03.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1972-09-09.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1972-09-09.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1972-09-19.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1972-09-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1972-10-17.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1972-10-17.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1972-10-18.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1972-10-18.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1972-10-19.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1972-10-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1973-06-22.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1973-06-22.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1973-06-24.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1973-06-24.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1973-06-26.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1973-06-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1973-10-29.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1973-10-29.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1973-10-30.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1973-10-30.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1974-05-17.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1974-05-17.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1974-05-19.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1974-05-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1974-05-21.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1974-05-21.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1977-05-03.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1977-05-03.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1977-05-04.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1977-05-04.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1977-10-01.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1977-10-01.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1977-10-02.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1977-10-02.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1979-12-04.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1979-12-04.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1979-12-09.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1979-12-09.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1985-04-27.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1985-04-27.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/beetsplug/gdplaylists/playlists/1985-04-28.yml` & `beets_gdplaylists-0.2.1/beetsplug/gdplaylists/playlists/1985-04-28.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.0/pyproject.toml` & `beets_gdplaylists-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="beets-gdplaylists"
-version="0.2.0"
+version="0.2.1"
 dynamic=["dependencies"]
 description="beets plugin to create Grateful Dead playlists"
 readme="README.md"
 authors=[{name="Ross Hendry", email="rhendry@gmail.com"}]
 keywords=["beets", "grateful dead", "plex", "playlists"]
 classifiers=[
   'Topic :: Multimedia :: Sound/Audio',
```

