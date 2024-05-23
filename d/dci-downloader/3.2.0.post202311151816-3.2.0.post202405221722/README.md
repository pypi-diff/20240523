# Comparing `tmp/dci-downloader-3.2.0.post202311151816.tar.gz` & `tmp/dci-downloader-3.2.0.post202405221722.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dci-downloader-3.2.0.post202311151816.tar", last modified: Wed Nov 15 20:22:25 2023, max compression
+gzip compressed data, was "dci-downloader-3.2.0.post202405221722.tar", last modified: Thu May 23 13:22:37 2024, max compression
```

## Comparing `dci-downloader-3.2.0.post202311151816.tar` & `dci-downloader-3.2.0.post202405221722.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-15 20:22:25.857037 dci-downloader-3.2.0.post202311151816/
--rw-r--r--   0 root         (0) root         (0)    11337 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/LICENSE
--rw-r--r--   0 root         (0) root         (0)       58 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6113 2023-11-15 20:22:25.857037 dci-downloader-3.2.0.post202311151816/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5593 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-15 20:22:25.855037 dci-downloader-3.2.0.post202311151816/dci_downloader/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/dci_downloader/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6965 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/dci_downloader/api.py
--rw-r--r--   0 root         (0) root         (0)     5579 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/dci_downloader/cli.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/dci_downloader/containers.py
--rw-r--r--   0 root         (0) root         (0)     2017 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/dci_downloader/downloader.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/dci_downloader/files_list.py
--rw-r--r--   0 root         (0) root         (0)     1896 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/dci_downloader/filters.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/dci_downloader/fs.py
--rw-r--r--   0 root         (0) root         (0)      981 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/dci_downloader/lock.py
--rwxr-xr-x   0 root         (0) root         (0)     2337 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/dci_downloader/main.py
--rw-r--r--   0 root         (0) root         (0)     9773 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/dci_downloader/settings.py
--rw-r--r--   0 root         (0) root         (0)      803 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/dci_downloader/stats.py
--rw-r--r--   0 root         (0) root         (0)       51 2023-11-15 20:22:25.000000 dci-downloader-3.2.0.post202311151816/dci_downloader/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-15 20:22:25.856037 dci-downloader-3.2.0.post202311151816/dci_downloader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6113 2023-11-15 20:22:25.000000 dci-downloader-3.2.0.post202311151816/dci_downloader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      613 2023-11-15 20:22:25.000000 dci-downloader-3.2.0.post202311151816/dci_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-15 20:22:25.000000 dci-downloader-3.2.0.post202311151816/dci_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-11-15 20:22:25.000000 dci-downloader-3.2.0.post202311151816/dci_downloader.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-11-15 20:22:25.000000 dci-downloader-3.2.0.post202311151816/dci_downloader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-11-15 20:22:25.000000 dci-downloader-3.2.0.post202311151816/dci_downloader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-15 20:22:25.857037 dci-downloader-3.2.0.post202311151816/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2202 2023-11-15 20:21:08.000000 dci-downloader-3.2.0.post202311151816/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:22:37.293616 dci-downloader-3.2.0.post202405221722/
+-rw-r--r--   0 root         (0) root         (0)    11337 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6443 2024-05-23 13:22:37.292616 dci-downloader-3.2.0.post202405221722/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5923 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:22:37.291616 dci-downloader-3.2.0.post202405221722/dci_downloader/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/dci_downloader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/dci_downloader/api.py
+-rw-r--r--   0 root         (0) root         (0)     5993 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/dci_downloader/cli.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/dci_downloader/containers.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/dci_downloader/downloader.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/dci_downloader/files_list.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/dci_downloader/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/dci_downloader/fs.py
+-rw-r--r--   0 root         (0) root         (0)      981 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/dci_downloader/lock.py
+-rwxr-xr-x   0 root         (0) root         (0)     2337 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/dci_downloader/main.py
+-rw-r--r--   0 root         (0) root         (0)     9946 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/dci_downloader/settings.py
+-rw-r--r--   0 root         (0) root         (0)      803 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/dci_downloader/stats.py
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-23 13:22:36.000000 dci-downloader-3.2.0.post202405221722/dci_downloader/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:22:37.292616 dci-downloader-3.2.0.post202405221722/dci_downloader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6443 2024-05-23 13:22:36.000000 dci-downloader-3.2.0.post202405221722/dci_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      613 2024-05-23 13:22:37.000000 dci-downloader-3.2.0.post202405221722/dci_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 13:22:36.000000 dci-downloader-3.2.0.post202405221722/dci_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-23 13:22:36.000000 dci-downloader-3.2.0.post202405221722/dci_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-23 13:22:37.000000 dci-downloader-3.2.0.post202405221722/dci_downloader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-23 13:22:37.000000 dci-downloader-3.2.0.post202405221722/dci_downloader.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 13:22:37.293616 dci-downloader-3.2.0.post202405221722/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2202 2024-05-23 13:21:38.000000 dci-downloader-3.2.0.post202405221722/setup.py
```

### Comparing `dci-downloader-3.2.0.post202311151816/LICENSE` & `dci-downloader-3.2.0.post202405221722/LICENSE`

 * *Files identical despite different names*

### Comparing `dci-downloader-3.2.0.post202311151816/PKG-INFO` & `dci-downloader-3.2.0.post202405221722/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dci-downloader
-Version: 3.2.0.post202311151816
+Version: 3.2.0.post202405221722
 Summary: DCI downloader module
 Home-page: https://github.com/redhat-cip/dci-downloader
 Author: Distributed CI team
 Author-email: distributed-ci@redhat.com
 License: Apache v2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -169,14 +169,23 @@
 
 Download RHEL-9.2 compose with debug rpms
 
 ```console
 $ dci-downloader RHEL-9.2 /tmp/repo --debug
 ```
 
