# Comparing `tmp/watchdog-3.0.0.tar.gz` & `tmp/watchdog-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchdog-3.0.0.tar", last modified: Mon Mar 20 09:09:43 2023, max compression
+gzip compressed data, was "watchdog-4.0.0.tar", last modified: Tue Feb  6 23:46:22 2024, max compression
```

## Comparing `watchdog-3.0.0.tar` & `watchdog-4.0.0.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:09:43.005191 watchdog-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-03-20 09:09:40.000000 watchdog-3.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-20 09:09:40.000000 watchdog-3.0.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-20 09:09:40.000000 watchdog-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-20 09:09:40.000000 watchdog-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    36459 2023-03-20 09:09:43.005191 watchdog-3.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     8467 2023-03-20 09:09:40.000000 watchdog-3.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25634 2023-03-20 09:09:40.000000 watchdog-3.0.0/changelog.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:09:42.993191 watchdog-3.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-03-20 09:09:40.000000 watchdog-3.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    16410 2023-03-20 09:09:40.000000 watchdog-3.0.0/docs/eclipse_cdt_style.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-03-20 09:09:40.000000 watchdog-3.0.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:09:42.997191 watchdog-3.0.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-20 09:09:40.000000 watchdog-3.0.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-03-20 09:09:40.000000 watchdog-3.0.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:09:42.997191 watchdog-3.0.0/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-20 09:09:40.000000 watchdog-3.0.0/docs/source/examples/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-20 09:09:40.000000 watchdog-3.0.0/docs/source/examples/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-20 09:09:40.000000 watchdog-3.0.0/docs/source/examples/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-20 09:09:40.000000 watchdog-3.0.0/docs/source/examples/tricks.json
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-20 09:09:40.000000 watchdog-3.0.0/docs/source/examples/tricks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-20 09:09:40.000000 watchdog-3.0.0/docs/source/global.rst.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-20 09:09:40.000000 watchdog-3.0.0/docs/source/hacking.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-20 09:09:40.000000 watchdog-3.0.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-03-20 09:09:40.000000 watchdog-3.0.0/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-03-20 09:09:40.000000 watchdog-3.0.0/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-20 09:09:40.000000 watchdog-3.0.0/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-20 09:09:43.009191 watchdog-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-03-20 09:09:40.000000 watchdog-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:09:42.997191 watchdog-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:09:42.997191 watchdog-3.0.0/src/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16579 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:09:43.001191 watchdog-3.0.0/src/watchdog/observers/
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/observers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/observers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14100 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/observers/fsevents.py
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/observers/fsevents2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/observers/inotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/observers/inotify_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19739 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/observers/inotify_c.py
--rw-r--r--   0 runner    (1001) docker     (123)    23950 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/observers/kqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/observers/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/observers/read_directory_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/observers/winapi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:09:43.001191 watchdog-3.0.0/src/watchdog/tricks/
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/tricks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:09:43.001191 watchdog-3.0.0/src/watchdog/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/utils/bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/utils/delayed_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/utils/dirsnapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/utils/echo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/utils/event_debouncer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/utils/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/utils/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/utils/process_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25210 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog/watchmedo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:09:42.997191 watchdog-3.0.0/src/watchdog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36459 2023-03-20 09:09:42.000000 watchdog-3.0.0/src/watchdog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-03-20 09:09:42.000000 watchdog-3.0.0/src/watchdog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 09:09:42.000000 watchdog-3.0.0/src/watchdog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-20 09:09:42.000000 watchdog-3.0.0/src/watchdog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 09:09:42.000000 watchdog-3.0.0/src/watchdog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-20 09:09:42.000000 watchdog-3.0.0/src/watchdog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-20 09:09:42.000000 watchdog-3.0.0/src/watchdog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    33438 2023-03-20 09:09:40.000000 watchdog-3.0.0/src/watchdog_fsevents.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 09:09:43.005191 watchdog-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_0_watchmedo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_delayed_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    23094 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_fsevents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_inotify_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_inotify_c.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_logging_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_observers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_observers_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_observers_winapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_pattern_matching_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_regex_matching_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_skip_repeats_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/test_snapshot_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-03-20 09:09:40.000000 watchdog-3.0.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-20 09:09:40.000000 watchdog-3.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:46:22.236496 watchdog-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-02-06 23:46:21.000000 watchdog-4.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-06 23:46:21.000000 watchdog-4.0.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-06 23:46:21.000000 watchdog-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-06 23:46:21.000000 watchdog-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    37531 2024-02-06 23:46:22.236496 watchdog-4.0.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8526 2024-02-06 23:46:21.000000 watchdog-4.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26654 2024-02-06 23:46:21.000000 watchdog-4.0.0/changelog.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:46:22.224496 watchdog-4.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-02-06 23:46:21.000000 watchdog-4.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    16410 2024-02-06 23:46:21.000000 watchdog-4.0.0/docs/eclipse_cdt_style.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-02-06 23:46:21.000000 watchdog-4.0.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:46:22.224496 watchdog-4.0.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-02-06 23:46:21.000000 watchdog-4.0.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-02-06 23:46:21.000000 watchdog-4.0.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:46:22.228496 watchdog-4.0.0/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-06 23:46:21.000000 watchdog-4.0.0/docs/source/examples/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-02-06 23:46:21.000000 watchdog-4.0.0/docs/source/examples/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-06 23:46:21.000000 watchdog-4.0.0/docs/source/examples/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-06 23:46:21.000000 watchdog-4.0.0/docs/source/examples/tricks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-06 23:46:21.000000 watchdog-4.0.0/docs/source/examples/tricks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-06 23:46:21.000000 watchdog-4.0.0/docs/source/global.rst.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-06 23:46:21.000000 watchdog-4.0.0/docs/source/hacking.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-02-06 23:46:21.000000 watchdog-4.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-02-06 23:46:21.000000 watchdog-4.0.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-02-06 23:46:21.000000 watchdog-4.0.0/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-06 23:46:21.000000 watchdog-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-06 23:46:21.000000 watchdog-4.0.0/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-02-06 23:46:22.236496 watchdog-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-02-06 23:46:21.000000 watchdog-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:46:22.228496 watchdog-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:46:22.228496 watchdog-4.0.0/src/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15551 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:46:22.232496 watchdog-4.0.0/src/watchdog/observers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/observers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/observers/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14049 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/observers/fsevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/observers/fsevents2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11254 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/observers/inotify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/observers/inotify_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19488 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/observers/inotify_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24030 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/observers/kqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/observers/polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/observers/read_directory_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/observers/winapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:46:22.232496 watchdog-4.0.0/src/watchdog/tricks/
+-rw-r--r--   0 runner    (1001) docker     (127)     9426 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/tricks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:46:22.232496 watchdog-4.0.0/src/watchdog/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/utils/bricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/utils/delayed_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15291 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/utils/dirsnapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/utils/echo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/utils/event_debouncer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/utils/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/utils/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/utils/process_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24980 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog/watchmedo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:46:22.228496 watchdog-4.0.0/src/watchdog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    37531 2024-02-06 23:46:22.000000 watchdog-4.0.0/src/watchdog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-02-06 23:46:22.000000 watchdog-4.0.0/src/watchdog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 23:46:22.000000 watchdog-4.0.0/src/watchdog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-06 23:46:22.000000 watchdog-4.0.0/src/watchdog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 23:46:22.000000 watchdog-4.0.0/src/watchdog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-06 23:46:22.000000 watchdog-4.0.0/src/watchdog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-06 23:46:22.000000 watchdog-4.0.0/src/watchdog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    33438 2024-02-06 23:46:21.000000 watchdog-4.0.0/src/watchdog_fsevents.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:46:22.236496 watchdog-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_0_watchmedo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_delayed_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20920 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_fsevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_inotify_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_inotify_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_logging_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_observers_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_observers_polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_observers_winapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_pattern_matching_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_regex_matching_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_skip_repeats_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/test_snapshot_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-02-06 23:46:21.000000 watchdog-4.0.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-06 23:46:21.000000 watchdog-4.0.0/tox.ini
```

### Comparing `watchdog-3.0.0/AUTHORS` & `watchdog-4.0.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/COPYING` & `watchdog-4.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/LICENSE` & `watchdog-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/PKG-INFO` & `watchdog-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchdog
-Version: 3.0.0
+Version: 4.0.0
 Summary: Filesystem events monitoring
 Home-page: https://github.com/gorakhargosh/watchdog
 Author: Yesudeep Mangalapilly
 Author-email: yesudeep@gmail.com
-License: Apache License 2.0
+License: Apache-2.0
 Project-URL: Documentation, https://python-watchdog.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/gorakhargosh/watchdog/
 Project-URL: Issues, https://github.com/gorakhargosh/watchdog/issues
 Project-URL: Changelog, https://github.com/gorakhargosh/watchdog/blob/master/changelog.rst
 Keywords: python filesystem monitoring monitor FSEvents kqueue inotify ReadDirectoryChangesW polling DirectorySnapshot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -26,41 +26,41 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: C
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: watchmedo
 License-File: LICENSE
 License-File: COPYING
 License-File: AUTHORS
 
 Watchdog
 ========
 
 |Build Status|
 |CirrusCI Status|
 
 Python API and shell utilities to monitor file system events.
 
-Works on 3.7+.
+Works on 3.8+.
 
 Example API Usage
 -----------------
 
 A simple program that uses watchdog to monitor directories specified
 as command-line arguments and logs events generated:
 
@@ -73,14 +73,15 @@
     from watchdog.events import LoggingEventHandler
 
     if __name__ == "__main__":
         logging.basicConfig(level=logging.INFO,
                             format='%(asctime)s - %(message)s',
                             datefmt='%Y-%m-%d %H:%M:%S')
         path = sys.argv[1] if len(sys.argv) > 1 else '.'
+        logging.info(f'start watching directory {path!r}')
         event_handler = LoggingEventHandler()
         observer = Observer()
         observer.schedule(event_handler, path, recursive=True)
         observer.start()
         try:
             while True:
                 time.sleep(1)
@@ -258,15 +259,15 @@
 
     from watchdog.observers.polling import PollingObserver as Observer
 
 
 Dependencies
 ------------
 
-1. Python 3.7 or above.
+1. Python 3.8 or above.
 2. XCode_ (only on macOS when installing from sources)
 3. PyYAML_ (only for ``watchmedo``)
 
 Licensing
 ---------
 
 Watchdog is licensed under the terms of the `Apache License, version 2.0`_.
@@ -327,14 +328,31 @@
 
 
 .. :changelog:
 
 Changelog
 ---------
 
+4.0.0
+~~~~~
+
+2024-02-06 • `full history <https://github.com/gorakhargosh/watchdog/compare/v3.0.0...v4.0.0>`__
+
+- Drop support for Python 3.7.
+- Add support for Python 3.12.
+- [snapshot] Add typing to ``dirsnapshot`` (`#1012 <https://github.com/gorakhargosh/watchdog/pull/1012>`__)
+- [snapshot] Added ``DirectorySnapshotDiff.ContextManager`` (`#1011 <https://github.com/gorakhargosh/watchdog/pull/1011>`__)
+- [events] ``FileSystemEvent``, and subclasses, are now ``dataclass``es, and their ``repr()`` has changed
+- [windows] ``WinAPINativeEvent`` is now a ``dataclass``, and its ``repr()`` has changed
+- [events] Log ``FileOpenedEvent``, and ``FileClosedEvent``, events in ``LoggingEventHandler``
+- [tests] Improve ``FileSystemEvent`` coverage
+- [watchmedo] Log all events in ``LoggerTrick``
+- [windows] The ``observers.read_directory_changes.WATCHDOG_TRAVERSE_MOVED_DIR_DELAY`` hack was removed. The constant will be kept to prevent breaking other softwares.
+- Thanks to our beloved contributors: @BoboTiG, @msabramo
+
 3.0.0
 ~~~~~
 
 2023-03-20 • `full history <https://github.com/gorakhargosh/watchdog/compare/v2.3.1...v3.0.0>`__
 
 - Drop support for Python 3.6.
 - ``watchdog`` is now PEP 561 compatible, and tested with ``mypy``
```

### Comparing `watchdog-3.0.0/README.rst` & `watchdog-4.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ========
 
 |Build Status|
 |CirrusCI Status|
 
 Python API and shell utilities to monitor file system events.
 
-Works on 3.7+.
+Works on 3.8+.
 
 Example API Usage
 -----------------
 
 A simple program that uses watchdog to monitor directories specified
 as command-line arguments and logs events generated:
 
@@ -23,14 +23,15 @@
     from watchdog.events import LoggingEventHandler
 
     if __name__ == "__main__":
         logging.basicConfig(level=logging.INFO,
                             format='%(asctime)s - %(message)s',
                             datefmt='%Y-%m-%d %H:%M:%S')
         path = sys.argv[1] if len(sys.argv) > 1 else '.'
+        logging.info(f'start watching directory {path!r}')
         event_handler = LoggingEventHandler()
         observer = Observer()
         observer.schedule(event_handler, path, recursive=True)
         observer.start()
         try:
             while True:
                 time.sleep(1)
@@ -208,15 +209,15 @@
 
     from watchdog.observers.polling import PollingObserver as Observer
 
 
 Dependencies
 ------------
 
-1. Python 3.7 or above.
+1. Python 3.8 or above.
 2. XCode_ (only on macOS when installing from sources)
 3. PyYAML_ (only for ``watchmedo``)
 
 Licensing
 ---------
 
 Watchdog is licensed under the terms of the `Apache License, version 2.0`_.
```

### Comparing `watchdog-3.0.0/changelog.rst` & `watchdog-4.0.0/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,29 @@
 .. :changelog:
 
 Changelog
 ---------
 
+4.0.0
+~~~~~
+
+2024-02-06 • `full history <https://github.com/gorakhargosh/watchdog/compare/v3.0.0...v4.0.0>`__
+
+- Drop support for Python 3.7.
+- Add support for Python 3.12.
+- [snapshot] Add typing to ``dirsnapshot`` (`#1012 <https://github.com/gorakhargosh/watchdog/pull/1012>`__)
+- [snapshot] Added ``DirectorySnapshotDiff.ContextManager`` (`#1011 <https://github.com/gorakhargosh/watchdog/pull/1011>`__)
+- [events] ``FileSystemEvent``, and subclasses, are now ``dataclass``es, and their ``repr()`` has changed
+- [windows] ``WinAPINativeEvent`` is now a ``dataclass``, and its ``repr()`` has changed
+- [events] Log ``FileOpenedEvent``, and ``FileClosedEvent``, events in ``LoggingEventHandler``
+- [tests] Improve ``FileSystemEvent`` coverage
+- [watchmedo] Log all events in ``LoggerTrick``
+- [windows] The ``observers.read_directory_changes.WATCHDOG_TRAVERSE_MOVED_DIR_DELAY`` hack was removed. The constant will be kept to prevent breaking other softwares.
+- Thanks to our beloved contributors: @BoboTiG, @msabramo
+
 3.0.0
 ~~~~~
 
 2023-03-20 • `full history <https://github.com/gorakhargosh/watchdog/compare/v2.3.1...v3.0.0>`__
 
 - Drop support for Python 3.6.
 - ``watchdog`` is now PEP 561 compatible, and tested with ``mypy``
```

### Comparing `watchdog-3.0.0/docs/Makefile` & `watchdog-4.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/docs/eclipse_cdt_style.xml` & `watchdog-4.0.0/docs/eclipse_cdt_style.xml`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/docs/make.bat` & `watchdog-4.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/docs/source/api.rst` & `watchdog-4.0.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/docs/source/conf.py` & `watchdog-4.0.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 SRC_DIR_PATH = os.path.join(TOP_DIR_PATH, "src")  # noqa
 sys.path.insert(0, SRC_DIR_PATH)  # noqa
 
 import watchdog.version  # noqa
 
 PROJECT_NAME = "watchdog"
 AUTHOR_NAME = "Yesudeep Mangalapilly and contributors"
-COPYRIGHT = "2010-2023, " + AUTHOR_NAME
+COPYRIGHT = f"2010-2024, {AUTHOR_NAME}"
 
 
 # -- General configuration -----------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
```

### Comparing `watchdog-3.0.0/docs/source/examples/patterns.py` & `watchdog-4.0.0/docs/source/examples/patterns.py`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/docs/source/examples/simple.py` & `watchdog-4.0.0/docs/source/examples/simple.py`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/docs/source/examples/tricks.json` & `watchdog-4.0.0/docs/source/examples/tricks.json`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/docs/source/examples/tricks.yaml` & `watchdog-4.0.0/docs/source/examples/tricks.yaml`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/docs/source/global.rst.inc` & `watchdog-4.0.0/docs/source/global.rst.inc`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. Global includes, substitutions, and common links.
 
 .. |author_name| replace:: Yesudeep Mangalapilly
 .. |author_email| replace:: yesudeep@gmail.com
-.. |copyright| replace:: Copyright 2012-2023 Google, Inc & contributors.
+.. |copyright| replace:: Copyright 2012-2024 Google, Inc & contributors.
 .. |project_name| replace:: ``watchdog``
-.. |project_version| replace:: 3.0.0
+.. |project_version| replace:: 4.0.0
 
 .. _issue tracker: https://github.com/gorakhargosh/watchdog/issues
 .. _code repository: https://github.com/gorakhargosh/watchdog
 
 .. _kqueue: https://www.freebsd.org/cgi/man.cgi?query=kqueue&sektion=2
 .. _FSEvents: https://developer.apple.com/library/mac/#documentation/Darwin/Conceptual/FSEvents_ProgGuide/Introduction/Introduction.html
 .. _inotify: https://linux.die.net/man/7/inotify
```

### Comparing `watchdog-3.0.0/docs/source/hacking.rst` & `watchdog-4.0.0/docs/source/hacking.rst`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/docs/source/index.rst` & `watchdog-4.0.0/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 Watchdog
 ========
 
 Python API library and shell utilities to monitor file system events.
 
-Works on 3.7+.
+Works on 3.8+.
 
 Directory monitoring made easy with
 -----------------------------------
 
 * A cross-platform API.
 
 * A shell tool to run commands in response to directory changes.
```

