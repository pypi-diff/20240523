# Comparing `tmp/cvat_sdk_i_digit-0.0.2.tar.gz` & `tmp/cvat_sdk_i_digit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat_sdk_i_digit-0.0.2.tar", last modified: Wed May 22 12:35:26 2024, max compression
+gzip compressed data, was "cvat_sdk_i_digit-0.0.3.tar", last modified: Wed May 22 12:43:28 2024, max compression
```

## Comparing `cvat_sdk_i_digit-0.0.2.tar` & `cvat_sdk_i_digit-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 dima      (1000) dima      (1000)        0 2024-05-22 12:35:26.626574 cvat_sdk_i_digit-0.0.2/
--rw-r--r--   0 dima      (1000) dima      (1000)      311 2024-05-22 12:35:26.626574 cvat_sdk_i_digit-0.0.2/PKG-INFO
--rw-rw-r--   0 dima      (1000) dima      (1000)        0 2024-05-22 11:23:00.000000 cvat_sdk_i_digit-0.0.2/README.md
-drwxrwxr-x   0 dima      (1000) dima      (1000)        0 2024-05-22 12:35:26.626574 cvat_sdk_i_digit-0.0.2/cvat_sdk_i_digit.egg-info/
--rw-r--r--   0 dima      (1000) dima      (1000)      311 2024-05-22 12:35:26.000000 cvat_sdk_i_digit-0.0.2/cvat_sdk_i_digit.egg-info/PKG-INFO
--rw-rw-r--   0 dima      (1000) dima      (1000)      223 2024-05-22 12:35:26.000000 cvat_sdk_i_digit-0.0.2/cvat_sdk_i_digit.egg-info/SOURCES.txt
--rw-rw-r--   0 dima      (1000) dima      (1000)        1 2024-05-22 12:35:26.000000 cvat_sdk_i_digit-0.0.2/cvat_sdk_i_digit.egg-info/dependency_links.txt
--rw-rw-r--   0 dima      (1000) dima      (1000)       71 2024-05-22 12:35:26.000000 cvat_sdk_i_digit-0.0.2/cvat_sdk_i_digit.egg-info/requires.txt
--rw-rw-r--   0 dima      (1000) dima      (1000)        1 2024-05-22 12:35:26.000000 cvat_sdk_i_digit-0.0.2/cvat_sdk_i_digit.egg-info/top_level.txt
--rw-rw-r--   0 dima      (1000) dima      (1000)      704 2024-05-22 12:35:22.000000 cvat_sdk_i_digit-0.0.2/pyproject.toml
--rw-rw-r--   0 dima      (1000) dima      (1000)       38 2024-05-22 12:35:26.626574 cvat_sdk_i_digit-0.0.2/setup.cfg
+drwxrwxr-x   0 dima      (1000) dima      (1000)        0 2024-05-22 12:43:28.343921 cvat_sdk_i_digit-0.0.3/
+-rw-r--r--   0 dima      (1000) dima      (1000)      311 2024-05-22 12:43:28.343921 cvat_sdk_i_digit-0.0.3/PKG-INFO
+-rw-rw-r--   0 dima      (1000) dima      (1000)        0 2024-05-22 11:23:00.000000 cvat_sdk_i_digit-0.0.3/README.md
+drwxrwxr-x   0 dima      (1000) dima      (1000)        0 2024-05-22 12:43:28.343921 cvat_sdk_i_digit-0.0.3/cvat_sdk_i_digit.egg-info/
+-rw-r--r--   0 dima      (1000) dima      (1000)      311 2024-05-22 12:43:28.000000 cvat_sdk_i_digit-0.0.3/cvat_sdk_i_digit.egg-info/PKG-INFO
+-rw-rw-r--   0 dima      (1000) dima      (1000)      223 2024-05-22 12:43:28.000000 cvat_sdk_i_digit-0.0.3/cvat_sdk_i_digit.egg-info/SOURCES.txt
+-rw-rw-r--   0 dima      (1000) dima      (1000)        1 2024-05-22 12:43:28.000000 cvat_sdk_i_digit-0.0.3/cvat_sdk_i_digit.egg-info/dependency_links.txt
+-rw-rw-r--   0 dima      (1000) dima      (1000)       71 2024-05-22 12:43:28.000000 cvat_sdk_i_digit-0.0.3/cvat_sdk_i_digit.egg-info/requires.txt
+-rw-rw-r--   0 dima      (1000) dima      (1000)        1 2024-05-22 12:43:28.000000 cvat_sdk_i_digit-0.0.3/cvat_sdk_i_digit.egg-info/top_level.txt
+-rw-rw-r--   0 dima      (1000) dima      (1000)      704 2024-05-22 12:42:57.000000 cvat_sdk_i_digit-0.0.3/pyproject.toml
+-rw-rw-r--   0 dima      (1000) dima      (1000)       38 2024-05-22 12:43:28.343921 cvat_sdk_i_digit-0.0.3/setup.cfg
```

### Comparing `cvat_sdk_i_digit-0.0.2/pyproject.toml` & `cvat_sdk_i_digit-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cvat_sdk_i_digit"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = [
     {name = "Шумелев Дмитрий Игоревич", email = "cmit.dima@gmail.com"}
 ]
 dependencies = [
     "cvat-sdk>=2.13.0",
     "pydantic-settings>=2.0.2",
```