+### Download only specified packages
+
+To download packages specified on the command line, use the `--package-filter` flag
+
+Download all kernel and glibc packages for RHEL-8.8 for the ppc64le architecture
+
+```console
+$ dci-downloader RHEL-8.8 /tmp --variant BaseOS --arch ppc64le --package-filter=kernel --package-filter=glibc
+```
 ### Settings file
 
 You can use a settings file to send parameters to parameterize dci-downloader.
 
 Use `--settings` parameter:
 
 ```console
```

### Comparing `dci-downloader-3.2.0.post202311151816/README.md` & `dci-downloader-3.2.0.post202405221722/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -154,14 +154,23 @@
 
 Download RHEL-9.2 compose with debug rpms
 
 ```console
 $ dci-downloader RHEL-9.2 /tmp/repo --debug
 ```
 
+### Download only specified packages
+
+To download packages specified on the command line, use the `--package-filter` flag
+
+Download all kernel and glibc packages for RHEL-8.8 for the ppc64le architecture
+
+```console
+$ dci-downloader RHEL-8.8 /tmp --variant BaseOS --arch ppc64le --package-filter=kernel --package-filter=glibc
+```
 ### Settings file
 
 You can use a settings file to send parameters to parameterize dci-downloader.
 
 Use `--settings` parameter:
 
 ```console
```

### Comparing `dci-downloader-3.2.0.post202311151816/dci_downloader/api.py` & `dci-downloader-3.2.0.post202405221722/dci_downloader/api.py`

 * *Files identical despite different names*

### Comparing `dci-downloader-3.2.0.post202311151816/dci_downloader/cli.py` & `dci-downloader-3.2.0.post202405221722/dci_downloader/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,17 @@
   dci-downloader --settings settings.yml
 
   # load options from several yaml settings file (newer override older)
   dci-downloader --settings settings.yml --settings extra.yml
 
   # download the latest RHEL-9 development build
   dci-downloader --filter=compose:development RHEL-9.0 /tmp/repo
