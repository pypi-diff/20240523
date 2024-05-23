# Comparing `tmp/pulp-glue-maven-0.2.0.tar.gz` & `tmp/pulp-glue-maven-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-glue-maven-0.2.0.tar", last modified: Fri Mar 17 10:03:26 2023, max compression
+gzip compressed data, was "pulp-glue-maven-0.3.0.tar", last modified: Thu May 23 10:00:14 2024, max compression
```

## Comparing `pulp-glue-maven-0.2.0.tar` & `pulp-glue-maven-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:03:26.607374 pulp-glue-maven-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-17 10:03:26.607374 pulp-glue-maven-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:03:13.000000 pulp-glue-maven-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:03:26.607374 pulp-glue-maven-0.2.0/pulp_glue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:03:26.607374 pulp-glue-maven-0.2.0/pulp_glue/maven/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:03:13.000000 pulp-glue-maven-0.2.0/pulp_glue/maven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-03-17 10:03:13.000000 pulp-glue-maven-0.2.0/pulp_glue/maven/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:03:13.000000 pulp-glue-maven-0.2.0/pulp_glue/maven/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:03:26.607374 pulp-glue-maven-0.2.0/pulp_glue_maven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-17 10:03:26.000000 pulp-glue-maven-0.2.0/pulp_glue_maven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-17 10:03:26.000000 pulp-glue-maven-0.2.0/pulp_glue_maven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 10:03:26.000000 pulp-glue-maven-0.2.0/pulp_glue_maven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-17 10:03:26.000000 pulp-glue-maven-0.2.0/pulp_glue_maven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-17 10:03:26.000000 pulp-glue-maven-0.2.0/pulp_glue_maven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-17 10:03:13.000000 pulp-glue-maven-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 10:03:26.607374 pulp-glue-maven-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-17 10:03:13.000000 pulp-glue-maven-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:00:14.828301 pulp-glue-maven-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-23 10:00:14.828301 pulp-glue-maven-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:00:06.000000 pulp-glue-maven-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:00:14.828301 pulp-glue-maven-0.3.0/pulp_glue/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:00:14.828301 pulp-glue-maven-0.3.0/pulp_glue/maven/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 10:00:06.000000 pulp-glue-maven-0.3.0/pulp_glue/maven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-23 10:00:06.000000 pulp-glue-maven-0.3.0/pulp_glue/maven/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:00:06.000000 pulp-glue-maven-0.3.0/pulp_glue/maven/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:00:14.828301 pulp-glue-maven-0.3.0/pulp_glue_maven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-23 10:00:14.000000 pulp-glue-maven-0.3.0/pulp_glue_maven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-23 10:00:14.000000 pulp-glue-maven-0.3.0/pulp_glue_maven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:00:14.000000 pulp-glue-maven-0.3.0/pulp_glue_maven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-23 10:00:14.000000 pulp-glue-maven-0.3.0/pulp_glue_maven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 10:00:14.000000 pulp-glue-maven-0.3.0/pulp_glue_maven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-23 10:00:06.000000 pulp-glue-maven-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 10:00:14.828301 pulp-glue-maven-0.3.0/setup.cfg
```

### Comparing `pulp-glue-maven-0.2.0/PKG-INFO` & `pulp-glue-maven-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pulp-glue-maven
-Version: 0.2.0
-Summary: Version agnostic glue library to talk to pulpcore's REST API.
-Home-page: https://github.com/pulp/pulp-cli-maven
-Author: Pulp Team
-Author-email: pulp-list@redhat.com
+Version: 0.3.0
+Summary: Version agnostic glue library to talk to pulpcore's REST API. (Maven plugin)
+Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
+Project-URL: repository, https://github.com/pulp/pulp-cli-maven
+Project-URL: changelog, https://github.com/pulp/pulp-cli-maven/blob/main/CHANGES.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Software Distribution
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulp-glue-maven-0.2.0/pulp_glue/maven/context.py` & `pulp-glue-maven-0.3.0/pulp_glue/maven/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-maven-0.2.0/pulp_glue_maven.egg-info/PKG-INFO` & `pulp-glue-maven-0.3.0/pulp_glue_maven.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pulp-glue-maven
-Version: 0.2.0
-Summary: Version agnostic glue library to talk to pulpcore's REST API.
-Home-page: https://github.com/pulp/pulp-cli-maven
-Author: Pulp Team
-Author-email: pulp-list@redhat.com
+Version: 0.3.0
+Summary: Version agnostic glue library to talk to pulpcore's REST API. (Maven plugin)
+Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
+Project-URL: repository, https://github.com/pulp/pulp-cli-maven
+Project-URL: changelog, https://github.com/pulp/pulp-cli-maven/blob/main/CHANGES.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Software Distribution
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

