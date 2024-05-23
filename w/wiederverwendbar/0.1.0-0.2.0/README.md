# Comparing `tmp/wiederverwendbar-0.1.0.tar.gz` & `tmp/wiederverwendbar-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiederverwendbar-0.1.0.tar", last modified: Thu May 23 08:54:19 2024, max compression
+gzip compressed data, was "wiederverwendbar-0.2.0.tar", last modified: Thu May 23 11:31:34 2024, max compression
```

## Comparing `wiederverwendbar-0.1.0.tar` & `wiederverwendbar-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,17 @@
--rw-r--r--   0        0        0       20 2024-05-23 08:41:07.437583 wiederverwendbar-0.1.0/README.md
--rw-r--r--   0        0        0      438 2024-05-23 08:54:19.402540 wiederverwendbar-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-23 08:41:07.439228 wiederverwendbar-0.1.0/src/wiederverwendbar/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 08:41:07.441100 wiederverwendbar-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      311 1970-01-01 00:00:00.000000 wiederverwendbar-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/README.md
+-rw-r--r--   0        0        0      682 2024-05-23 11:31:34.532018 wiederverwendbar-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      155 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/functions/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/functions/find_class_method.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/handlers/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/handlers/rich_console_handler.py
+-rw-r--r--   0        0        0      624 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/handlers/stream_console_handler.py
+-rw-r--r--   0        0        0     2378 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py
+-rw-r--r--   0        0        0     3036 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/logger.py
+-rw-r--r--   0        0        0     5665 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/logger_settings.py
+-rw-r--r--   0        0        0      161 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/logger_singleton.py
+-rw-r--r--   0        0        0     3643 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/singleton.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      417 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/tests/logger.py
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 wiederverwendbar-0.2.0/PKG-INFO
```