### Comparing `watchdog-3.0.0/docs/source/installation.rst` & `watchdog-4.0.0/docs/source/installation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. include:: global.rst.inc
 
 .. _installation:
 
 Installation
 ============
-|project_name| requires 3.7+ to work. See a list of :ref:`installation-dependencies`.
+|project_name| requires 3.8+ to work. See a list of :ref:`installation-dependencies`.
 
 Installing from PyPI using pip
 ------------------------------
 
 .. parsed-literal::
 
     $ python -m pip install -U |project_name|
```

### Comparing `watchdog-3.0.0/docs/source/quickstart.rst` & `watchdog-4.0.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/setup.cfg` & `watchdog-4.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/setup.py` & `watchdog-4.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     name="watchdog",
     version=version.VERSION_STRING,
     description="Filesystem events monitoring",
     long_description=readme + "\n\n" + changelog,
     long_description_content_type="text/x-rst",
     author="Yesudeep Mangalapilly",
     author_email="yesudeep@gmail.com",
-    license="Apache License 2.0",
+    license="Apache-2.0",
     url="https://github.com/gorakhargosh/watchdog",
     keywords=" ".join(
         [
             "python",
             "filesystem",
             "monitoring",
             "monitor",
@@ -125,19 +125,19 @@
         "Operating System :: Microsoft :: Windows :: Windows 8.1",
         "Operating System :: Microsoft :: Windows :: Windows 10",
         "Operating System :: Microsoft :: Windows :: Windows 11",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Programming Language :: C",
         "Topic :: Software Development :: Libraries",
         "Topic :: System :: Monitoring",
         "Topic :: System :: Filesystems",
         "Topic :: Utilities",
     ],
@@ -150,10 +150,10 @@
     },
     ext_modules=ext_modules,
     entry_points={
         "console_scripts": [
             "watchmedo = watchdog.watchmedo:main [watchmedo]",
         ]
     },
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     zip_safe=False,
 )
```

### Comparing `watchdog-3.0.0/src/watchdog/__init__.py` & `watchdog-4.0.0/src/watchdog/__init__.py`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/src/watchdog/events.py` & `watchdog-4.0.0/src/watchdog/events.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,107 +92,55 @@
 """
 
 from __future__ import annotations
 
 import logging
 import os.path
 import re
+from dataclasses import dataclass, field
+from typing import Optional
 
 from watchdog.utils.patterns import match_any_paths
 
 EVENT_TYPE_MOVED = "moved"
 EVENT_TYPE_DELETED = "deleted"
 EVENT_TYPE_CREATED = "created"
 EVENT_TYPE_MODIFIED = "modified"
 EVENT_TYPE_CLOSED = "closed"
 EVENT_TYPE_OPENED = "opened"
 
 
+@dataclass(unsafe_hash=True)
 class FileSystemEvent:
     """
     Immutable type that represents a file system event that is triggered
     when a change occurs on the monitored file system.
 
     All FileSystemEvent objects are required to be immutable and hence
     can be used as keys in dictionaries or be added to sets.
     """
 
-    event_type = ""
-    """The type of the event as a string."""
+    src_path: str
+    dest_path: str = ""
+    event_type: str = field(default="", init=False)
+    is_directory: bool = field(default=False, init=False)
 
-    is_directory = False
-    """True if event was emitted for a directory; False otherwise."""
-
-    is_synthetic = False
     """
     True if event was synthesized; False otherwise.
-
     These are events that weren't actually broadcast by the OS, but
     are presumed to have happened based on other, actual events.
     """
-
-    def __init__(self, src_path):
-        self._src_path = src_path
-
-    @property
-    def src_path(self):
-        """Source path of the file system object that triggered this event."""
-        return self._src_path
-
-    def __str__(self):
-        return self.__repr__()
-
-    def __repr__(self):
-        return (
-            f"<{type(self).__name__}: event_type={self.event_type}, "
-            f"src_path={self.src_path!r}, is_directory={self.is_directory}>"
-        )
-
-    # Used for comparison of events.
-    @property
-    def key(self):
-        return (self.event_type, self.src_path, self.is_directory)
-
-    def __eq__(self, event):
-        return self.key == event.key
-
-    def __ne__(self, event):
-        return self.key != event.key
-
-    def __hash__(self):
-        return hash(self.key)
+    is_synthetic: bool = field(default=False)
 
 
 class FileSystemMovedEvent(FileSystemEvent):
-    """
-    File system event representing any kind of file system movement.
-    """
+    """File system event representing any kind of file system movement."""
 
     event_type = EVENT_TYPE_MOVED
 
-    def __init__(self, src_path, dest_path):
-        super().__init__(src_path)
-        self._dest_path = dest_path
-
-    @property
-    def dest_path(self):
-        """The destination path of the move event."""
-        return self._dest_path
-
-    # Used for hashing this as an immutable object.
-    @property
-    def key(self):
-        return (self.event_type, self.src_path, self.dest_path, self.is_directory)
-
-    def __repr__(self):
-        return (
-            f"<{type(self).__name__}: src_path={self.src_path!r}, "
-            f"dest_path={self.dest_path!r}, is_directory={self.is_directory}>"
-        )
-
 
 # File events.
 
 
 class FileDeletedEvent(FileSystemEvent):
     """File system event representing file deletion on the file system."""
 
@@ -260,15 +208,15 @@
 
 
 class FileSystemEventHandler:
     """
     Base file system event handler that you can override methods from.
     """
 
-    def dispatch(self, event):
+    def dispatch(self, event: FileSystemEvent) -> None:
         """Dispatches events to the appropriate methods.
 
         :param event:
             The event object representing the file system event.
         :type event:
             :class:`FileSystemEvent`
         """
@@ -278,69 +226,69 @@
             EVENT_TYPE_DELETED: self.on_deleted,
             EVENT_TYPE_MODIFIED: self.on_modified,
             EVENT_TYPE_MOVED: self.on_moved,
             EVENT_TYPE_CLOSED: self.on_closed,
             EVENT_TYPE_OPENED: self.on_opened,
         }[event.event_type](event)
 
-    def on_any_event(self, event):
+    def on_any_event(self, event: FileSystemEvent) -> None:
         """Catch-all event handler.
 
         :param event:
             The event object representing the file system event.
         :type event:
             :class:`FileSystemEvent`
         """
 
-    def on_moved(self, event):
+    def on_moved(self, event: FileSystemEvent) -> None:
         """Called when a file or a directory is moved or renamed.
 
         :param event:
             Event representing file/directory movement.
         :type event:
             :class:`DirMovedEvent` or :class:`FileMovedEvent`
         """
 
-    def on_created(self, event):
+    def on_created(self, event: FileSystemEvent) -> None:
         """Called when a file or directory is created.
 
         :param event:
             Event representing file/directory creation.
         :type event:
             :class:`DirCreatedEvent` or :class:`FileCreatedEvent`
         """
 
-    def on_deleted(self, event):
+    def on_deleted(self, event: FileSystemEvent) -> None:
         """Called when a file or directory is deleted.
 
         :param event:
             Event representing file/directory deletion.
         :type event:
             :class:`DirDeletedEvent` or :class:`FileDeletedEvent`
         """
 
-    def on_modified(self, event):
+    def on_modified(self, event: FileSystemEvent) -> None:
         """Called when a file or directory is modified.
 
         :param event:
             Event representing file/directory modification.
         :type event:
             :class:`DirModifiedEvent` or :class:`FileModifiedEvent`
         """
 
-    def on_closed(self, event):
+    def on_closed(self, event: FileSystemEvent) -> None:
         """Called when a file opened for writing is closed.
 
         :param event:
             Event representing file closing.
         :type event:
             :class:`FileClosedEvent`
         """
 
-    def on_opened(self, event):
+    def on_opened(self, event: FileSystemEvent) -> None:
         """Called when a file is opened.
 
         :param event:
             Event representing file opening.
         :type event:
             :class:`FileOpenedEvent`
         """
@@ -394,15 +342,15 @@
         """
         (Read-only)
         ``True`` if path names should be matched sensitive to case; ``False``
         otherwise.
         """
         return self._case_sensitive
 
-    def dispatch(self, event):
+    def dispatch(self, event: FileSystemEvent) -> None:
         """Dispatches events to the appropriate methods.
 
         :param event:
             The event object representing the file system event.
         :type event:
             :class:`FileSystemEvent`
         """
@@ -482,15 +430,15 @@
         """
         (Read-only)
         ``True`` if path names should be matched sensitive to case; ``False``
         otherwise.
         """
         return self._case_sensitive
 
-    def dispatch(self, event):
+    def dispatch(self, event: FileSystemEvent) -> None:
         """Dispatches events to the appropriate methods.
 
         :param event:
             The event object representing the file system event.
         :type event:
             :class:`FileSystemEvent`
         """
@@ -509,45 +457,52 @@
         if any(r.match(p) for r in self.regexes for p in paths):
             super().dispatch(event)
 
 
 class LoggingEventHandler(FileSystemEventHandler):
     """Logs all the events captured."""
 
-    def __init__(self, logger=None):
+    def __init__(self, logger: Optional[logging.Logger] = None) -> None:
         super().__init__()
-
         self.logger = logger or logging.root
 
-    def on_moved(self, event):
+    def on_moved(self, event: FileSystemEvent) -> None:
         super().on_moved(event)
 
         what = "directory" if event.is_directory else "file"
-        self.logger.info(
-            "Moved %s: from %s to %s", what, event.src_path, event.dest_path
-        )
+        self.logger.info("Moved %s: from %s to %s", what, event.src_path, event.dest_path)
 
-    def on_created(self, event):
+    def on_created(self, event: FileSystemEvent) -> None:
         super().on_created(event)
 
         what = "directory" if event.is_directory else "file"
         self.logger.info("Created %s: %s", what, event.src_path)
 
-    def on_deleted(self, event):
+    def on_deleted(self, event: FileSystemEvent) -> None:
         super().on_deleted(event)
 
         what = "directory" if event.is_directory else "file"
         self.logger.info("Deleted %s: %s", what, event.src_path)
 
-    def on_modified(self, event):
+    def on_modified(self, event: FileSystemEvent) -> None:
         super().on_modified(event)
 
         what = "directory" if event.is_directory else "file"
         self.logger.info("Modified %s: %s", what, event.src_path)
 
+    def on_closed(self, event: FileSystemEvent) -> None:
+        super().on_closed(event)
+
+        self.logger.info("Closed file: %s", event.src_path)
+
+    def on_opened(self, event: FileSystemEvent) -> None:
+        super().on_opened(event)
+
+        self.logger.info("Opened file: %s", event.src_path)
+
 
 def generate_sub_moved_events(src_dir_path, dest_dir_path):
     """Generates an event list of :class:`DirMovedEvent` and
     :class:`FileMovedEvent` objects for all the files and directories within
     the given moved directory that were moved along with the directory.
 
     :param src_dir_path:
@@ -557,28 +512,20 @@
     :returns:
         An iterable of file system events of type :class:`DirMovedEvent` and
         :class:`FileMovedEvent`.
     """
     for root, directories, filenames in os.walk(dest_dir_path):
         for directory in directories:
             full_path = os.path.join(root, directory)
-            renamed_path = (
-                full_path.replace(dest_dir_path, src_dir_path) if src_dir_path else None
-            )
-            dir_moved_event = DirMovedEvent(renamed_path, full_path)
-            dir_moved_event.is_synthetic = True
-            yield dir_moved_event
+            renamed_path = full_path.replace(dest_dir_path, src_dir_path) if src_dir_path else ""
+            yield DirMovedEvent(renamed_path, full_path, is_synthetic=True)
         for filename in filenames:
             full_path = os.path.join(root, filename)
-            renamed_path = (
-                full_path.replace(dest_dir_path, src_dir_path) if src_dir_path else None
-            )
-            file_moved_event = FileMovedEvent(renamed_path, full_path)
-            file_moved_event.is_synthetic = True
-            yield file_moved_event
+            renamed_path = full_path.replace(dest_dir_path, src_dir_path) if src_dir_path else ""
+            yield FileMovedEvent(renamed_path, full_path, is_synthetic=True)
 
 
 def generate_sub_created_events(src_dir_path):
     """Generates an event list of :class:`DirCreatedEvent` and
     :class:`FileCreatedEvent` objects for all the files and directories within
     the given moved directory that were moved along with the directory.
 
@@ -586,14 +533,10 @@
         The source path of the created directory.
     :returns:
         An iterable of file system events of type :class:`DirCreatedEvent` and
         :class:`FileCreatedEvent`.
     """
     for root, directories, filenames in os.walk(src_dir_path):
         for directory in directories:
-            dir_created_event = DirCreatedEvent(os.path.join(root, directory))
-            dir_created_event.is_synthetic = True
-            yield dir_created_event
+            yield DirCreatedEvent(os.path.join(root, directory), is_synthetic=True)
         for filename in filenames:
-            file_created_event = FileCreatedEvent(os.path.join(root, filename))
-            file_created_event.is_synthetic = True
-            yield file_created_event
+            yield FileCreatedEvent(os.path.join(root, filename), is_synthetic=True)
```

### Comparing `watchdog-3.0.0/src/watchdog/observers/__init__.py` & `watchdog-4.0.0/src/watchdog/observers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 
 elif sys.platform.startswith("darwin"):
     try:
         from .fsevents import FSEventsObserver as Observer
     except Exception:
         try:
             from .kqueue import KqueueObserver as Observer
+
             warnings.warn("Failed to import fsevents. Fall back to kqueue")
         except Exception:
             from .polling import PollingObserver as Observer
 
             warnings.warn("Failed to import fsevents and kqueue. Fall back to polling.")
 
 elif sys.platform in ("dragonfly", "freebsd", "netbsd", "openbsd", "bsd"):
```

### Comparing `watchdog-3.0.0/src/watchdog/observers/api.py` & `watchdog-4.0.0/src/watchdog/observers/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,48 +39,61 @@
 class ObservedWatch:
     """An scheduled watch.
 
     :param path:
         Path string.
     :param recursive:
         ``True`` if watch is recursive; ``False`` otherwise.
+    :param event_filter:
+        Optional collection of :class:`watchdog.events.FileSystemEvent` to watch
     """
 
-    def __init__(self, path, recursive):
+    def __init__(self, path, recursive, event_filter=None):
         if isinstance(path, Path):
             self._path = str(path)
         else:
             self._path = path
         self._is_recursive = recursive
+        self._event_filter = frozenset(event_filter) if event_filter is not None else None
 
     @property
     def path(self):
         """The path that this watch monitors."""
         return self._path
 
     @property
     def is_recursive(self):
         """Determines whether subdirectories are watched for the path."""
         return self._is_recursive
 
     @property
+    def event_filter(self):
+        """Collection of event types watched for the path"""
+        return self._event_filter
+
+    @property
     def key(self):
-        return self.path, self.is_recursive
+        return self.path, self.is_recursive, self.event_filter
 
     def __eq__(self, watch):
         return self.key == watch.key
 
     def __ne__(self, watch):
         return self.key != watch.key
 
     def __hash__(self):
         return hash(self.key)
 
     def __repr__(self):
-        return f"<{type(self).__name__}: path={self.path!r}, is_recursive={self.is_recursive}>"
+        if self.event_filter is not None:
+            event_filter_str = "|".join(sorted(_cls.__name__ for _cls in self.event_filter))
+            event_filter_str = f", event_filter={event_filter_str}"
+        else:
+            event_filter_str = ""
+        return f"<{type(self).__name__}: path={self.path!r}, is_recursive={self.is_recursive}{event_filter_str}>"
 
 
 # Observer classes
 class EventEmitter(BaseThread):
     """
     Producer thread base class subclassed by event emitters
     that generate events and populate a queue with them.
@@ -93,21 +106,26 @@
         The watch to observe and produce events for.
     :type watch:
         :class:`ObservedWatch`
     :param timeout:
         Timeout (in seconds) between successive attempts at reading events.
     :type timeout:
         ``float``
+    :param event_filter:
+        Collection of event types to emit, or None for no filtering (default).
+    :type event_filter:
+        Optional[Iterable[:class:`watchdog.events.FileSystemEvent`]]
     """
 
-    def __init__(self, event_queue, watch, timeout=DEFAULT_EMITTER_TIMEOUT):
+    def __init__(self, event_queue, watch, timeout=DEFAULT_EMITTER_TIMEOUT, event_filter=None):
         super().__init__()
         self._event_queue = event_queue
         self._watch = watch
         self._timeout = timeout
+        self._event_filter = frozenset(event_filter) if event_filter is not None else None
 
     @property
     def timeout(self):
         """
         Blocking timeout for reading events.
         """
         return self._timeout
@@ -125,15 +143,16 @@
 
         :param event:
             Event to be queued.
         :type event:
             An instance of :class:`watchdog.events.FileSystemEvent`
             or a subclass.
         """
-        self._event_queue.put((event, self.watch))
+        if self._event_filter is None or any(isinstance(event, cls) for cls in self._event_filter):
+            self._event_queue.put((event, self.watch))
 
     def queue_events(self, timeout):
         """Override this method to populate the event queue with events
         per interval period.
 
         :param timeout:
             Timeout (in seconds) between successive attempts at
@@ -260,15 +279,15 @@
             try:
                 emitter.start()
             except Exception:
                 self._remove_emitter(emitter)
                 raise
         super().start()
 
-    def schedule(self, event_handler, path, recursive=False):
+    def schedule(self, event_handler, path, recursive=False, event_filter=None):
         """
         Schedules watching a path and calls appropriate methods specified
         in the given event handler in response to file system events.
 
         :param event_handler:
             An event handler instance that has appropriate event handling
             methods which will be called by the observer in response to
@@ -280,27 +299,30 @@
         :type path:
             ``str``
         :param recursive:
             ``True`` if events will be emitted for sub-directories
             traversed recursively; ``False`` otherwise.
         :type recursive:
             ``bool``
+        :param event_filter:
+            Collection of event types to emit, or None for no filtering (default).
+        :type event_filter:
+            Optional[Iterable[:class:`watchdog.events.FileSystemEvent`]]
         :return:
             An :class:`ObservedWatch` object instance representing
             a watch.
         """
         with self._lock:
