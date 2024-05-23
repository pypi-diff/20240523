# Comparing `tmp/panoptica_genai_protection-0.1.6.tar.gz` & `tmp/panoptica_genai_protection-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panoptica_genai_protection-0.1.6.tar", last modified: Sun May  5 12:42:01 2024, max compression
+gzip compressed data, was "panoptica_genai_protection-0.1.7.tar", last modified: Mon May  6 08:05:35 2024, max compression
```

## Comparing `panoptica_genai_protection-0.1.6.tar` & `panoptica_genai_protection-0.1.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:42:01.842210 panoptica_genai_protection-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-05 12:42:01.842210 panoptica_genai_protection-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-05 12:41:51.000000 panoptica_genai_protection-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 12:42:01.842210 panoptica_genai_protection-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:05:35.845744 panoptica_genai_protection-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-06 08:05:35.845744 panoptica_genai_protection-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-06 08:05:23.000000 panoptica_genai_protection-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:05:35.845744 panoptica_genai_protection-0.1.7/setup.cfg
```

### Comparing `panoptica_genai_protection-0.1.6/PKG-INFO` & `panoptica_genai_protection-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptica_genai_protection
-Version: 0.1.6
+Version: 0.1.7
 Summary: Protecting GenAI from Prompt Injection
 Author: marvin-team@cisco.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `panoptica_genai_protection-0.1.6/README.md` & `panoptica_genai_protection-0.1.7/README.md`

 * *Files identical despite different names*

