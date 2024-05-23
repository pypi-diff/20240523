# Comparing `tmp/wiederverwendbar-0.2.0.tar.gz` & `tmp/wiederverwendbar-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiederverwendbar-0.2.0.tar", last modified: Thu May 23 11:31:34 2024, max compression
+gzip compressed data, was "wiederverwendbar-0.2.1.tar", last modified: Thu May 23 12:44:35 2024, max compression
```

## Comparing `wiederverwendbar-0.2.0.tar` & `wiederverwendbar-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0       19 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/README.md
--rw-r--r--   0        0        0      682 2024-05-23 11:31:34.532018 wiederverwendbar-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      155 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/functions/__init__.py
--rw-r--r--   0        0        0      407 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/functions/find_class_method.py
--rw-r--r--   0        0        0        0 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/handlers/__init__.py
--rw-r--r--   0        0        0      600 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/handlers/rich_console_handler.py
--rw-r--r--   0        0        0      624 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/handlers/stream_console_handler.py
--rw-r--r--   0        0        0     2378 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py
--rw-r--r--   0        0        0     3036 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/logger.py
--rw-r--r--   0        0        0     5665 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/logger_settings.py
--rw-r--r--   0        0        0      161 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/logger/logger_singleton.py
--rw-r--r--   0        0        0     3643 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/src/wiederverwendbar/singleton.py
--rw-r--r--   0        0        0        0 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      417 2024-05-23 11:30:49.193620 wiederverwendbar-0.2.0/tests/logger.py
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 wiederverwendbar-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-23 12:43:13.002601 wiederverwendbar-0.2.1/README.md
+-rw-r--r--   0        0        0      682 2024-05-23 12:44:35.518765 wiederverwendbar-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      155 2024-05-23 12:43:13.002601 wiederverwendbar-0.2.1/src/wiederverwendbar/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 12:43:13.002601 wiederverwendbar-0.2.1/src/wiederverwendbar/functions/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-23 12:43:13.002601 wiederverwendbar-0.2.1/src/wiederverwendbar/functions/find_class_method.py
+-rw-r--r--   0        0        0      186 2024-05-23 12:43:13.002601 wiederverwendbar-0.2.1/src/wiederverwendbar/logger/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 12:43:13.002601 wiederverwendbar-0.2.1/src/wiederverwendbar/logger/handlers/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-23 12:43:13.002601 wiederverwendbar-0.2.1/src/wiederverwendbar/logger/handlers/rich_console_handler.py
+-rw-r--r--   0        0        0      624 2024-05-23 12:43:13.006600 wiederverwendbar-0.2.1/src/wiederverwendbar/logger/handlers/stream_console_handler.py
+-rw-r--r--   0        0        0     2378 2024-05-23 12:43:13.006600 wiederverwendbar-0.2.1/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py
+-rw-r--r--   0        0        0     3036 2024-05-23 12:43:13.006600 wiederverwendbar-0.2.1/src/wiederverwendbar/logger/logger.py
+-rw-r--r--   0        0        0     5665 2024-05-23 12:43:13.006600 wiederverwendbar-0.2.1/src/wiederverwendbar/logger/logger_settings.py
+-rw-r--r--   0        0        0      161 2024-05-23 12:43:13.006600 wiederverwendbar-0.2.1/src/wiederverwendbar/logger/logger_singleton.py
+-rw-r--r--   0        0        0        0 2024-05-23 12:43:13.006600 wiederverwendbar-0.2.1/src/wiederverwendbar/models/__init__.py
+-rw-r--r--   0        0        0     2145 2024-05-23 12:43:13.006600 wiederverwendbar-0.2.1/src/wiederverwendbar/models/file_config.py
+-rw-r--r--   0        0        0      762 2024-05-23 12:43:13.006600 wiederverwendbar-0.2.1/src/wiederverwendbar/models/indexable_model.py
+-rw-r--r--   0        0        0     3643 2024-05-23 12:43:13.006600 wiederverwendbar-0.2.1/src/wiederverwendbar/singleton.py
+-rw-r--r--   0        0        0        0 2024-05-23 12:43:13.006600 wiederverwendbar-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      384 2024-05-23 12:43:13.006600 wiederverwendbar-0.2.1/tests/logger.py
+-rw-r--r--   0        0        0      462 2024-05-23 12:43:13.006600 wiederverwendbar-0.2.1/tests/test.py
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 wiederverwendbar-0.2.1/PKG-INFO
```

### Comparing `wiederverwendbar-0.2.0/pyproject.toml` & `wiederverwendbar-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 dependencies = [
     "pydantic>=2.7.1",
     "pydantic-settings>=2.2.1",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.optional-dependencies]
 rich = [
     "rich>=13.7.1",
```

### Comparing `wiederverwendbar-0.2.0/src/wiederverwendbar/logger/handlers/rich_console_handler.py` & `wiederverwendbar-0.2.1/src/wiederverwendbar/logger/handlers/rich_console_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.0/src/wiederverwendbar/logger/handlers/stream_console_handler.py` & `wiederverwendbar-0.2.1/src/wiederverwendbar/logger/handlers/stream_console_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.0/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py` & `wiederverwendbar-0.2.1/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.0/src/wiederverwendbar/logger/logger.py` & `wiederverwendbar-0.2.1/src/wiederverwendbar/logger/logger.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.0/src/wiederverwendbar/logger/logger_settings.py` & `wiederverwendbar-0.2.1/src/wiederverwendbar/logger/logger_settings.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.0/src/wiederverwendbar/singleton.py` & `wiederverwendbar-0.2.1/src/wiederverwendbar/singleton.py`

 * *Files identical despite different names*