-            watch = ObservedWatch(path, recursive)
+            watch = ObservedWatch(path, recursive, event_filter)
             self._add_handler_for_watch(event_handler, watch)
 
             # If we don't have an emitter for this watch already, create it.
             if self._emitter_for_watch.get(watch) is None:
-                emitter = self._emitter_class(
-                    event_queue=self.event_queue, watch=watch, timeout=self.timeout
-                )
+                emitter = self._emitter_class(event_queue=self.event_queue, watch=watch, timeout=self.timeout,
+                                              event_filter=event_filter)
                 if self.is_alive():
                     emitter.start()
                 self._add_emitter(emitter)
             self._watches.add(watch)
         return watch
 
     def add_handler_for_watch(self, event_handler, watch):
```

### Comparing `watchdog-3.0.0/src/watchdog/observers/fsevents.py` & `watchdog-4.0.0/src/watchdog/observers/fsevents.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 import logging
 import os
 import threading
 import time
 import unicodedata
 
-import _watchdog_fsevents as _fsevents  # type: ignore[import]
+import _watchdog_fsevents as _fsevents  # type: ignore[import-not-found]
 
 from watchdog.events import (
     DirCreatedEvent,
     DirDeletedEvent,
     DirModifiedEvent,
     DirMovedEvent,
     FileCreatedEvent,
@@ -58,14 +58,16 @@
         The event queue to fill with events.
     :param watch:
         A watch object representing the directory to monitor.
     :type watch:
         :class:`watchdog.observers.api.ObservedWatch`
     :param timeout:
         Read events blocking timeout (in seconds).
+    :param event_filter:
+        Collection of event types to emit, or None for no filtering (default).
     :param suppress_history:
         The FSEvents API may emit historic events up to 30 sec before the watch was
         started. When ``suppress_history`` is ``True``, those events will be suppressed
         by creating a directory snapshot of the watched path before starting the stream
         as a reference to suppress old events. Warning: This may result in significant
         memory usage in case of a large number of items in the watched path.
     :type timeout:
@@ -73,25 +75,24 @@
     """
 
     def __init__(
         self,
         event_queue,
         watch,
         timeout=DEFAULT_EMITTER_TIMEOUT,
+        event_filter=None,
         suppress_history=False,
     ):
-        super().__init__(event_queue, watch, timeout)
+        super().__init__(event_queue, watch, timeout, event_filter)
         self._fs_view = set()
         self.suppress_history = suppress_history
         self._start_time = 0.0
         self._starting_state = None
         self._lock = threading.Lock()
-        self._absolute_watch_path = os.path.realpath(
-            os.path.abspath(os.path.expanduser(self.watch.path))
-        )
+        self._absolute_watch_path = os.path.realpath(os.path.abspath(os.path.expanduser(self.watch.path)))
 
     def on_thread_stop(self):
         _fsevents.remove_watch(self.watch)
         _fsevents.stop(self)
 
     def queue_event(self, event):
         # fsevents defaults to be recursive, so if the watch was meant to be non-recursive then we need to drop
@@ -103,17 +104,15 @@
             if not self._is_recursive_event(event):
                 logger.debug("queue_event %s", event)
                 EventEmitter.queue_event(self, event)
             else:
                 logger.debug("drop event %s", event)
 
     def _is_recursive_event(self, event):
-        src_path = (
-            event.src_path if event.is_directory else os.path.dirname(event.src_path)
-        )
+        src_path = event.src_path if event.is_directory else os.path.dirname(event.src_path)
         if src_path == self._absolute_watch_path:
             return False
 
         if isinstance(event, (FileMovedEvent, DirMovedEvent)):
             # when moving something into the watch path we must always take the dirname,
             # otherwise we miss out on `DirMovedEvent`s
             dest_path = os.path.dirname(event.dest_path)
@@ -132,17 +131,15 @@
         self.queue_event(cls(src_path))
         self.queue_event(DirModifiedEvent(dirname))
 
     def _queue_modified_event(self, event, src_path, dirname):
         cls = DirModifiedEvent if event.is_directory else FileModifiedEvent
         self.queue_event(cls(src_path))
 
-    def _queue_renamed_event(
-        self, src_event, src_path, dst_path, src_dirname, dst_dirname
-    ):
+    def _queue_renamed_event(self, src_event, src_path, dst_path, src_dirname, dst_dirname):
         cls = DirMovedEvent if src_event.is_directory else FileMovedEvent
         dst_path = self._encode_path(dst_path)
         self.queue_event(cls(src_path, dst_path))
         self.queue_event(DirModifiedEvent(src_dirname))
         self.queue_event(DirModifiedEvent(dst_dirname))
 
     def _is_historic_created_event(self, event):
@@ -166,17 +163,15 @@
     def _is_meta_mod(event):
         """Returns True if the event indicates a change in metadata."""
         return event.is_inode_meta_mod or event.is_xattr_mod or event.is_owner_change
 
     def queue_events(self, timeout, events):
         if logger.getEffectiveLevel() <= logging.DEBUG:
             for event in events:
-                flags = ", ".join(
-                    attr for attr in dir(event) if getattr(event, attr) is True
-                )
+                flags = ", ".join(attr for attr in dir(event) if getattr(event, attr) is True)
                 logger.debug(f"{event}: {flags}")
 
         if time.monotonic() - self._start_time > 60:
             # Event history is no longer needed, let's free some memory.
             self._starting_state = None
 
         while events:
@@ -234,30 +229,26 @@
 
                 if event.is_modified or self._is_meta_mod(event):
                     self._queue_modified_event(event, src_path, src_dirname)
 
                 if event.is_renamed:
                     # Check if we have a corresponding destination event in the watched path.
                     dst_event = next(
-                        iter(
-                            e for e in events if e.is_renamed and e.inode == event.inode
-                        ),
+                        iter(e for e in events if e.is_renamed and e.inode == event.inode),
                         None,
                     )
 
                     if dst_event:
                         # Item was moved within the watched folder.
                         logger.debug("Destination event for rename is %s", dst_event)
 
                         dst_path = self._encode_path(dst_event.path)
                         dst_dirname = os.path.dirname(dst_path)
 
-                        self._queue_renamed_event(
-                            event, src_path, dst_path, src_dirname, dst_dirname
-                        )
+                        self._queue_renamed_event(event, src_path, dst_path, src_dirname, dst_dirname)
                         self._fs_view.add(event.inode)
 
                         for sub_event in generate_sub_moved_events(src_path, dst_path):
                             self.queue_event(sub_event)
 
                         # Process any coalesced flags for the dst_event.
```

### Comparing `watchdog-3.0.0/src/watchdog/observers/fsevents2.py` & `watchdog-4.0.0/src/watchdog/observers/fsevents2.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 import queue
 import unicodedata
 import warnings
 from threading import Thread
 from typing import List, Optional, Type
 
 # pyobjc
-import AppKit  # type: ignore[import]
-from FSEvents import (  # type: ignore[import]
+import AppKit  # type: ignore[import-not-found]
+from FSEvents import (  # type: ignore[import-not-found]
     CFRunLoopGetCurrent,
     CFRunLoopRun,
     CFRunLoopStop,
     FSEventStreamCreate,
     FSEventStreamInvalidate,
     FSEventStreamRelease,
     FSEventStreamScheduleWithRunLoop,
@@ -102,17 +102,15 @@
         )
         if self._stream_ref is None:
             raise OSError("FSEvents. Could not create stream.")
 
     def run(self):
         pool = AppKit.NSAutoreleasePool.alloc().init()
         self._run_loop = CFRunLoopGetCurrent()
-        FSEventStreamScheduleWithRunLoop(
-            self._stream_ref, self._run_loop, kCFRunLoopDefaultMode
-        )
+        FSEventStreamScheduleWithRunLoop(self._stream_ref, self._run_loop, kCFRunLoopDefaultMode)
         if not FSEventStreamStart(self._stream_ref):
             FSEventStreamInvalidate(self._stream_ref)
             FSEventStreamRelease(self._stream_ref)
             raise OSError("FSEvents. Could not start stream.")
 
         CFRunLoopRun()
         FSEventStreamStop(self._stream_ref)
@@ -122,21 +120,16 @@
         # Make sure waiting thread is notified
         self._queue.put(None)
 
     def stop(self):
         if self._run_loop is not None:
             CFRunLoopStop(self._run_loop)
 
-    def _callback(
-        self, streamRef, clientCallBackInfo, numEvents, eventPaths, eventFlags, eventIDs
-    ):
-        events = [
-            NativeEvent(path, flags, _id)
-            for path, flags, _id in zip(eventPaths, eventFlags, eventIDs)
-        ]
+    def _callback(self, streamRef, clientCallBackInfo, numEvents, eventPaths, eventFlags, eventIDs):
+        events = [NativeEvent(path, flags, _id) for path, flags, _id in zip(eventPaths, eventFlags, eventIDs)]
         logger.debug(f"FSEvents callback. Got {numEvents} events:")
         for e in events:
             logger.debug(e)
         self._queue.put(events)
 
     def read_events(self):
         """
@@ -188,16 +181,16 @@
 
 
 class FSEventsEmitter(EventEmitter):
     """
     FSEvents based event emitter. Handles conversion of native events.
     """
 
-    def __init__(self, event_queue, watch, timeout=DEFAULT_EMITTER_TIMEOUT):
-        super().__init__(event_queue, watch, timeout)
+    def __init__(self, event_queue, watch, timeout=DEFAULT_EMITTER_TIMEOUT, event_filter=None):
+        super().__init__(event_queue, watch, timeout, event_filter)
         self._fsevents = FSEventsQueue(watch.path)
         self._fsevents.start()
 
     def on_thread_stop(self):
         self._fsevents.stop()
 
     def queue_events(self, timeout):
@@ -215,25 +208,19 @@
             if event.is_renamed:
                 # Internal moves appears to always be consecutive in the same
                 # buffer and have IDs differ by exactly one (while others
                 # don't) making it possible to pair up the two events coming
                 # from a single move operation. (None of this is documented!)
                 # Otherwise, guess whether file was moved in or out.
                 # TODO: handle id wrapping
-                if (
-                    i + 1 < len(events)
-                    and events[i + 1].is_renamed
-                    and events[i + 1].event_id == event.event_id + 1
-                ):
+                if i + 1 < len(events) and events[i + 1].is_renamed and events[i + 1].event_id == event.event_id + 1:
                     cls = DirMovedEvent if event.is_directory else FileMovedEvent
                     self.queue_event(cls(event.path, events[i + 1].path))
                     self.queue_event(DirModifiedEvent(os.path.dirname(event.path)))
-                    self.queue_event(
-                        DirModifiedEvent(os.path.dirname(events[i + 1].path))
-                    )
+                    self.queue_event(DirModifiedEvent(os.path.dirname(events[i + 1].path)))
                     i += 1
                 elif os.path.exists(event.path):
                     cls = DirCreatedEvent if event.is_directory else FileCreatedEvent
                     self.queue_event(cls(event.path))
                     self.queue_event(DirModifiedEvent(os.path.dirname(event.path)))
                 else:
                     cls = DirDeletedEvent if event.is_directory else FileDeletedEvent
```

### Comparing `watchdog-3.0.0/src/watchdog/observers/inotify.py` & `watchdog-4.0.0/src/watchdog/observers/inotify.py`

 * *Files 16% similar despite different names*

```diff
@@ -85,14 +85,15 @@
     FileSystemEvent,
     generate_sub_created_events,
     generate_sub_moved_events,
 )
 from watchdog.observers.api import DEFAULT_EMITTER_TIMEOUT, DEFAULT_OBSERVER_TIMEOUT, BaseObserver, EventEmitter
 
 from .inotify_buffer import InotifyBuffer
+from .inotify_c import InotifyConstants
 
 logger = logging.getLogger(__name__)
 
 
 class InotifyEmitter(EventEmitter):
     """
     inotify(7)-based event emitter.
@@ -103,24 +104,29 @@
         A watch object representing the directory to monitor.
     :type watch:
         :class:`watchdog.observers.api.ObservedWatch`
     :param timeout:
         Read events blocking timeout (in seconds).
     :type timeout:
         ``float``
+    :param event_filter:
+        Collection of event types to emit, or None for no filtering (default).
+    :type event_filter:
+        Optional[Iterable[:class:`watchdog.events.FileSystemEvent`]]
     """
 
-    def __init__(self, event_queue, watch, timeout=DEFAULT_EMITTER_TIMEOUT):
-        super().__init__(event_queue, watch, timeout)
+    def __init__(self, event_queue, watch, timeout=DEFAULT_EMITTER_TIMEOUT, event_filter=None):
+        super().__init__(event_queue, watch, timeout, event_filter)
         self._lock = threading.Lock()
         self._inotify = None
 
     def on_thread_start(self):
         path = os.fsencode(self.watch.path)
-        self._inotify = InotifyBuffer(path, self.watch.is_recursive)
+        event_mask = self.get_event_mask_from_filter()
+        self._inotify = InotifyBuffer(path, self.watch.is_recursive, event_mask)
 
     def on_thread_stop(self):
         if self._inotify:
             self._inotify.close()
             self._inotify = None
 
     def queue_events(self, timeout, full_events=False):
@@ -151,15 +157,15 @@
                         self.queue_event(sub_event)
                 return
 
             src_path = self._decode_path(event.src_path)
             if event.is_moved_to:
                 if full_events:
                     cls = DirMovedEvent if event.is_directory else FileMovedEvent
-                    self.queue_event(cls(None, src_path))
+                    self.queue_event(cls("", src_path))
                 else:
                     cls = DirCreatedEvent if event.is_directory else FileCreatedEvent
                     self.queue_event(cls(src_path))
                 self.queue_event(DirModifiedEvent(os.path.dirname(src_path)))
                 if event.is_directory and self.watch.is_recursive:
                     for sub_event in generate_sub_created_events(src_path):
                         self.queue_event(sub_event)
@@ -171,15 +177,15 @@
                 self.queue_event(cls(src_path))
             elif event.is_delete or (event.is_moved_from and not full_events):
                 cls = DirDeletedEvent if event.is_directory else FileDeletedEvent
                 self.queue_event(cls(src_path))
                 self.queue_event(DirModifiedEvent(os.path.dirname(src_path)))
             elif event.is_moved_from and full_events:
                 cls = DirMovedEvent if event.is_directory else FileMovedEvent
-                self.queue_event(cls(src_path, None))
+                self.queue_event(cls(src_path, ""))
                 self.queue_event(DirModifiedEvent(os.path.dirname(src_path)))
             elif event.is_create:
                 cls = DirCreatedEvent if event.is_directory else FileCreatedEvent
                 self.queue_event(cls(src_path))
                 self.queue_event(DirModifiedEvent(os.path.dirname(src_path)))
             elif event.is_close_write and not event.is_directory:
                 cls = FileClosedEvent
@@ -198,14 +204,44 @@
 
     def _decode_path(self, path):
         """Decode path only if unicode string was passed to this emitter."""
         if isinstance(self.watch.path, bytes):
             return path
         return os.fsdecode(path)
 