+
+  # download the latest RHEL-8 kernel packages for x86 and ppc64le architectures
+  dci-downloader dci-downloader RHEL-8.8 /tmp --variant BaseOS --arch x86_64 --arch ppc64le --package-filter=kernel
 """
 
 COPYRIGHT = """
 copyright:
   Copyright © 2019 Red Hat.
   Licensed under the Apache License, Version 2.0
 """
@@ -126,14 +129,21 @@
         action="append",
         dest="settings_files_paths",
         metavar="FILE_PATH",
         help="settings file(s) to overwrite cli parameters",
         default=[],
     )
     parser.add_argument("--version", action="version", version=__version__)
+    parser.add_argument(
+        "--package-filter",
+        action="append",
+        dest="package_filters",
+        help="Download only the specified package(s) (e.g. kernel, glibc, etc)",
+        default=[]
+    )
     parsed_arguments = parser.parse_args(arguments)
     if not parsed_arguments.archs:
         parsed_arguments.archs = ["x86_64"]
     parsed_arguments.archs = list(set(parsed_arguments.archs))
 
     if parsed_arguments.settings_files_paths is None:
         download_folder = parsed_arguments.download_folder
```

### Comparing `dci-downloader-3.2.0.post202311151816/dci_downloader/containers.py` & `dci-downloader-3.2.0.post202405221722/dci_downloader/containers.py`

 * *Files identical despite different names*

### Comparing `dci-downloader-3.2.0.post202311151816/dci_downloader/downloader.py` & `dci-downloader-3.2.0.post202405221722/dci_downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `dci-downloader-3.2.0.post202311151816/dci_downloader/files_list.py` & `dci-downloader-3.2.0.post202405221722/dci_downloader/files_list.py`

 * *Files identical despite different names*

### Comparing `dci-downloader-3.2.0.post202311151816/dci_downloader/fs.py` & `dci-downloader-3.2.0.post202405221722/dci_downloader/fs.py`

 * *Files identical despite different names*

### Comparing `dci-downloader-3.2.0.post202311151816/dci_downloader/lock.py` & `dci-downloader-3.2.0.post202405221722/dci_downloader/lock.py`

 * *Files identical despite different names*

### Comparing `dci-downloader-3.2.0.post202311151816/dci_downloader/main.py` & `dci-downloader-3.2.0.post202405221722/dci_downloader/main.py`

 * *Files identical despite different names*

### Comparing `dci-downloader-3.2.0.post202311151816/dci_downloader/settings.py` & `dci-downloader-3.2.0.post202405221722/dci_downloader/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
             "with_debug": with_debug,
             "with_source": with_source,
             "with_iso": False,
         }
         for v in variants
     ]
     filters = topic_info.get("filters", [])
+    package_filters = topic_info.get("package_filters", [])
     return {
         "name": name,
         "components": components,
         "archs": archs,
         "variants": variants,
         "download_everything": topic_info.get("download_everything", False),
         "download_folder": topic_info["download_folder"],
@@ -55,14 +56,15 @@
         "client_id": topic_info["client_id"],
         "api_secret": topic_info["api_secret"],
         "registry": topic_info["registry"],
         "component_id": component_id,
         "with_debug": with_debug,
         "with_source": with_source,
         "filters": filters,
+        "package_filters": package_filters,
     }
 
 
 def _clean_settings(settings):
     new_settings = []
     for topic in settings["topics"]:
         topic["download_folder"] = settings["download_folder"]
@@ -147,14 +149,15 @@
                 "with_debug": cli_arguments["with_debug"],
                 "with_source": cli_arguments["with_source"],
                 "name": topic_name,
                 "with_iso": cli_arguments["with_iso"],
                 "archs": cli_arguments["archs"],
                 "filters": cli_arguments["filters"],
                 "component_id": cli_arguments["component_id"],
+                "package_filters": cli_arguments["package_filters"],
             }
         )
 
     settings_from_files = {"download_folder": None, "registry": None, "topics": []}
     settings_files_paths = cli_arguments["settings_files_paths"]
     if settings_files_paths:
         settings_from_files.update(
```

### Comparing `dci-downloader-3.2.0.post202311151816/dci_downloader/stats.py` & `dci-downloader-3.2.0.post202405221722/dci_downloader/stats.py`

 * *Files identical despite different names*

### Comparing `dci-downloader-3.2.0.post202311151816/dci_downloader.egg-info/PKG-INFO` & `dci-downloader-3.2.0.post202405221722/dci_downloader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dci-downloader
-Version: 3.2.0.post202311151816
+Version: 3.2.0.post202405221722
 Summary: DCI downloader module
 Home-page: https://github.com/redhat-cip/dci-downloader
 Author: Distributed CI team
 Author-email: distributed-ci@redhat.com
 License: Apache v2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -169,14 +169,23 @@
 
 Download RHEL-9.2 compose with debug rpms
 
 ```console
 $ dci-downloader RHEL-9.2 /tmp/repo --debug
 ```
 
+### Download only specified packages
+
+To download packages specified on the command line, use the `--package-filter` flag
+
+Download all kernel and glibc packages for RHEL-8.8 for the ppc64le architecture
+
+```console
+$ dci-downloader RHEL-8.8 /tmp --variant BaseOS --arch ppc64le --package-filter=kernel --package-filter=glibc
+```
 ### Settings file
 
 You can use a settings file to send parameters to parameterize dci-downloader.
 
 Use `--settings` parameter:
 
 ```console
```

### Comparing `dci-downloader-3.2.0.post202311151816/dci_downloader.egg-info/SOURCES.txt` & `dci-downloader-3.2.0.post202405221722/dci_downloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dci-downloader-3.2.0.post202311151816/setup.py` & `dci-downloader-3.2.0.post202405221722/setup.py`

 * *Files identical despite different names*