+    def get_event_mask_from_filter(self):
+        """Optimization: Only include events we are filtering in inotify call"""
+        if self._event_filter is None:
+            return None
+
+        # always listen to delete self
+        event_mask = InotifyConstants.IN_DELETE_SELF
+        for cls in self._event_filter:
+            if cls in (DirMovedEvent, FileMovedEvent):
+                event_mask |= InotifyConstants.IN_MOVE
+            elif cls in (DirCreatedEvent, FileCreatedEvent):
+                event_mask |= InotifyConstants.IN_MOVE | InotifyConstants.IN_CREATE
+            elif cls is DirModifiedEvent:
+                event_mask |= (
+                    InotifyConstants.IN_MOVE
+                    | InotifyConstants.IN_ATTRIB
+                    | InotifyConstants.IN_MODIFY
+                    | InotifyConstants.IN_CREATE
+                    | InotifyConstants.IN_CLOSE_WRITE
+                )
+            elif cls is FileModifiedEvent:
+                event_mask |= InotifyConstants.IN_ATTRIB | InotifyConstants.IN_MODIFY
+            elif cls in (DirDeletedEvent, FileDeletedEvent):
+                event_mask |= InotifyConstants.IN_DELETE
+            elif cls is FileClosedEvent:
+                event_mask |= InotifyConstants.IN_CLOSE
+            elif cls is FileOpenedEvent:
+                event_mask |= InotifyConstants.IN_OPEN
+        return event_mask
+
 
 class InotifyFullEmitter(InotifyEmitter):
     """
     inotify(7)-based event emitter. By default this class produces move events even if they are not matched
     Such move events will have a ``None`` value for the unmatched part.
 
     :param event_queue:
```

### Comparing `watchdog-3.0.0/src/watchdog/observers/inotify_buffer.py` & `watchdog-4.0.0/src/watchdog/observers/inotify_buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 class InotifyBuffer(BaseThread):
     """A wrapper for `Inotify` that holds events for `delay` seconds. During
     this time, IN_MOVED_FROM and IN_MOVED_TO events are paired.
     """
 
     delay = 0.5
 
-    def __init__(self, path, recursive=False):
+    def __init__(self, path, recursive=False, event_mask=None):
         super().__init__()
         self._queue = DelayedQueue[InotifyEvent](self.delay)
-        self._inotify = Inotify(path, recursive)
+        self._inotify = Inotify(path, recursive, event_mask)
         self.start()
 
     def read_event(self):
         """Returns a single event or a tuple of from/to events in case of a
         paired move event. If this buffer has been closed, immediately return
         None.
         """
@@ -55,19 +55,15 @@
     def _group_events(self, event_list):
         """Group any matching move events"""
         grouped: List[Union[InotifyEvent, Tuple[InotifyEvent, InotifyEvent]]] = []
         for inotify_event in event_list:
             logger.debug("in-event %s", inotify_event)
 
             def matching_from_event(event):
-                return (
-                    not isinstance(event, tuple)
-                    and event.is_moved_from
-                    and event.cookie == inotify_event.cookie
-                )
+                return not isinstance(event, tuple) and event.is_moved_from and event.cookie == inotify_event.cookie
 
             if inotify_event.is_moved_to:
                 # Check if move_from is already in the buffer
                 for index, event in enumerate(grouped):
                     if matching_from_event(event):
                         if TYPE_CHECKING:
                             # this check is hidden from mypy inside matching_from_event()
@@ -100,17 +96,15 @@
                     if inotify_event.src_path == self._inotify.path:
                         # Watch was removed explicitly (inotify_rm_watch(2)) or automatically (file
                         # was deleted, or filesystem was unmounted), stop watching for events
                         deleted_self = True
                     continue
 
                 # Only add delay for unmatched move_from events
-                delay = (
-                    not isinstance(inotify_event, tuple) and inotify_event.is_moved_from
-                )
+                delay = not isinstance(inotify_event, tuple) and inotify_event.is_moved_from
                 self._queue.put(inotify_event, delay)
 
                 if (
                     not isinstance(inotify_event, tuple)
                     and inotify_event.is_delete_self
                     and inotify_event.src_path == self._inotify.path
                 ):
```

### Comparing `watchdog-3.0.0/src/watchdog/observers/inotify_c.py` & `watchdog-4.0.0/src/watchdog/observers/inotify_c.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,28 +24,20 @@
 from ctypes import c_char_p, c_int, c_uint32
 from functools import reduce
 
 from watchdog.utils import UnsupportedLibc
 
 libc = ctypes.CDLL(None)
 
-if (
-    not hasattr(libc, "inotify_init")
-    or not hasattr(libc, "inotify_add_watch")
-    or not hasattr(libc, "inotify_rm_watch")
-):
+if not hasattr(libc, "inotify_init") or not hasattr(libc, "inotify_add_watch") or not hasattr(libc, "inotify_rm_watch"):
     raise UnsupportedLibc(f"Unsupported libc version found: {libc._name}")
 
-inotify_add_watch = ctypes.CFUNCTYPE(c_int, c_int, c_char_p, c_uint32, use_errno=True)(
-    ("inotify_add_watch", libc)
-)
+inotify_add_watch = ctypes.CFUNCTYPE(c_int, c_int, c_char_p, c_uint32, use_errno=True)(("inotify_add_watch", libc))
 
-inotify_rm_watch = ctypes.CFUNCTYPE(c_int, c_int, c_uint32, use_errno=True)(
-    ("inotify_rm_watch", libc)
-)
+inotify_rm_watch = ctypes.CFUNCTYPE(c_int, c_int, c_uint32, use_errno=True)(("inotify_rm_watch", libc))
 
 inotify_init = ctypes.CFUNCTYPE(c_int, use_errno=True)(("inotify_init", libc))
 
 
 class InotifyConstants:
     # User-space events
     IN_ACCESS = 0x00000001  # File was accessed.
@@ -156,27 +148,30 @@
         The directory path for which we want an inotify object.
     :type path:
         :class:`bytes`
     :param recursive:
         ``True`` if subdirectories should be monitored; ``False`` otherwise.
     """
 
-    def __init__(self, path, recursive=False, event_mask=WATCHDOG_ALL_EVENTS):
+    def __init__(self, path, recursive=False, event_mask=None):
         # The file descriptor associated with the inotify instance.
         inotify_fd = inotify_init()
         if inotify_fd == -1:
             Inotify._raise_error()
         self._inotify_fd = inotify_fd
         self._lock = threading.Lock()
 
         # Stores the watch descriptor for a given path.
         self._wd_for_path = {}
         self._path_for_wd = {}
 
         self._path = path
+        # Default to all events
+        if event_mask is None:
+            event_mask = WATCHDOG_ALL_EVENTS
         self._event_mask = event_mask
         self._is_recursive = recursive
         if os.path.isdir(path):
             self._add_dir_watch(path, recursive, event_mask)
         else:
             self._add_watch(path, event_mask)
         self._moved_from_events = {}
@@ -316,55 +311,45 @@
 
         with self._lock:
             event_list = []
             for wd, mask, cookie, name in Inotify._parse_event_buffer(event_buffer):
                 if wd == -1:
                     continue
                 wd_path = self._path_for_wd[wd]
-                src_path = (
-                    os.path.join(wd_path, name) if name else wd_path
-                )  # avoid trailing slash
+                src_path = os.path.join(wd_path, name) if name else wd_path  # avoid trailing slash
                 inotify_event = InotifyEvent(wd, mask, cookie, name, src_path)
 
                 if inotify_event.is_moved_from:
                     self.remember_move_from_event(inotify_event)
                 elif inotify_event.is_moved_to:
                     move_src_path = self.source_for_move(inotify_event)
                     if move_src_path in self._wd_for_path:
                         moved_wd = self._wd_for_path[move_src_path]
                         del self._wd_for_path[move_src_path]
                         self._wd_for_path[inotify_event.src_path] = moved_wd
                         self._path_for_wd[moved_wd] = inotify_event.src_path
                         if self.is_recursive:
                             for _path, _wd in self._wd_for_path.copy().items():
-                                if _path.startswith(
-                                    move_src_path + os.path.sep.encode()
-                                ):
+                                if _path.startswith(move_src_path + os.path.sep.encode()):
                                     moved_wd = self._wd_for_path.pop(_path)
-                                    _move_to_path = _path.replace(
-                                        move_src_path, inotify_event.src_path
-                                    )
+                                    _move_to_path = _path.replace(move_src_path, inotify_event.src_path)
                                     self._wd_for_path[_move_to_path] = moved_wd
                                     self._path_for_wd[moved_wd] = _move_to_path
                     src_path = os.path.join(wd_path, name)
                     inotify_event = InotifyEvent(wd, mask, cookie, name, src_path)
 
                 if inotify_event.is_ignored:
                     # Clean up book-keeping for deleted watches.
                     path = self._path_for_wd.pop(wd)
                     if self._wd_for_path[path] == wd:
                         del self._wd_for_path[path]
 
                 event_list.append(inotify_event)
 
-                if (
-                    self.is_recursive
-                    and inotify_event.is_directory
-                    and inotify_event.is_create
-                ):
+                if self.is_recursive and inotify_event.is_directory and inotify_event.is_create:
                     # TODO: When a directory from another part of the
                     # filesystem is moved into a watched directory, this
                     # will not generate events for the directory tree.
                     # We need to coalesce IN_MOVED_TO events and those
                     # IN_MOVED_TO events which don't pair up with
                     # IN_MOVED_FROM events should be marked IN_CREATE
                     # instead relative to this directory.
@@ -557,19 +542,15 @@
         return self._mask & InotifyConstants.IN_IGNORED > 0
 
     @property
     def is_directory(self):
         # It looks like the kernel does not provide this information for
         # IN_DELETE_SELF and IN_MOVE_SELF. In this case, assume it's a dir.
         # See also: https://github.com/seb-m/pyinotify/blob/2c7e8f8/python2/pyinotify.py#L897
-        return (
-            self.is_delete_self
-            or self.is_move_self
-            or self._mask & InotifyConstants.IN_ISDIR > 0
-        )
+        return self.is_delete_self or self.is_move_self or self._mask & InotifyConstants.IN_ISDIR > 0
 
     @property
     def key(self):
         return self._src_path, self._wd, self._mask, self._cookie, self._name
 
     def __eq__(self, inotify_event):
         return self.key == inotify_event.key
```

### Comparing `watchdog-3.0.0/src/watchdog/observers/kqueue.py` & `watchdog-4.0.0/src/watchdog/observers/kqueue.py`

 * *Files 1% similar despite different names*

```diff
@@ -424,36 +424,36 @@
         A watch object representing the directory to monitor.
     :type watch:
         :class:`watchdog.observers.api.ObservedWatch`
     :param timeout:
         Read events blocking timeout (in seconds).
     :type timeout:
         ``float``
+    :param event_filter:
+        Collection of event types to emit, or None for no filtering (default).
+    :type event_filter:
+        Optional[Iterable[:class:`watchdog.events.FileSystemEvent`]]
     :param stat: stat function. See ``os.stat`` for details.
     """
 
-    def __init__(
-        self, event_queue, watch, timeout=DEFAULT_EMITTER_TIMEOUT, stat=os.stat
-    ):
-        super().__init__(event_queue, watch, timeout)
+    def __init__(self, event_queue, watch, timeout=DEFAULT_EMITTER_TIMEOUT, event_filter=None, stat=os.stat):
+        super().__init__(event_queue, watch, timeout, event_filter)
 
         self._kq = select.kqueue()
         self._lock = threading.RLock()
 
         # A collection of KeventDescriptor.
         self._descriptors = KeventDescriptorSet()
 
         def custom_stat(path, self=self):
             stat_info = stat(path)
             self._register_kevent(path, S_ISDIR(stat_info.st_mode))
             return stat_info
 
-        self._snapshot = DirectorySnapshot(
-            watch.path, recursive=watch.is_recursive, stat=custom_stat
-        )
+        self._snapshot = DirectorySnapshot(watch.path, recursive=watch.is_recursive, stat=custom_stat)
 
     def _register_kevent(self, path, is_directory):
         """
         Registers a kevent descriptor for the given path.
 
         :param path:
             Path for which a kevent descriptor will be created.
@@ -539,17 +539,15 @@
         descriptor = self._descriptors.get_for_fd(kev.ident)
         src_path = descriptor.path
 
         if is_renamed(kev):
             # Kqueue does not specify the destination names for renames
             # to, so we have to process these using the a snapshot
             # of the directory.
-            for event in self._gen_renamed_events(
-                src_path, descriptor.is_directory, ref_snapshot, new_snapshot
-            ):
+            for event in self._gen_renamed_events(src_path, descriptor.is_directory, ref_snapshot, new_snapshot):
                 yield event
         elif is_attrib_modified(kev):
             if descriptor.is_directory:
                 yield DirModifiedEvent(src_path)
             else:
                 yield FileModifiedEvent(src_path)
         elif is_modified(kev):
@@ -652,33 +650,29 @@
             try:
                 event_list = self._read_events(timeout)
                 # TODO: investigate why order appears to be reversed
                 event_list.reverse()
 
                 # Take a fresh snapshot of the directory and update the
                 # saved snapshot.
-                new_snapshot = DirectorySnapshot(
-                    self.watch.path, self.watch.is_recursive
-                )
+                new_snapshot = DirectorySnapshot(self.watch.path, self.watch.is_recursive)
                 ref_snapshot = self._snapshot
                 self._snapshot = new_snapshot
                 diff_events = new_snapshot - ref_snapshot
 
                 # Process events
                 for directory_created in diff_events.dirs_created:
                     self.queue_event(DirCreatedEvent(directory_created))
                 for file_created in diff_events.files_created:
                     self.queue_event(FileCreatedEvent(file_created))
                 for file_modified in diff_events.files_modified:
                     self.queue_event(FileModifiedEvent(file_modified))
 
                 for kev in event_list:
-                    for event in self._gen_kqueue_events(
-                        kev, ref_snapshot, new_snapshot
-                    ):
+                    for event in self._gen_kqueue_events(kev, ref_snapshot, new_snapshot):
                         self.queue_event(event)
 
             except OSError as e:
                 if e.errno != errno.EBADF:
                     raise
 
     def on_thread_stop(self):
```

### Comparing `watchdog-3.0.0/src/watchdog/observers/polling.py` & `watchdog-4.0.0/src/watchdog/observers/polling.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,33 +45,34 @@
     DirMovedEvent,
     FileCreatedEvent,
     FileDeletedEvent,
     FileModifiedEvent,
     FileMovedEvent,
 )
 from watchdog.observers.api import DEFAULT_EMITTER_TIMEOUT, DEFAULT_OBSERVER_TIMEOUT, BaseObserver, EventEmitter
-from watchdog.utils.dirsnapshot import DirectorySnapshot, DirectorySnapshotDiff
+from watchdog.utils.dirsnapshot import DirectorySnapshot, DirectorySnapshotDiff, EmptyDirectorySnapshot
 
 
 class PollingEmitter(EventEmitter):
     """
     Platform-independent emitter that polls a directory to detect file
     system changes.
     """
 
     def __init__(
         self,
         event_queue,
         watch,
         timeout=DEFAULT_EMITTER_TIMEOUT,
+        event_filter=None,
         stat=os.stat,
         listdir=os.scandir,
     ):
-        super().__init__(event_queue, watch, timeout)
-        self._snapshot = None
+        super().__init__(event_queue, watch, timeout, event_filter)
+        self._snapshot: DirectorySnapshot = EmptyDirectorySnapshot()
         self._lock = threading.Lock()
         self._take_snapshot = lambda: DirectorySnapshot(
             self.watch.path, self.watch.is_recursive, stat=stat, listdir=listdir
         )
 
     def on_thread_start(self):
         self._snapshot = self._take_snapshot()
```

### Comparing `watchdog-3.0.0/src/watchdog/observers/read_directory_changes.py` & `watchdog-4.0.0/src/watchdog/observers/read_directory_changes.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 from __future__ import annotations
 
 import os.path
 import platform
 import sys
 import threading
-import time
 
 from watchdog.events import (
     DirCreatedEvent,
     DirDeletedEvent,
     DirModifiedEvent,
     DirMovedEvent,
     FileCreatedEvent,
@@ -36,38 +35,40 @@
 )
 from watchdog.observers.api import DEFAULT_EMITTER_TIMEOUT, DEFAULT_OBSERVER_TIMEOUT, BaseObserver, EventEmitter
 
 assert sys.platform.startswith("win"), f"{__name__} requires Windows"
 
 from watchdog.observers.winapi import close_directory_handle, get_directory_handle, read_events  # noqa: E402
 
-# HACK:
+# Obsolete constant, it's no more used since v4.0.0.
 WATCHDOG_TRAVERSE_MOVED_DIR_DELAY = 1  # seconds
 
 
 class WindowsApiEmitter(EventEmitter):
     """
     Windows API-based emitter that uses ReadDirectoryChangesW
     to detect file system changes for a watch.
     """
 
-    def __init__(self, event_queue, watch, timeout=DEFAULT_EMITTER_TIMEOUT):
-        super().__init__(event_queue, watch, timeout)
+    def __init__(self, event_queue, watch, timeout=DEFAULT_EMITTER_TIMEOUT, event_filter=None):
+        super().__init__(event_queue, watch, timeout, event_filter)
         self._lock = threading.Lock()
         self._handle = None
 
     def on_thread_start(self):
         self._handle = get_directory_handle(self.watch.path)
 
     if platform.python_implementation() == "PyPy":
 
         def start(self):
             """PyPy needs some time before receiving events, see #792."""
+            from time import sleep
+
             super().start()
-            time.sleep(0.01)
+            sleep(0.01)
 
     def on_thread_stop(self):
         if self._handle:
             close_directory_handle(self._handle)
 
     def _read_events(self):
         return read_events(self._handle, self.watch.path, self.watch.is_recursive)
@@ -81,53 +82,29 @@
 
                 if winapi_event.is_renamed_old:
                     last_renamed_src_path = src_path
                 elif winapi_event.is_renamed_new:
                     dest_path = src_path
                     src_path = last_renamed_src_path
                     if os.path.isdir(dest_path):
-                        event = DirMovedEvent(src_path, dest_path)
+                        self.queue_event(DirMovedEvent(src_path, dest_path))
                         if self.watch.is_recursive:
-                            # HACK: We introduce a forced delay before
-                            # traversing the moved directory. This will read
-                            # only file movement that finishes within this
-                            # delay time.
-                            time.sleep(WATCHDOG_TRAVERSE_MOVED_DIR_DELAY)
-                            # The following block of code may not
-                            # obtain moved events for the entire tree if
-                            # the I/O is not completed within the above
-                            # delay time. So, it's not guaranteed to work.
-                            # TODO: Come up with a better solution, possibly
-                            # a way to wait for I/O to complete before
-                            # queuing events.
-                            for sub_moved_event in generate_sub_moved_events(
-                                src_path, dest_path
-                            ):
+                            for sub_moved_event in generate_sub_moved_events(src_path, dest_path):
                                 self.queue_event(sub_moved_event)
-                        self.queue_event(event)
                     else:
                         self.queue_event(FileMovedEvent(src_path, dest_path))
                 elif winapi_event.is_modified:
-                    cls = (
-                        DirModifiedEvent
-                        if os.path.isdir(src_path)
-                        else FileModifiedEvent
-                    )
+                    cls = DirModifiedEvent if os.path.isdir(src_path) else FileModifiedEvent
                     self.queue_event(cls(src_path))
                 elif winapi_event.is_added:
                     isdir = os.path.isdir(src_path)
                     cls = DirCreatedEvent if isdir else FileCreatedEvent
                     self.queue_event(cls(src_path))
                     if isdir and self.watch.is_recursive:
-                        # If a directory is moved from outside the watched folder to inside it
-                        # we only get a created directory event out of it, not any events for its children
-                        # so use the same hack as for file moves to get the child events
-                        time.sleep(WATCHDOG_TRAVERSE_MOVED_DIR_DELAY)
-                        sub_events = generate_sub_created_events(src_path)
-                        for sub_created_event in sub_events:
+                        for sub_created_event in generate_sub_created_events(src_path):
                             self.queue_event(sub_created_event)
                 elif winapi_event.is_removed:
                     self.queue_event(FileDeletedEvent(src_path))
                 elif winapi_event.is_removed_self:
                     self.queue_event(DirDeletedEvent(self.watch.path))
                     self.stop()
```

### Comparing `watchdog-3.0.0/src/watchdog/observers/winapi.py` & `watchdog-4.0.0/src/watchdog/observers/winapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 #
 # Portions of this code were taken from pyfilesystem, which uses the above
 # new BSD license.
 
 from __future__ import annotations
 
 import sys
+from dataclasses import dataclass
 from functools import reduce
 
 assert sys.platform.startswith("win"), f"{__name__} requires Windows"
 import ctypes.wintypes  # noqa: E402
 
 LPVOID = ctypes.wintypes.LPVOID
 
@@ -307,17 +308,15 @@
     GetFinalPathNameByHandleW(handle, buff, PATH_BUFFER_SIZE, VOLUME_NAME_NT)
     return buff.value != path
 
 
 def _generate_observed_path_deleted_event():
     # Create synthetic event for notify that observed directory is deleted
     path = ctypes.create_unicode_buffer(".")
-    event = FILE_NOTIFY_INFORMATION(
-        0, FILE_ACTION_DELETED_SELF, len(path), path.value.encode("utf-8")
-    )
+    event = FILE_NOTIFY_INFORMATION(0, FILE_ACTION_DELETED_SELF, len(path), path.value.encode("utf-8"))
     event_size = ctypes.sizeof(event)
     buff = ctypes.create_string_buffer(PATH_BUFFER_SIZE)
     ctypes.memmove(buff, ctypes.addressof(event), event_size)
     return buff, event_size
 
 
 def get_directory_handle(path):
@@ -371,18 +370,18 @@
             return _generate_observed_path_deleted_event()
 
         raise e
 
     return event_buffer.raw, int(nbytes.value)
 
 
+@dataclass(unsafe_hash=True)
 class WinAPINativeEvent:
-    def __init__(self, action, src_path):
-        self.action = action
-        self.src_path = src_path
+    action: int
+    src_path: str
 
     @property
     def is_added(self):
         return self.action == FILE_ACTION_CREATED
 
     @property
     def is_removed(self):
@@ -400,17 +399,12 @@
     def is_renamed_new(self):
         return self.action == FILE_ACTION_RENAMED_NEW_NAME
 
     @property
     def is_removed_self(self):
         return self.action == FILE_ACTION_REMOVED_SELF
 
-    def __repr__(self):
-        return (
-            f"<{type(self).__name__}: action={self.action}, src_path={self.src_path!r}>"
-        )
-
 
 def read_events(handle, path, recursive):
     buf, nbytes = read_directory_changes(handle, path, recursive)
     events = _parse_event_buffer(buf, nbytes)
     return [WinAPINativeEvent(action, src_path) for action, src_path in events]
```

### Comparing `watchdog-3.0.0/src/watchdog/tricks/__init__.py` & `watchdog-4.0.0/src/watchdog/tricks/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 import os
 import signal
 import subprocess
 import sys
 import threading
 import time
 
-from watchdog.events import EVENT_TYPE_OPENED, PatternMatchingEventHandler
+from watchdog.events import EVENT_TYPE_OPENED, FileSystemEvent, PatternMatchingEventHandler
 from watchdog.utils import echo
 from watchdog.utils.event_debouncer import EventDebouncer
 from watchdog.utils.process_watcher import ProcessWatcher
 
 logger = logging.getLogger(__name__)
 echo_events = functools.partial(echo.echo, write=lambda msg: logger.info(msg))
 
@@ -79,39 +79,16 @@
 """
 
 
 class LoggerTrick(Trick):
 
     """A simple trick that does only logs events."""
 
-    def on_any_event(self, event):
-        pass
-
-    @echo_events
-    def on_modified(self, event):
-        pass
-
-    @echo_events
-    def on_deleted(self, event):
-        pass
-
-    @echo_events
-    def on_created(self, event):
-        pass
-
-    @echo_events
-    def on_moved(self, event):
-        pass
-
     @echo_events
-    def on_closed(self, event):
-        pass
-
-    @echo_events
-    def on_opened(self, event):
+    def on_any_event(self, event: FileSystemEvent) -> None:
         pass
 
 
 class ShellCommandTrick(Trick):
 
     """Executes shell commands in response to matched events."""
 
@@ -174,17 +151,15 @@
             self._process_watchers.add(process_watcher)
             process_watcher.process_termination_callback = functools.partial(
                 self._process_watchers.discard, process_watcher
             )
             process_watcher.start()
 
     def is_process_running(self):
-        return self._process_watchers or (
-            self.process is not None and self.process.poll() is None
-        )
+        return self._process_watchers or (self.process is not None and self.process.poll() is None)
 
 
 class AutoRestartTrick(Trick):
 
     """Starts a long-running subprocess and restarts it on matched events.
 
     The command parameter is a list of command arguments, such as
@@ -259,17 +234,15 @@
             process_watcher.join()
 
     def _start_process(self):
         if self._is_trick_stopping:
             return
 
         # windows doesn't have setsid
-        self.process = subprocess.Popen(
-            self.command, preexec_fn=getattr(os, "setsid", None)
-        )
+        self.process = subprocess.Popen(self.command, preexec_fn=getattr(os, "setsid", None))
         if self.restart_on_command_exit:
             self.process_watcher = ProcessWatcher(self.process, self._restart_process)
             self.process_watcher.start()
 
     def _stop_process(self):
         # Ensure the body of the function is not run in parallel in different threads.
         with self._stopping_lock:
```

### Comparing `watchdog-3.0.0/src/watchdog/utils/__init__.py` & `watchdog-4.0.0/src/watchdog/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,29 +118,25 @@
     What won't work:
     - ClassName
     - modle.name.ClassName     # Typo in module name.
     - module.name.ClasNam      # Typo in classname.
     """
     dotted_path_split = dotted_path.split(".")
     if len(dotted_path_split) <= 1:
-        raise ValueError(
-            f"Dotted module path {dotted_path} must contain a module name and a classname"
-        )
+        raise ValueError(f"Dotted module path {dotted_path} must contain a module name and a classname")
     klass_name = dotted_path_split[-1]
     module_name = ".".join(dotted_path_split[:-1])
 
     module = load_module(module_name)
     if hasattr(module, klass_name):
         return getattr(module, klass_name)
         # Finally create and return an instance of the class
         # return klass(*args, **kwargs)
     else:
-        raise AttributeError(
-            f"Module {module_name} does not have class attribute {klass_name}"
-        )
+        raise AttributeError(f"Module {module_name} does not have class attribute {klass_name}")
 
 
 if TYPE_CHECKING or sys.version_info >= (3, 8):
     # using `as` to explicitly re-export this since this is a compatibility layer
     from typing import Protocol as Protocol
 else:
     # Provide a dummy Protocol class when not available from stdlib.  Should be used
```

### Comparing `watchdog-3.0.0/src/watchdog/utils/bricks.py` & `watchdog-4.0.0/src/watchdog/utils/bricks.py`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/src/watchdog/utils/delayed_queue.py` & `watchdog-4.0.0/src/watchdog/utils/delayed_queue.py`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/src/watchdog/utils/dirsnapshot.py` & `watchdog-4.0.0/src/watchdog/utils/dirsnapshot.py`

 * *Files 21% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 """
 
 from __future__ import annotations
 
 import errno
 import os
 from stat import S_ISDIR
+from typing import Any, Callable, Iterator, List, Optional, Tuple
 
 
 class DirectorySnapshotDiff:
     """
     Compares two directory snapshots and creates an object that represents
     the difference between the two snapshots.
 
@@ -75,36 +76,41 @@
         to think a file has been deleted and created again but it would be the
         exact same file.
         Set to True only if you are sure you will always use the same device.
     :type ignore_device:
         :class:`bool`
     """
 
-    def __init__(self, ref, snapshot, ignore_device=False):
+    def __init__(
+        self,
+        ref: DirectorySnapshot,
+        snapshot: DirectorySnapshot,
+        ignore_device: bool = False,
+    ):
         created = snapshot.paths - ref.paths
         deleted = ref.paths - snapshot.paths
 
         if ignore_device:
 
-            def get_inode(directory, full_path):
+            def get_inode(directory: DirectorySnapshot, full_path: str) -> int | Tuple[int, int]:
                 return directory.inode(full_path)[0]
 
         else:
 
-            def get_inode(directory, full_path):
+            def get_inode(directory: DirectorySnapshot, full_path: str) -> int | Tuple[int, int]:
                 return directory.inode(full_path)
 
         # check that all unchanged paths have the same inode
         for path in ref.paths & snapshot.paths:
             if get_inode(ref, path) != get_inode(snapshot, path):
                 created.add(path)
                 deleted.add(path)
 
         # find moved paths
-        moved = set()
+        moved: set[Tuple[str, str]] = set()
         for path in set(deleted):
             inode = ref.inode(path)
             new_path = snapshot.path(inode)
             if new_path:
                 # file is not deleted but moved
                 deleted.remove(path)
                 moved.add((path, new_path))
@@ -114,42 +120,38 @@
             old_path = ref.path(inode)
             if old_path:
                 created.remove(path)
                 moved.add((old_path, path))
 
         # find modified paths
         # first check paths that have not moved
-        modified = set()
+        modified: set[str] = set()
         for path in ref.paths & snapshot.paths:
             if get_inode(ref, path) == get_inode(snapshot, path):
-                if ref.mtime(path) != snapshot.mtime(path) or ref.size(
-                    path
-                ) != snapshot.size(path):
+                if ref.mtime(path) != snapshot.mtime(path) or ref.size(path) != snapshot.size(path):
                     modified.add(path)
 
         for old_path, new_path in moved:
-            if ref.mtime(old_path) != snapshot.mtime(new_path) or ref.size(
-                old_path
-            ) != snapshot.size(new_path):
+            if ref.mtime(old_path) != snapshot.mtime(new_path) or ref.size(old_path) != snapshot.size(new_path):
                 modified.add(old_path)
 
         self._dirs_created = [path for path in created if snapshot.isdir(path)]
         self._dirs_deleted = [path for path in deleted if ref.isdir(path)]
         self._dirs_modified = [path for path in modified if ref.isdir(path)]
         self._dirs_moved = [(frm, to) for (frm, to) in moved if ref.isdir(frm)]
 
         self._files_created = list(created - set(self._dirs_created))
         self._files_deleted = list(deleted - set(self._dirs_deleted))
         self._files_modified = list(modified - set(self._dirs_modified))
         self._files_moved = list(moved - set(self._dirs_moved))
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.__repr__()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         fmt = (
             "<{0} files(created={1}, deleted={2}, modified={3}, moved={4}),"
             " folders(created={5}, deleted={6}, modified={7}, moved={8})>"
         )
         return fmt.format(
             type(self).__name__,
             len(self._files_created),
@@ -159,69 +161,136 @@
             len(self._dirs_created),
             len(self._dirs_deleted),
             len(self._dirs_modified),
             len(self._dirs_moved),
         )
 
     @property
-    def files_created(self):
+    def files_created(self) -> List[str]:
         """List of files that were created."""
         return self._files_created
 
     @property
-    def files_deleted(self):
+    def files_deleted(self) -> List[str]:
         """List of files that were deleted."""
         return self._files_deleted
 
     @property
-    def files_modified(self):
+    def files_modified(self) -> List[str]:
         """List of files that were modified."""
         return self._files_modified
 
     @property
-    def files_moved(self):
+    def files_moved(self) -> list[Tuple[str, str]]:
         """
         List of files that were moved.
 
         Each event is a two-tuple the first item of which is the path
         that has been renamed to the second item in the tuple.
         """
         return self._files_moved
 
     @property
-    def dirs_modified(self):
+    def dirs_modified(self) -> List[str]:
         """
         List of directories that were modified.
         """
         return self._dirs_modified
 
     @property
-    def dirs_moved(self):
+    def dirs_moved(self) -> List[tuple[str, str]]:
         """
         List of directories that were moved.
 
         Each event is a two-tuple the first item of which is the path
         that has been renamed to the second item in the tuple.
         """
         return self._dirs_moved
 
     @property
-    def dirs_deleted(self):
+    def dirs_deleted(self) -> List[str]:
         """
         List of directories that were deleted.
         """
         return self._dirs_deleted
 
     @property
-    def dirs_created(self):
+    def dirs_created(self) -> List[str]:
         """
         List of directories that were created.
         """
         return self._dirs_created
 
+    class ContextManager:
+        """
+        Context manager that creates two directory snapshots and a
+        diff object that represents the difference between the two snapshots.
+
+        :param path:
+            The directory path for which a snapshot should be taken.
+        :type path:
+            ``str``
+        :param recursive:
+            ``True`` if the entire directory tree should be included in the
+            snapshot; ``False`` otherwise.
+        :type recursive:
+            ``bool``
+        :param stat:
+            Use custom stat function that returns a stat structure for path.
+            Currently only st_dev, st_ino, st_mode and st_mtime are needed.
+
+            A function taking a ``path`` as argument which will be called
+            for every entry in the directory tree.
+        :param listdir:
+            Use custom listdir function. For details see ``os.scandir``.
+        :param ignore_device:
+            A boolean indicating whether to ignore the device id or not.
+            By default, a file may be uniquely identified by a combination of its first
+            inode and its device id. The problem is that the device id may (or may not)
+            change between system boots. This problem would cause the DirectorySnapshotDiff
+            to think a file has been deleted and created again but it would be the
+            exact same file.
+            Set to True only if you are sure you will always use the same device.
+        :type ignore_device:
+            :class:`bool`
+        """
+
+        def __init__(
+            self,
+            path: str,
+            recursive: bool = True,
+            stat: Callable[[str], os.stat_result] = os.stat,
+            listdir: Callable[[Optional[str]], Iterator[os.DirEntry]] = os.scandir,
+            ignore_device: bool = False,
+        ):
+            self.path = path
+            self.recursive = recursive
+            self.stat = stat
+            self.listdir = listdir
+            self.ignore_device = ignore_device
+
+        def __enter__(self):
+            self.pre_snapshot = self.get_snapshot()
+
+        def __exit__(self, *args):
+            self.post_snapshot = self.get_snapshot()
+            self.diff = DirectorySnapshotDiff(
+                self.pre_snapshot,
+                self.post_snapshot,
+                ignore_device=self.ignore_device,
+            )
+
+        def get_snapshot(self):
+            return DirectorySnapshot(
+                path=self.path,
+                recursive=self.recursive,
+                stat=self.stat,
+                listdir=self.listdir,
+            )
+
 
 class DirectorySnapshot:
     """
     A snapshot of stat information of files in a directory.
 
     :param path:
         The directory path for which a snapshot should be taken.
@@ -238,32 +307,38 @@
 
         A function taking a ``path`` as argument which will be called
         for every entry in the directory tree.
     :param listdir:
         Use custom listdir function. For details see ``os.scandir``.
     """
 
-    def __init__(self, path, recursive=True, stat=os.stat, listdir=os.scandir):
+    def __init__(
+        self,
+        path: str,
+        recursive: bool = True,
+        stat: Callable[[str], os.stat_result] = os.stat,
+        listdir: Callable[[Optional[str]], Iterator[os.DirEntry]] = os.scandir,
+    ):
         self.recursive = recursive
         self.stat = stat
         self.listdir = listdir
 
-        self._stat_info = {}
-        self._inode_to_path = {}
+        self._stat_info: dict[str, os.stat_result] = {}
+        self._inode_to_path: dict[Tuple[int, int], str] = {}
 
         st = self.stat(path)
         self._stat_info[path] = st
         self._inode_to_path[(st.st_ino, st.st_dev)] = path
 
         for p, st in self.walk(path):
             i = (st.st_ino, st.st_dev)
             self._inode_to_path[i] = p
             self._stat_info[p] = st
 
-    def walk(self, root):
+    def walk(self, root: str) -> Iterator[Tuple[str, os.stat_result]]:
         try:
             paths = [os.path.join(root, entry.name) for entry in self.listdir(root)]
         except OSError as e:
             # Directory may have been deleted between finding it in the directory
             # list of its parent and trying to delete its contents. If this
             # happens we treat it as empty. Likewise if the directory was replaced
             # with a file of the same name (less likely, but possible).
@@ -287,89 +362,92 @@
                     if S_ISDIR(st.st_mode):
                         for entry in self.walk(path):
                             yield entry
                 except PermissionError:
                     pass
 
     @property
-    def paths(self):
+    def paths(self) -> set[str]:
         """
         Set of file/directory paths in the snapshot.
         """
         return set(self._stat_info.keys())
 
-    def path(self, id):
+    def path(self, id: Tuple[int, int]) -> Optional[str]:
         """
         Returns path for id. None if id is unknown to this snapshot.
         """
         return self._inode_to_path.get(id)
 
-    def inode(self, path):
+    def inode(self, path: str) -> Tuple[int, int]:
         """Returns an id for path."""
         st = self._stat_info[path]
         return (st.st_ino, st.st_dev)
 
-    def isdir(self, path):
+    def isdir(self, path: str) -> bool:
         return S_ISDIR(self._stat_info[path].st_mode)
 
-    def mtime(self, path):
+    def mtime(self, path: str) -> float:
         return self._stat_info[path].st_mtime
 
-    def size(self, path):
+    def size(self, path: str) -> int:
         return self._stat_info[path].st_size
 
-    def stat_info(self, path):
+    def stat_info(self, path: str) -> os.stat_result:
         """
         Returns a stat information object for the specified path from
         the snapshot.
 
         Attached information is subject to change. Do not use unless
         you specify `stat` in constructor. Use :func:`inode`, :func:`mtime`,
         :func:`isdir` instead.
 
         :param path:
             The path for which stat information should be obtained
             from a snapshot.
         """
         return self._stat_info[path]
 
-    def __sub__(self, previous_dirsnap):
+    def __sub__(self, previous_dirsnap: DirectorySnapshot) -> DirectorySnapshotDiff:
         """Allow subtracting a DirectorySnapshot object instance from
         another.
 
         :returns:
             A :class:`DirectorySnapshotDiff` object.
         """
         return DirectorySnapshotDiff(previous_dirsnap, self)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.__repr__()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return str(self._stat_info)
 
 
-class EmptyDirectorySnapshot:
+class EmptyDirectorySnapshot(DirectorySnapshot):
     """Class to implement an empty snapshot. This is used together with
     DirectorySnapshot and DirectorySnapshotDiff in order to get all the files/folders
     in the directory as created.
     """
 
+    def __init__(self):
+        pass
+
     @staticmethod
-    def path(_):
+    def path(_: Any) -> None:
         """Mock up method to return the path of the received inode. As the snapshot
         is intended to be empty, it always returns None.
 
         :returns:
             None.
         """
         return None
 
     @property
-    def paths(self):
+    def paths(self) -> set:
         """Mock up method to return a set of file/directory paths in the snapshot. As
         the snapshot is intended to be empty, it always returns an empty set.
 
         :returns:
             An empty set.
         """
         return set()
```

### Comparing `watchdog-3.0.0/src/watchdog/utils/echo.py` & `watchdog-4.0.0/src/watchdog/utils/echo.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,19 +45,15 @@
     """Determine if an instancemethod is a classmethod."""
     return inspect.ismethod(instancemethod) and instancemethod.__self__ is klass
 
 
 def is_static_method(method, klass):
     """Returns True if method is an instance method of klass."""
     return next(
-        (
-            isinstance(c.__dict__[name(method)], staticmethod)
-            for c in klass.mro()
-            if name(method) in c.__dict__
-        ),
+        (isinstance(c.__dict__[name(method)], staticmethod) for c in klass.mro() if name(method) in c.__dict__),
         False,
     )
 
 
 def is_class_private_name(name):
     """Determine if a name is a class private name."""
     # Exclude system defined names such as __init__, __add__ etc
@@ -103,17 +99,15 @@
     argdefs = dict(list(zip(argnames[-len(fn_defaults) :], fn_defaults)))
 
     @functools.wraps(fn)
     def wrapped(*v, **k):
         # Collect function arguments by chaining together positional,
         # defaulted, extra positional and keyword arguments.
         positional = list(map(format_arg_value, list(zip(argnames, v))))
-        defaulted = [
-            format_arg_value((a, argdefs[a])) for a in argnames[len(v) :] if a not in k
-        ]
+        defaulted = [format_arg_value((a, argdefs[a])) for a in argnames[len(v) :] if a not in k]
         nameless = list(map(repr, v[argcount:]))
         keyword = list(map(format_arg_value, list(k.items())))
         args = positional + defaulted + nameless + keyword
         write(f"{name(fn)}({', '.join(args)})\n")
         return fn(*v, **k)
 
     return wrapped
```

### Comparing `watchdog-3.0.0/src/watchdog/utils/event_debouncer.py` & `watchdog-4.0.0/src/watchdog/utils/event_debouncer.py`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/src/watchdog/utils/patterns.py` & `watchdog-4.0.0/src/watchdog/utils/patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,25 +23,19 @@
     else:
         included_patterns = {pattern.lower() for pattern in included_patterns}
         excluded_patterns = {pattern.lower() for pattern in excluded_patterns}
         path = PureWindowsPath(path)
 
     common_patterns = included_patterns & excluded_patterns
     if common_patterns:
-        raise ValueError(
-            "conflicting patterns `{}` included and excluded".format(common_patterns)
-        )
-    return any(path.match(p) for p in included_patterns) and not any(
-        path.match(p) for p in excluded_patterns
-    )
+        raise ValueError("conflicting patterns `{}` included and excluded".format(common_patterns))
+    return any(path.match(p) for p in included_patterns) and not any(path.match(p) for p in excluded_patterns)
 
 
-def filter_paths(
-    paths, included_patterns=None, excluded_patterns=None, case_sensitive=True
-):
+def filter_paths(paths, included_patterns=None, excluded_patterns=None, case_sensitive=True):
     """
     Filters from a set of paths based on acceptable patterns and
     ignorable patterns.
     :param pathnames:
         A list of path names that will be filtered based on matching and
         ignored patterns.
     :param included_patterns:
@@ -61,17 +55,15 @@
     excluded = [] if excluded_patterns is None else excluded_patterns
 
     for path in paths:
         if _match_path(path, set(included), set(excluded), case_sensitive):
             yield path
 
 
-def match_any_paths(
-    paths, included_patterns=None, excluded_patterns=None, case_sensitive=True
-):
+def match_any_paths(paths, included_patterns=None, excluded_patterns=None, case_sensitive=True):
     """
     Matches from a set of paths based on acceptable patterns and
     ignorable patterns.
     :param pathnames:
         A list of path names that will be filtered based on matching and
         ignored patterns.
     :param included_patterns:
```

### Comparing `watchdog-3.0.0/src/watchdog/utils/platform.py` & `watchdog-4.0.0/src/watchdog/utils/platform.py`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/src/watchdog/utils/process_watcher.py` & `watchdog-4.0.0/src/watchdog/utils/process_watcher.py`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/src/watchdog/version.py` & `watchdog-4.0.0/src/watchdog/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 # limitations under the License.
 
 
 from __future__ import annotations
 
 # When updating this version number, please update the
 # ``docs/source/global.rst.inc`` file as well.
-VERSION_MAJOR = 3
+VERSION_MAJOR = 4
 VERSION_MINOR = 0
 VERSION_BUILD = 0
 VERSION_INFO = (VERSION_MAJOR, VERSION_MINOR, VERSION_BUILD)
 VERSION_STRING = f"{VERSION_MAJOR}.{VERSION_MINOR}.{VERSION_BUILD}"
 
 __version__ = VERSION_INFO
```

### Comparing `watchdog-3.0.0/src/watchdog/watchmedo.py` & `watchdog-4.0.0/src/watchdog/watchmedo.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,25 +93,19 @@
       >>> args.func(args)
 
     """
 
     def decorator(func):
         name = func.__name__.replace("_", "-")
         desc = dedent(func.__doc__)
-        parser = parent.add_parser(
-            name, description=desc, aliases=cmd_aliases, formatter_class=HelpFormatter
-        )
+        parser = parent.add_parser(name, description=desc, aliases=cmd_aliases, formatter_class=HelpFormatter)
         command_parsers[name] = parser
         verbosity_group = parser.add_mutually_exclusive_group()
-        verbosity_group.add_argument(
-            "-q", "--quiet", dest="verbosity", action="append_const", const=-1
-        )
-        verbosity_group.add_argument(
-            "-v", "--verbose", dest="verbosity", action="append_const", const=1
-        )
+        verbosity_group.add_argument("-q", "--quiet", dest="verbosity", action="append_const", const=-1)
+        verbosity_group.add_argument("-v", "--verbose", dest="verbosity", action="append_const", const=1)
         for arg in args:
             parser.add_argument(*arg[0], **arg[1])
             parser.set_defaults(func=func)
         return func
 
     return decorator
 
@@ -233,17 +227,15 @@
         ),
         argument(
             "--recursive",
             action="store_true",
             default=True,
             help="Recursively monitor paths (defaults to True).",
         ),
-        argument(
-            "--debug-force-polling", action="store_true", help="[debug] Forces polling."
-        ),
+        argument("--debug-force-polling", action="store_true", help="[debug] Forces polling."),
         argument(
             "--debug-force-kqueue",
             action="store_true",
             help="[debug] Forces BSD kqueue(2).",
         ),
         argument(
             "--debug-force-winapi",
@@ -292,17 +284,15 @@
             raise OSError(errno.ENOENT, os.strerror(errno.ENOENT), tricks_file)
 
         config = load_config(tricks_file)
 
         try:
             tricks = config[CONFIG_KEY_TRICKS]
         except KeyError:
-            raise KeyError(
-                f"No {CONFIG_KEY_TRICKS!r} key specified in {tricks_file!r}."
-            )
+            raise KeyError(f"No {CONFIG_KEY_TRICKS!r} key specified in {tricks_file!r}.")
 
         if CONFIG_KEY_PYTHON_PATH in config:
             add_to_sys_path(config[CONFIG_KEY_PYTHON_PATH])
 
         dir_path = os.path.dirname(tricks_file)
         if not dir_path:
             dir_path = os.path.relpath(os.getcwd())
@@ -425,20 +415,16 @@
             "--interval",
             "--timeout",
             dest="timeout",
             default=1.0,
             type=float,
             help="Use this as the polling interval/blocking timeout.",
         ),
-        argument(
-            "--trace", action="store_true", help="Dumps complete dispatching trace."
-        ),
-        argument(
-            "--debug-force-polling", action="store_true", help="[debug] Forces polling."
-        ),
+        argument("--trace", action="store_true", help="Dumps complete dispatching trace."),
+        argument("--debug-force-polling", action="store_true", help="[debug] Forces polling."),
         argument(
             "--debug-force-kqueue",
             action="store_true",
             help="[debug] Forces BSD kqueue(2).",
         ),
         argument(
             "--debug-force-winapi",
@@ -572,17 +558,15 @@
             "-W",
             "--drop",
             dest="drop_during_process",
             action="store_true",
             help="Ignore events that occur while command is still being"
             " executed to avoid multiple simultaneous instances.",
         ),
-        argument(
-            "--debug-force-polling", action="store_true", help="[debug] Forces polling."
-        ),
+        argument("--debug-force-polling", action="store_true", help="[debug] Forces polling."),
     ]
 )
 def shell_command(args):
     """
     Command to execute shell commands in response to file system events.
     """
     from watchdog.tricks import ShellCommandTrick
@@ -625,16 +609,15 @@
         ),
         argument(
             "-d",
             "--directory",
             dest="directories",
             metavar="DIRECTORY",
             action="append",
-            help="Directory to watch. Use another -d or --directory option "
-            "for each directory.",
+            help="Directory to watch. Use another -d or --directory option " "for each directory.",
         ),
         argument(
             "-p",
             "--pattern",
             "--patterns",
             dest="patterns",
             default="*",
@@ -673,24 +656,21 @@
         ),
         argument(
             "--signal",
             dest="signal",
             default="SIGINT",
             help="Stop the subprocess with this signal (default SIGINT).",
         ),
-        argument(
-            "--debug-force-polling", action="store_true", help="[debug] Forces polling."
-        ),
+        argument("--debug-force-polling", action="store_true", help="[debug] Forces polling."),
         argument(
             "--kill-after",
             dest="kill_after",
             default=10.0,
             type=float,
-            help="When stopping, kill the subprocess after the specified timeout "
-            "in seconds (default 10.0).",
+            help="When stopping, kill the subprocess after the specified timeout " "in seconds (default 10.0).",
         ),
         argument(
             "--debounce-interval",
             dest="debounce_interval",
             default=0.0,
             type=float,
             help="After a file change, Wait until the specified interval (in "
```

### Comparing `watchdog-3.0.0/src/watchdog.egg-info/PKG-INFO` & `watchdog-4.0.0/src/watchdog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchdog
-Version: 3.0.0
+Version: 4.0.0
 Summary: Filesystem events monitoring
 Home-page: https://github.com/gorakhargosh/watchdog
 Author: Yesudeep Mangalapilly
 Author-email: yesudeep@gmail.com
-License: Apache License 2.0
+License: Apache-2.0
 Project-URL: Documentation, https://python-watchdog.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/gorakhargosh/watchdog/
 Project-URL: Issues, https://github.com/gorakhargosh/watchdog/issues
 Project-URL: Changelog, https://github.com/gorakhargosh/watchdog/blob/master/changelog.rst
 Keywords: python filesystem monitoring monitor FSEvents kqueue inotify ReadDirectoryChangesW polling DirectorySnapshot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -26,41 +26,41 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: C
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: watchmedo
 License-File: LICENSE
 License-File: COPYING
 License-File: AUTHORS
 
 Watchdog
 ========
 
 |Build Status|
 |CirrusCI Status|
 
 Python API and shell utilities to monitor file system events.
 
-Works on 3.7+.
+Works on 3.8+.
 
 Example API Usage
 -----------------
 
 A simple program that uses watchdog to monitor directories specified
 as command-line arguments and logs events generated:
 
@@ -73,14 +73,15 @@
     from watchdog.events import LoggingEventHandler
 
     if __name__ == "__main__":
         logging.basicConfig(level=logging.INFO,
                             format='%(asctime)s - %(message)s',
                             datefmt='%Y-%m-%d %H:%M:%S')
         path = sys.argv[1] if len(sys.argv) > 1 else '.'
+        logging.info(f'start watching directory {path!r}')
         event_handler = LoggingEventHandler()
         observer = Observer()
         observer.schedule(event_handler, path, recursive=True)
         observer.start()
         try:
             while True:
                 time.sleep(1)
@@ -258,15 +259,15 @@
 
     from watchdog.observers.polling import PollingObserver as Observer
 
 
 Dependencies
 ------------
 
-1. Python 3.7 or above.
+1. Python 3.8 or above.
 2. XCode_ (only on macOS when installing from sources)
 3. PyYAML_ (only for ``watchmedo``)
 
 Licensing
 ---------
 
 Watchdog is licensed under the terms of the `Apache License, version 2.0`_.
@@ -327,14 +328,31 @@
 
 
 .. :changelog:
 
 Changelog
 ---------
 
+4.0.0
+~~~~~
+
+2024-02-06 • `full history <https://github.com/gorakhargosh/watchdog/compare/v3.0.0...v4.0.0>`__
+
+- Drop support for Python 3.7.
+- Add support for Python 3.12.
+- [snapshot] Add typing to ``dirsnapshot`` (`#1012 <https://github.com/gorakhargosh/watchdog/pull/1012>`__)
+- [snapshot] Added ``DirectorySnapshotDiff.ContextManager`` (`#1011 <https://github.com/gorakhargosh/watchdog/pull/1011>`__)
+- [events] ``FileSystemEvent``, and subclasses, are now ``dataclass``es, and their ``repr()`` has changed
+- [windows] ``WinAPINativeEvent`` is now a ``dataclass``, and its ``repr()`` has changed
+- [events] Log ``FileOpenedEvent``, and ``FileClosedEvent``, events in ``LoggingEventHandler``
+- [tests] Improve ``FileSystemEvent`` coverage
+- [watchmedo] Log all events in ``LoggerTrick``
+- [windows] The ``observers.read_directory_changes.WATCHDOG_TRAVERSE_MOVED_DIR_DELAY`` hack was removed. The constant will be kept to prevent breaking other softwares.
+- Thanks to our beloved contributors: @BoboTiG, @msabramo
+
 3.0.0
 ~~~~~
 
 2023-03-20 • `full history <https://github.com/gorakhargosh/watchdog/compare/v2.3.1...v3.0.0>`__
 
 - Drop support for Python 3.6.
 - ``watchdog`` is now PEP 561 compatible, and tested with ``mypy``
```

### Comparing `watchdog-3.0.0/src/watchdog.egg-info/SOURCES.txt` & `watchdog-4.0.0/src/watchdog.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 AUTHORS
 COPYING
 LICENSE
 MANIFEST.in
 README.rst
 changelog.rst
+pyproject.toml
 requirements-tests.txt
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/eclipse_cdt_style.xml
 docs/make.bat
```

### Comparing `watchdog-3.0.0/src/watchdog_fsevents.c` & `watchdog-4.0.0/src/watchdog_fsevents.c`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/tests/__init__.py` & `watchdog-4.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/tests/conftest.py` & `watchdog-4.0.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,15 @@
     """
     Fail on thread leak.
     We do not use pytest-threadleak because it is not reliable.
     """
     old_thread_count = threading.active_count()
     yield
     gc.collect()  # Clear the stuff from other function-level fixtures
-    assert (
-        threading.active_count() == old_thread_count
-    )  # Only previously existing threads
+    assert threading.active_count() == old_thread_count  # Only previously existing threads
 
 
 @pytest.fixture(autouse=True)
 def no_warnings(recwarn):
     """Fail on warning."""
 
     yield
```

### Comparing `watchdog-3.0.0/tests/shell.py` & `watchdog-4.0.0/tests/shell.py`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/tests/test_0_watchmedo.py` & `watchdog-4.0.0/tests/test_0_watchmedo.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,18 +54,15 @@
 
     assert not os.path.exists(critical_dir)
 
 
 def make_dummy_script(tmpdir, n=10):
     script = os.path.join(tmpdir, f"auto-test-{n}.py")
     with open(script, "w") as f:
-        f.write(
-            'import time\nfor i in range(%d):\n\tprint("+++++ %%d" %% i, flush=True)\n\ttime.sleep(1)\n'
-            % n
-        )
+        f.write('import time\nfor i in range(%d):\n\tprint("+++++ %%d" %% i, flush=True)\n\ttime.sleep(1)\n' % n)
     return script
 
 
 def test_kill_auto_restart(tmpdir, capfd):
     script = make_dummy_script(tmpdir)
     a = AutoRestartTrick([sys.executable, script])
     a.start()
@@ -192,33 +189,29 @@
 )
 def test_auto_restart_subprocess_termination(tmpdir, capfd, restart_on_command_exit):
     """Run auto-restart with a script that terminates in about 2 seconds.
 
     After 5 seconds, expect it to have been restarted at least once.
     """
     script = make_dummy_script(tmpdir, n=2)
-    trick = AutoRestartTrick(
-        [sys.executable, script], restart_on_command_exit=restart_on_command_exit
-    )
+    trick = AutoRestartTrick([sys.executable, script], restart_on_command_exit=restart_on_command_exit)
     trick.start()
     time.sleep(5)
     trick.stop()
     cap = capfd.readouterr()
     if restart_on_command_exit:
         assert cap.out.splitlines(keepends=False).count("+++++ 0") > 1
         assert trick.restart_count >= 1
     else:
         assert cap.out.splitlines(keepends=False).count("+++++ 0") == 1
         assert trick.restart_count == 0
 
 
 def test_auto_restart_arg_parsing_basic():
-    args = watchmedo.cli.parse_args(
-        ["auto-restart", "-d", ".", "--recursive", "--debug-force-polling", "cmd"]
-    )
+    args = watchmedo.cli.parse_args(["auto-restart", "-d", ".", "--recursive", "--debug-force-polling", "cmd"])
     assert args.func is watchmedo.auto_restart
     assert args.command == "cmd"
     assert args.directories == ["."]
     assert args.recursive
     assert args.debug_force_polling
```

### Comparing `watchdog-3.0.0/tests/test_delayed_queue.py` & `watchdog-4.0.0/tests/test_delayed_queue.py`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/tests/test_emitter.py` & `watchdog-4.0.0/tests/test_emitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,18 +47,15 @@
     # enable more verbose logs
     fsevents_logger = logging.getLogger("fsevents")
     fsevents_logger.setLevel(logging.DEBUG)
 
 
 def rerun_filter(exc, *args):
     time.sleep(5)
-    if issubclass(exc[0], Empty) and platform.is_windows():
-        return True
-
-    return False
+    return bool(issubclass(exc[0], Empty) and platform.is_windows())
 
 
 @pytest.mark.flaky(max_runs=5, min_passes=1, rerun_filter=rerun_filter)
 def test_create(p: P, event_queue: TestEventQueue, start_watching: StartWatching, expect_event: ExpectEvent) -> None:
     start_watching()
     open(p("a"), "a").close()
 
@@ -73,17 +70,15 @@
         assert isinstance(event, FileOpenedEvent)
         event = event_queue.get(timeout=5)[0]
         assert event.src_path == p("a")
         assert isinstance(event, FileClosedEvent)
 
 
 @pytest.mark.xfail(reason="known to be problematic")
-@pytest.mark.skipif(
-    not platform.is_linux(), reason="FileCloseEvent only supported in GNU/Linux"
-)
+@pytest.mark.skipif(not platform.is_linux(), reason="FileCloseEvent only supported in GNU/Linux")
 @pytest.mark.flaky(max_runs=5, min_passes=1, rerun_filter=rerun_filter)
 def test_close(p: P, event_queue: TestEventQueue, start_watching: StartWatching) -> None:
     f_d = open(p("a"), "a")
     start_watching()
     f_d.close()
 
     # After file creation/open in append mode
@@ -242,28 +237,26 @@
 
     expect_event(FileCreatedEvent(p("dir2", "b")))
 
     if not platform.is_windows():
         expect_event(DirModifiedEvent(p("dir2")))
 
 
-@pytest.mark.skipif(
-    not platform.is_linux(), reason="InotifyFullEmitter only supported in Linux"
-)
+@pytest.mark.skipif(not platform.is_linux(), reason="InotifyFullEmitter only supported in Linux")
 def test_move_to_full(p: P, event_queue: TestEventQueue, start_watching: StartWatching) -> None:
     mkdir(p("dir1"))
     mkdir(p("dir2"))
     mkfile(p("dir1", "a"))
     start_watching(p("dir2"), use_full_emitter=True)
     mv(p("dir1", "a"), p("dir2", "b"))
 
     event = event_queue.get(timeout=5)[0]
     assert isinstance(event, FileMovedEvent)
     assert event.dest_path == p("dir2", "b")
-    assert event.src_path is None  # Should equal None since the path was not watched
+    assert event.src_path == ""  # Should be blank since the path was not watched
 
 
 @pytest.mark.flaky(max_runs=5, min_passes=1, rerun_filter=rerun_filter)
 def test_move_from(p: P, start_watching: StartWatching, expect_event: ExpectEvent) -> None:
     mkdir(p("dir1"))
     mkdir(p("dir2"))
     mkfile(p("dir1", "a"))
@@ -273,28 +266,26 @@
 
     expect_event(FileDeletedEvent(p("dir1", "a")))
 
     if not platform.is_windows():
         expect_event(DirModifiedEvent(p("dir1")))
 
 
-@pytest.mark.skipif(
-    not platform.is_linux(), reason="InotifyFullEmitter only supported in Linux"
-)
+@pytest.mark.skipif(not platform.is_linux(), reason="InotifyFullEmitter only supported in Linux")
 def test_move_from_full(p: P, event_queue: TestEventQueue, start_watching: StartWatching) -> None:
     mkdir(p("dir1"))
     mkdir(p("dir2"))
     mkfile(p("dir1", "a"))
     start_watching(p("dir1"), use_full_emitter=True)
     mv(p("dir1", "a"), p("dir2", "b"))
 
     event = event_queue.get(timeout=5)[0]
     assert isinstance(event, FileMovedEvent)
     assert event.src_path == p("dir1", "a")
-    assert event.dest_path is None  # Should equal None since path not watched
+    assert event.dest_path == ""  # Should be blank since path not watched
 
 
 @pytest.mark.flaky(max_runs=5, min_passes=1, rerun_filter=rerun_filter)
 def test_separate_consecutive_moves(p: P, start_watching: StartWatching, expect_event: ExpectEvent) -> None:
     mkdir(p("dir1"))
     mkfile(p("dir1", "a"))
     mkfile(p("b"))
@@ -317,17 +308,15 @@
         expected_events = [d_created, a_deleted, dir_modif, dir_modif]
 
     for expected_event in expected_events:
         expect_event(expected_event)
 
 
 @pytest.mark.flaky(max_runs=5, min_passes=1, rerun_filter=rerun_filter)
-@pytest.mark.skipif(
-    platform.is_bsd(), reason="BSD create another set of events for this test"
-)
+@pytest.mark.skipif(platform.is_bsd(), reason="BSD create another set of events for this test")
 def test_delete_self(p: P, start_watching: StartWatching, expect_event: ExpectEvent) -> None:
     mkdir(p("dir1"))
     emitter = start_watching(p("dir1"))
     rm(p("dir1"), True)
     expect_event(DirDeletedEvent(p("dir1")))
     emitter.join(5)
     assert not emitter.is_alive()
@@ -356,17 +345,15 @@
     for _ in range(times * 4):
         event = event_queue.get(timeout=5)[0]
         logger.debug(event)
         etype = type(event)
         count[etype] += 1
         assert event.src_path == etype_for_dir[etype]
         assert count[DirCreatedEvent] >= count[DirDeletedEvent]
-        assert (
-            count[DirCreatedEvent] + count[DirDeletedEvent] >= count[DirModifiedEvent]
-        )
+        assert count[DirCreatedEvent] + count[DirDeletedEvent] >= count[DirModifiedEvent]
     assert count == {
         DirCreatedEvent: times,
         DirModifiedEvent: times * 2,
         DirDeletedEvent: times,
     }
 
 
@@ -444,159 +431,78 @@
         with pytest.raises(Empty):
             event_queue.get(timeout=5)
         mkfile(p("dir1", "dir2", "somefile"))
         with pytest.raises(Empty):
             event_queue.get(timeout=5)
 
         mkdir(p("dir3"))
-        expect_event(
-            DirModifiedEvent(p())
-        )  # the contents of the parent directory changed
+        expect_event(DirModifiedEvent(p()))  # the contents of the parent directory changed
 
         mv(p("dir1", "dir2", "somefile"), p("somefile"))
         expect_event(FileMovedEvent(p("dir1", "dir2", "somefile"), p("somefile")))
         expect_event(DirModifiedEvent(p()))
 
         mv(p("dir1", "dir2"), p("dir2"))
         expect_event(DirMovedEvent(p("dir1", "dir2"), p("dir2")))
         expect_event(DirModifiedEvent(p()))
 
 
-@pytest.mark.skipif(
-    platform.is_windows(), reason="Windows create another set of events for this test"
-)
+@pytest.mark.flaky(max_runs=5, min_passes=1, rerun_filter=rerun_filter)
 def test_renaming_top_level_directory(
     p: P,
     event_queue: TestEventQueue,
     start_watching: StartWatching,
     expect_event: ExpectEvent,
 ) -> None:
     start_watching()
 
     mkdir(p("a"))
     expect_event(DirCreatedEvent(p("a")))
-    expect_event(DirModifiedEvent(p()))
+    if not platform.is_windows():
+        expect_event(DirModifiedEvent(p()))
 
     mkdir(p("a", "b"))
     expect_event(DirCreatedEvent(p("a", "b")))
     expect_event(DirModifiedEvent(p("a")))
 
     mv(p("a"), p("a2"))
     expect_event(DirMovedEvent(p("a"), p("a2")))
-    expect_event(DirModifiedEvent(p()))
-    expect_event(DirModifiedEvent(p()))
-
-    expect_event(DirMovedEvent(p("a", "b"), p("a2", "b")))
+    if not platform.is_windows():
+        expect_event(DirModifiedEvent(p()))
+        expect_event(DirModifiedEvent(p()))
+    expect_event(DirMovedEvent(p("a", "b"), p("a2", "b"), is_synthetic=True))
 
     if platform.is_bsd():
         expect_event(DirModifiedEvent(p()))
 
     open(p("a2", "b", "c"), "a").close()
 
     # DirModifiedEvent may emitted, but sometimes after waiting time is out.
     events = []
     while True:
         events.append(event_queue.get(timeout=5)[0])
         if event_queue.empty():
             break
 
     assert all(
-        [
-            isinstance(
-                e,
-                (
-                    FileCreatedEvent,
-                    FileMovedEvent,
-                    FileOpenedEvent,
-                    DirModifiedEvent,
-                    FileClosedEvent,
-                ),
-            )
-            for e in events
-        ]
-    )
-
-    for event in events:
-        if isinstance(event, FileCreatedEvent):
-            assert event.src_path == p("a2", "b", "c")
-        elif isinstance(event, FileMovedEvent):
-            assert event.dest_path == p("a2", "b", "c")
-            assert event.src_path == p("a", "b", "c")
-        elif isinstance(event, DirModifiedEvent):
-            assert event.src_path == p("a2", "b")
-
-
-@pytest.mark.flaky(max_runs=5, min_passes=1, rerun_filter=rerun_filter)
-@pytest.mark.skipif(
-    not platform.is_windows(),
-    reason="Non-Windows create another set of events for this test",
-)
-def test_renaming_top_level_directory_on_windows(
-    p: P,
-    event_queue: TestEventQueue,
-    start_watching: StartWatching,
-) -> None:
-    start_watching()
-
-    mkdir(p("a"))
-    event = event_queue.get(timeout=5)[0]
-    assert isinstance(event, DirCreatedEvent)
-    assert event.src_path == p("a")
-
-    mkdir(p("a", "b"))
-    event = event_queue.get(timeout=5)[0]
-    assert isinstance(event, DirCreatedEvent)
-    assert event.src_path == p("a", "b")
-
-    event = event_queue.get(timeout=5)[0]
-    assert isinstance(event, DirCreatedEvent)
-    assert event.src_path == p("a", "b")
-
-    event = event_queue.get(timeout=5)[0]
-    assert isinstance(event, DirModifiedEvent)
-    assert event.src_path == p("a")
-
-    mv(p("a"), p("a2"))
-    event = event_queue.get(timeout=5)[0]
-    assert isinstance(event, DirMovedEvent)
-    assert event.src_path == p("a", "b")
-
-    open(p("a2", "b", "c"), "a").close()
-
-    events = []
-    while True:
-        events.append(event_queue.get(timeout=5)[0])
-        if event_queue.empty():
-            break
-
-    assert all(
-        [
-            isinstance(
-                e, (FileCreatedEvent, FileMovedEvent, DirMovedEvent, DirModifiedEvent)
-            )
-            for e in events
-        ]
+        isinstance(e, (FileCreatedEvent, FileMovedEvent, FileOpenedEvent, DirModifiedEvent, FileClosedEvent))
+        for e in events
     )
 
     for event in events:
         if isinstance(event, FileCreatedEvent):
             assert event.src_path == p("a2", "b", "c")
         elif isinstance(event, FileMovedEvent):
             assert event.dest_path == p("a2", "b", "c")
             assert event.src_path == p("a", "b", "c")
-        elif isinstance(event, DirMovedEvent):
-            assert event.dest_path == p("a2")
-            assert event.src_path == p("a")
         elif isinstance(event, DirModifiedEvent):
             assert event.src_path == p("a2", "b")
 
 
-@pytest.mark.skipif(
-    platform.is_windows(), reason="Windows create another set of events for this test"
-)
+@pytest.mark.skipif(platform.is_windows(), reason="Windows create another set of events for this test")
 def test_move_nested_subdirectories(
     p: P,
     event_queue: TestEventQueue,
     start_watching: StartWatching,
     expect_event: ExpectEvent,
 ) -> None:
     mkdir(p("dir1/dir2/dir3"), parents=True)
@@ -604,16 +510,16 @@
     start_watching()
     mv(p("dir1/dir2"), p("dir2"))
 
     expect_event(DirMovedEvent(p("dir1", "dir2"), p("dir2")))
     expect_event(DirModifiedEvent(p("dir1")))
     expect_event(DirModifiedEvent(p()))
 
-    expect_event(DirMovedEvent(p("dir1", "dir2", "dir3"), p("dir2", "dir3")))
-    expect_event(FileMovedEvent(p("dir1", "dir2", "dir3", "a"), p("dir2", "dir3", "a")))
+    expect_event(DirMovedEvent(p("dir1", "dir2", "dir3"), p("dir2", "dir3"), is_synthetic=True))
+    expect_event(FileMovedEvent(p("dir1", "dir2", "dir3", "a"), p("dir2", "dir3", "a"), is_synthetic=True))
 
     if platform.is_bsd():
         event = event_queue.get(timeout=5)[0]
         assert p(event.src_path) == p()
         assert isinstance(event, DirModifiedEvent)
 
         event = event_queue.get(timeout=5)[0]
@@ -677,17 +583,15 @@
         if isinstance(event, FileModifiedEvent):
             assert event.src_path == p("dir2", "dir3", "a")
         elif isinstance(event, DirModifiedEvent):
             assert event.src_path in [p("dir2"), p("dir2", "dir3")]
 
 
 @pytest.mark.flaky(max_runs=5, min_passes=1, rerun_filter=rerun_filter)
-@pytest.mark.skipif(
-    platform.is_bsd(), reason="BSD create another set of events for this test"
-)
+@pytest.mark.skipif(platform.is_bsd(), reason="BSD create another set of events for this test")
 def test_file_lifecyle(p: P, start_watching: StartWatching, expect_event: ExpectEvent) -> None:
     start_watching()
 
     mkfile(p("a"))
     touch(p("a"))
     mv(p("a"), p("b"))
     rm(p("b"))
```

### Comparing `watchdog-3.0.0/tests/test_events.py` & `watchdog-4.0.0/tests/test_events.py`

 * *Files 13% similar despite different names*

```diff
@@ -174,7 +174,28 @@
             assert event.event_type == EVENT_TYPE_OPENED
 
     handler = TestableEventHandler()
 
     for event in all_events:
         assert not event.is_synthetic
         handler.dispatch(event)
+
+
+def test_event_comparison():
+    creation1 = FileCreatedEvent("foo")
+    creation2 = FileCreatedEvent("foo")
+    creation3 = FileCreatedEvent("bar")
+    assert creation1 == creation2
+    assert creation1 != creation3
+    assert creation2 != creation3
+
+    move1 = FileMovedEvent("a", "b")
+    move2 = FileMovedEvent("a", "b")
+    move3 = FileMovedEvent("a", "c")
+    move4 = FileMovedEvent("b", "a")
+    assert creation1 != move1  # type: ignore[comparison-overlap]
+    assert move1 == move2
+    assert move1 != move3
+    assert move1 != move4
+    assert move2 != move3
+    assert move2 != move4
+    assert move3 != move4
```

### Comparing `watchdog-3.0.0/tests/test_fsevents.py` & `watchdog-4.0.0/tests/test_fsevents.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import time
 from os import mkdir, rmdir
 from random import random
 from threading import Thread
 from time import sleep
 from unittest.mock import patch
 
-import _watchdog_fsevents as _fsevents  # type: ignore[import]
+import _watchdog_fsevents as _fsevents  # type: ignore[import-not-found]
 
 from watchdog.events import FileSystemEventHandler
 from watchdog.observers import Observer
 from watchdog.observers.api import BaseObserver, ObservedWatch
 from watchdog.observers.fsevents import FSEventsEmitter
 
 from .shell import touch
@@ -51,24 +51,20 @@
         (_fsevents.NativeEvent("", 0, 0x00000800, 0), False),
         # renamed, removed
         (_fsevents.NativeEvent("", 0, 0x00000800 | 0x00000200, 0), True),
         # renamed, removed, created
         (_fsevents.NativeEvent("", 0, 0x00000800 | 0x00000200 | 0x00000100, 0), True),
         # renamed, removed, created, itemfindermod
         (
-            _fsevents.NativeEvent(
-                "", 0, 0x00000800 | 0x00000200 | 0x00000100 | 0x00002000, 0
-            ),
+            _fsevents.NativeEvent("", 0, 0x00000800 | 0x00000200 | 0x00000100 | 0x00002000, 0),
             True,
         ),
         # xattr, removed, modified, itemfindermod
         (
-            _fsevents.NativeEvent(
-                "", 0, 0x00008000 | 0x00000200 | 0x00001000 | 0x00002000, 0
-            ),
+            _fsevents.NativeEvent("", 0, 0x00008000 | 0x00000200 | 0x00001000 | 0x00002000, 0),
             False,
         ),
     ],
 )
 def test_coalesced_event_check(event, expectation):
     assert event.is_coalesced == expectation
 
@@ -115,17 +111,15 @@
 
     orig = FSEventsEmitter.events_callback
 
     def cb(*args):
         FSEventsEmitter.stop(emitter)
         orig(*args)
 
-    with caplog.at_level(logging.ERROR), patch.object(
-        FSEventsEmitter, "events_callback", new=cb
-    ):
+    with caplog.at_level(logging.ERROR), patch.object(FSEventsEmitter, "events_callback", new=cb):
         emitter = start_watching(tmpdir)
         # Less than 100 is not enough events to trigger the error
         for n in range(100):
             touch(p("{}.txt".format(n)))
         emitter.stop()
         assert not caplog.records
 
@@ -272,17 +266,15 @@
             self.observed_events.add(event)
 
         def done(self):
             return not self.expected_events
 
     cwd = os.getcwd()
     os.chdir(p())
-    event_handler = TestEventHandler(
-        patterns=["*.json"], ignore_patterns=[], ignore_directories=True
-    )
+    event_handler = TestEventHandler(patterns=["*.json"], ignore_patterns=[], ignore_directories=True)
     observer = Observer()
     observer.schedule(event_handler, ".")
     observer.start()
     time.sleep(0.1)
 
     try:
         touch(p("foo.json"))
@@ -325,15 +317,13 @@
         touch(p("dir_rec", "my1.txt"))
 
         expected = {"dir_rec", "my0.txt", "my1.txt"}
         timeout_at = time.time() + 5
         while not expected.issubset(handler.changes) and time.time() < timeout_at:
             time.sleep(0.2)
 
-        assert expected.issubset(
-            handler.changes
-        ), f"Did not find expected changes. Found: {handler.changes}"
+        assert expected.issubset(handler.changes), f"Did not find expected changes. Found: {handler.changes}"
     finally:
         for watch in watches:
             observer.unschedule(watch)
         observer.stop()
         observer.join(1)
```

### Comparing `watchdog-3.0.0/tests/test_inotify_buffer.py` & `watchdog-4.0.0/tests/test_inotify_buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
     inotify.read_event()
 
     # Ensure InotifyBuffer shuts down cleanly without raising an exception
     inotify.close()
 
 
 @pytest.mark.timeout(5)
+@pytest.mark.skipif("GITHUB_REF" not in os.environ, reason="sudo password prompt")
 def test_unmount_watched_directory_filesystem(p):
     mkdir(p("dir1"))
     mount_tmpfs(p("dir1"))
     mkdir(p("dir1/dir2"))
     inotify = InotifyBuffer(p("dir1/dir2").encode())
     unmount(p("dir1"))
 
@@ -151,16 +152,14 @@
         self._inotify.read_events = delay_call(  # type: ignore[method-assign]
             function=self._inotify.read_events, seconds=1
         )
 
         return super().run(*args, **kwargs)
 
 
-@pytest.mark.parametrize(
-    argnames="cls", argvalues=[InotifyBuffer, InotifyBufferDelayedRead]
-)
+@pytest.mark.parametrize(argnames="cls", argvalues=[InotifyBuffer, InotifyBufferDelayedRead])
 def test_close_should_terminate_thread(p, cls):
     inotify = cls(p("").encode(), recursive=True)
 
     assert inotify.is_alive()
     inotify.close()
     assert not inotify.is_alive()
```

### Comparing `watchdog-3.0.0/tests/test_inotify_c.py` & `watchdog-4.0.0/tests/test_inotify_c.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,20 +41,16 @@
     inotify_fd.last = 0
     inotify_fd.wds = []
 
     const = InotifyConstants()
 
     # CREATE DELETE CREATE DELETE DELETE_SELF IGNORE DELETE_SELF IGNORE
     inotify_fd.buf = (
-        struct_inotify(
-            wd=1, mask=const.IN_CREATE | const.IN_ISDIR, length=16, name=b"subdir1"
-        )
-        + struct_inotify(
-            wd=1, mask=const.IN_DELETE | const.IN_ISDIR, length=16, name=b"subdir1"
-        )
+        struct_inotify(wd=1, mask=const.IN_CREATE | const.IN_ISDIR, length=16, name=b"subdir1")
+        + struct_inotify(wd=1, mask=const.IN_DELETE | const.IN_ISDIR, length=16, name=b"subdir1")
     ) * 2 + (
         struct_inotify(wd=2, mask=const.IN_DELETE_SELF)
         + struct_inotify(wd=2, mask=const.IN_IGNORED)
         + struct_inotify(wd=3, mask=const.IN_DELETE_SELF)
         + struct_inotify(wd=3, mask=const.IN_IGNORED)
     )
 
@@ -155,19 +151,13 @@
     assert repr(event)
 
 
 def test_event_equality(p: P) -> None:
     wd_parent_dir = 42
     filename = "file.ext"
     full_path = p(filename)
-    event1 = InotifyEvent(
-        wd_parent_dir, InotifyConstants.IN_CREATE, 0, filename, full_path
-    )
-    event2 = InotifyEvent(
-        wd_parent_dir, InotifyConstants.IN_CREATE, 0, filename, full_path
-    )
-    event3 = InotifyEvent(
-        wd_parent_dir, InotifyConstants.IN_ACCESS, 0, filename, full_path
-    )
+    event1 = InotifyEvent(wd_parent_dir, InotifyConstants.IN_CREATE, 0, filename, full_path)
+    event2 = InotifyEvent(wd_parent_dir, InotifyConstants.IN_CREATE, 0, filename, full_path)
+    event3 = InotifyEvent(wd_parent_dir, InotifyConstants.IN_ACCESS, 0, filename, full_path)
     assert event1 == event2
     assert event1 != event3
     assert event2 != event3
```

### Comparing `watchdog-3.0.0/tests/test_logging_event_handler.py` & `watchdog-4.0.0/tests/test_logging_event_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,36 +12,41 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from watchdog.events import (
+    EVENT_TYPE_CLOSED,
     EVENT_TYPE_CREATED,
     EVENT_TYPE_DELETED,
     EVENT_TYPE_MODIFIED,
     EVENT_TYPE_MOVED,
+    EVENT_TYPE_OPENED,
     DirCreatedEvent,
     DirDeletedEvent,
     DirModifiedEvent,
     DirMovedEvent,
+    FileClosedEvent,
     FileCreatedEvent,
     FileDeletedEvent,
     FileModifiedEvent,
     FileMovedEvent,
+    FileOpenedEvent,
+    FileSystemEvent,
     LoggingEventHandler,
 )
 
 path_1 = "/path/xyz"
 path_2 = "/path/abc"
 
 
 class _TestableEventHandler(LoggingEventHandler):
     def on_any_event(self, event):
-        assert True
+        assert isinstance(event, FileSystemEvent)
 
     def on_modified(self, event):
         super().on_modified(event)
         assert event.event_type == EVENT_TYPE_MODIFIED
 
     def on_deleted(self, event):
         super().on_deleted(event)
@@ -51,33 +56,45 @@
         super().on_moved(event)
         assert event.event_type == EVENT_TYPE_MOVED
 
     def on_created(self, event):
         super().on_created(event)
         assert event.event_type == EVENT_TYPE_CREATED
 
+    def on_closed(self, event):
+        super().on_closed(event)
+        assert event.event_type == EVENT_TYPE_CLOSED
+
+    def on_opened(self, event):
+        super().on_opened(event)
+        assert event.event_type == EVENT_TYPE_OPENED
+
 
 def test_logging_event_handler_dispatch():
     # Utilities.
     dir_del_event = DirDeletedEvent("/path/blah.py")
     file_del_event = FileDeletedEvent("/path/blah.txt")
     dir_cre_event = DirCreatedEvent("/path/blah.py")
     file_cre_event = FileCreatedEvent("/path/blah.txt")
     dir_mod_event = DirModifiedEvent("/path/blah.py")
     file_mod_event = FileModifiedEvent("/path/blah.txt")
     dir_mov_event = DirMovedEvent("/path/blah.py", "/path/blah")
     file_mov_event = FileMovedEvent("/path/blah.txt", "/path/blah")
+    file_ope_event = FileOpenedEvent("/path/blah.txt")
+    file_clo_event = FileClosedEvent("/path/blah.txt")
 
     all_events = [
         dir_mod_event,
         dir_del_event,
         dir_cre_event,
         dir_mov_event,
         file_mod_event,
         file_del_event,
         file_cre_event,
         file_mov_event,
+        file_ope_event,
+        file_clo_event,
     ]
 
     handler = _TestableEventHandler()
     for event in all_events:
         handler.dispatch(event)
```

### Comparing `watchdog-3.0.0/tests/test_observer.py` & `watchdog-4.0.0/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/tests/test_observers_api.py` & `watchdog-4.0.0/tests/test_observers_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 
 import time
 from pathlib import Path
 
 import pytest
 
-from watchdog.events import FileModifiedEvent, LoggingEventHandler
+from watchdog.events import FileModifiedEvent, FileOpenedEvent, LoggingEventHandler
 from watchdog.observers.api import BaseObserver, EventDispatcher, EventEmitter, EventQueue, ObservedWatch
 
 
 def test_observer_constructor():
     ObservedWatch(Path("/foobar"), True)
 
 
@@ -53,14 +53,19 @@
 
 def test_observer__repr__():
     observed_watch = ObservedWatch("/foobar", True)
     repr_str = "<ObservedWatch: path='/foobar', is_recursive=True>"
     assert observed_watch.__repr__() == repr(observed_watch)
     assert repr(observed_watch) == repr_str
 
+    observed_watch = ObservedWatch("/foobar", False, [FileOpenedEvent, FileModifiedEvent])
+    repr_str = "<ObservedWatch: path='/foobar', is_recursive=False, event_filter=FileModifiedEvent|FileOpenedEvent>"
+    assert observed_watch.__repr__() == repr(observed_watch)
+    assert repr(observed_watch) == repr_str
+
 
 def test_event_emitter():
     event_queue = EventQueue()
     watch = ObservedWatch("/foobar", True)
     event_emitter = EventEmitter(event_queue, watch, timeout=1)
     event_emitter.queue_event(FileModifiedEvent("/foobar/blah"))
```

### Comparing `watchdog-3.0.0/tests/test_observers_polling.py` & `watchdog-4.0.0/tests/test_observers_polling.py`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/tests/test_observers_winapi.py` & `watchdog-4.0.0/tests/test_observers_winapi.py`

 * *Files identical despite different names*

### Comparing `watchdog-3.0.0/tests/test_pattern_matching_event_handler.py` & `watchdog-4.0.0/tests/test_pattern_matching_event_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,20 +138,16 @@
             assert_patterns(event)
 
         def on_created(self, event):
             assert_check_directory(self, event)
             assert event.event_type == EVENT_TYPE_CREATED
             assert_patterns(event)
 
-    no_dirs_handler = TestableEventHandler(
-        patterns=patterns, ignore_patterns=ignore_patterns, ignore_directories=True
-    )
-    handler = TestableEventHandler(
-        patterns=patterns, ignore_patterns=ignore_patterns, ignore_directories=False
-    )
+    no_dirs_handler = TestableEventHandler(patterns=patterns, ignore_patterns=ignore_patterns, ignore_directories=True)
+    handler = TestableEventHandler(patterns=patterns, ignore_patterns=ignore_patterns, ignore_directories=False)
 
     for event in all_events:
         no_dirs_handler.dispatch(event)
     for event in all_events:
         handler.dispatch(event)
```

### Comparing `watchdog-3.0.0/tests/test_patterns.py` & `watchdog-4.0.0/tests/test_patterns.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,20 @@
     [
         ("/users/gorakhargosh/foobar.py", {"*.py"}, {"*.PY"}, True, True),
         ("/users/gorakhargosh/foobar.py", {"*.py"}, {"*.PY"}, True, True),
         ("/users/gorakhargosh/", {"*.py"}, {"*.txt"}, False, False),
         ("/users/gorakhargosh/foobar.py", {"*.py"}, {"*.PY"}, False, ValueError),
     ],
 )
-def test_match_path(
-    input, included_patterns, excluded_patterns, case_sensitive, expected
-):
+def test_match_path(input, included_patterns, excluded_patterns, case_sensitive, expected):
     if expected == ValueError:
         with pytest.raises(expected):
             _match_path(input, included_patterns, excluded_patterns, case_sensitive)
     else:
-        assert (
-            _match_path(input, included_patterns, excluded_patterns, case_sensitive)
-            is expected
-        )
+        assert _match_path(input, included_patterns, excluded_patterns, case_sensitive) is expected
 
 
 @pytest.mark.parametrize(
     "included_patterns, excluded_patterns, case_sensitive, expected",
     [
         (None, None, True, None),
         (None, None, False, None),
@@ -46,36 +41,29 @@
 def test_filter_paths(included_patterns, excluded_patterns, case_sensitive, expected):
     pathnames = {
         "/users/gorakhargosh/foobar.py",
         "/var/cache/pdnsd.status",
         "/etc/pdnsd.conf",
         "/usr/local/bin/python",
     }
-    actual = set(
-        filter_paths(pathnames, included_patterns, excluded_patterns, case_sensitive)
-    )
+    actual = set(filter_paths(pathnames, included_patterns, excluded_patterns, case_sensitive))
     assert actual == expected if expected else pathnames
 
 
 @pytest.mark.parametrize(
     "included_patterns, excluded_patterns, case_sensitive, expected",
     [
         (None, None, True, True),
         (None, None, False, True),
         (["*py", "*.conf"], ["*.status"], True, True),
         (["*.txt"], None, False, False),
         (["*.txt"], None, True, False),
     ],
 )
-def test_match_any_paths(
-    included_patterns, excluded_patterns, case_sensitive, expected
-):
+def test_match_any_paths(included_patterns, excluded_patterns, case_sensitive, expected):
     pathnames = {
         "/users/gorakhargosh/foobar.py",
         "/var/cache/pdnsd.status",
         "/etc/pdnsd.conf",
         "/usr/local/bin/python",
     }
-    assert (
-        match_any_paths(pathnames, included_patterns, excluded_patterns, case_sensitive)
-        == expected
-    )
+    assert match_any_paths(pathnames, included_patterns, excluded_patterns, case_sensitive) == expected
```

### Comparing `watchdog-3.0.0/tests/test_regex_matching_event_handler.py` & `watchdog-4.0.0/tests/test_regex_matching_event_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,20 +136,16 @@
             assert_regexes(self, event)
 
         def on_created(self, event):
             assert_check_directory(self, event)
             assert event.event_type == EVENT_TYPE_CREATED
             assert_regexes(self, event)
 
-    no_dirs_handler = TestableEventHandler(
-        regexes=regexes, ignore_regexes=ignore_regexes, ignore_directories=True
-    )
-    handler = TestableEventHandler(
-        regexes=regexes, ignore_regexes=ignore_regexes, ignore_directories=False
-    )
+    no_dirs_handler = TestableEventHandler(regexes=regexes, ignore_regexes=ignore_regexes, ignore_directories=True)
+    handler = TestableEventHandler(regexes=regexes, ignore_regexes=ignore_regexes, ignore_directories=False)
 
     for event in all_events:
         no_dirs_handler.dispatch(event)
     for event in all_events:
         handler.dispatch(event)
```

### Comparing `watchdog-3.0.0/tests/test_skip_repeats_queue.py` & `watchdog-4.0.0/tests/test_skip_repeats_queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,13 +102,13 @@
     assert e1 == q.get()
     assert q.empty()
 
 
 @cpython_only
 def test_eventlet_monkey_patching():
     try:
-        import eventlet  # type: ignore[import]
+        import eventlet  # type: ignore[import-untyped]
     except Exception:
         pytest.skip("eventlet not installed")
 
     eventlet.monkey_patch()
     basic_actions()
```

### Comparing `watchdog-3.0.0/tests/test_snapshot_diff.py` & `watchdog-4.0.0/tests/test_snapshot_diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,28 @@
     touch(p("dir1", "a"))
     ref = DirectorySnapshot(p("dir2"))
     mv(p("dir1", "a"), p("dir2", "b"))
     diff = DirectorySnapshotDiff(ref, DirectorySnapshot(p("dir2")))
     assert diff.files_created == [p("dir2", "b")]
 
 
+def test_move_to_with_context_manager(p):
+    mkdir(p("dir1"))
+    touch(p("dir1", "a"))
+    mkdir(p("dir2"))
+
+    dir1_cm = DirectorySnapshotDiff.ContextManager(p("dir1"))
+    dir2_cm = DirectorySnapshotDiff.ContextManager(p("dir2"))
+    with dir1_cm, dir2_cm:
+        mv(p("dir1", "a"), p("dir2", "b"))
+
+    assert dir1_cm.diff.files_deleted == [p("dir1", "a")]
+    assert dir2_cm.diff.files_created == [p("dir2", "b")]
+
+
 def test_move_from(p):
     mkdir(p("dir1"))
     mkdir(p("dir2"))
     touch(p("dir1", "a"))
     ref = DirectorySnapshot(p("dir1"))
     mv(p("dir1", "a"), p("dir2", "b"))
     diff = DirectorySnapshotDiff(ref, DirectorySnapshot(p("dir1")))
```

### Comparing `watchdog-3.0.0/tests/utils.py` & `watchdog-4.0.0/tests/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,26 +62,25 @@
         recursive: bool = True,
     ) -> EventEmitter:
         # todo: check if other platforms expect the trailing slash (e.g. `p('')`)
         path = self.tmp if path is None else path
 
         emitter: EventEmitter
         if sys.platform.startswith("linux") and use_full_emitter:
-            emitter = InotifyFullEmitter(
-                self.event_queue, ObservedWatch(path, recursive=recursive)
-            )
+            emitter = InotifyFullEmitter(self.event_queue, ObservedWatch(path, recursive=recursive))
         else:
             emitter = Emitter(self.event_queue, ObservedWatch(path, recursive=recursive))
 
         self.emitters.append(emitter)
 
         if sys.platform.startswith("darwin"):
             # TODO: I think this could be better...  .suppress_history should maybe
             #       become a common attribute.
             from watchdog.observers.fsevents import FSEventsEmitter
+
             assert isinstance(emitter, FSEventsEmitter)
             emitter.suppress_history = True
 
         emitter.start()
 
         return emitter
```

### Comparing `watchdog-3.0.0/tox.ini` & `watchdog-4.0.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 envlist =
-    py{311,310,39,38,37,36,py3}
+    py{312,311,310,39,38,py3}
     docs
     mypy
 skip_missing_interpreters = True
 
 [testenv]
 usedevelop = true
 deps =
```

