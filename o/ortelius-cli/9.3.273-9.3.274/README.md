# Comparing `tmp/ortelius-cli-9.3.273.tar.gz` & `tmp/ortelius_cli-9.3.274.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortelius-cli-9.3.273.tar", last modified: Wed Apr 10 17:20:04 2024, max compression
+gzip compressed data, was "ortelius_cli-9.3.274.tar", last modified: Thu May 23 17:02:39 2024, max compression
```

## Comparing `ortelius-cli-9.3.273.tar` & `ortelius_cli-9.3.274.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-10 17:20:04.010419 ortelius-cli-9.3.273/
--rw-r--r--   0 steve      (502) staff       (20)    10480 2023-12-11 19:25:24.000000 ortelius-cli-9.3.273/LICENSE
--rw-r--r--   0 steve      (502) staff       (20)       17 2023-12-11 19:25:24.000000 ortelius-cli-9.3.273/MANIFEST.in
--rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-10 17:20:04.009379 ortelius-cli-9.3.273/PKG-INFO
--rw-r--r--   0 steve      (502) staff       (20)      818 2023-12-11 19:25:24.000000 ortelius-cli-9.3.273/README.md
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-10 17:20:03.994422 ortelius-cli-9.3.273/bin/
--rwxr-xr-x   0 steve      (502) staff       (20)    71076 2024-04-10 17:19:43.000000 ortelius-cli-9.3.273/bin/dh
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-10 17:20:03.997767 ortelius-cli-9.3.273/deployhub/
--rw-r--r--   0 steve      (502) staff       (20)       65 2024-04-10 17:19:43.000000 ortelius-cli-9.3.273/deployhub/__init__.py
--rw-r--r--   0 steve      (502) staff       (20)    71203 2024-04-09 22:35:31.000000 ortelius-cli-9.3.273/deployhub/dhapi.py
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-10 17:20:04.001274 ortelius-cli-9.3.273/doc/
--rw-r--r--   0 steve      (502) staff       (20)    23768 2023-12-11 19:25:24.000000 ortelius-cli-9.3.273/doc/deployhub.md
--rw-r--r--   0 steve      (502) staff       (20)    11674 2023-12-11 19:25:24.000000 ortelius-cli-9.3.273/doc/dh.md
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-10 17:20:04.008158 ortelius-cli-9.3.273/ortelius_cli.egg-info/
--rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-10 17:20:03.000000 ortelius-cli-9.3.273/ortelius_cli.egg-info/PKG-INFO
--rw-r--r--   0 steve      (502) staff       (20)      292 2024-04-10 17:20:03.000000 ortelius-cli-9.3.273/ortelius_cli.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (502) staff       (20)        1 2024-04-10 17:20:03.000000 ortelius-cli-9.3.273/ortelius_cli.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (502) staff       (20)       68 2024-04-10 17:20:03.000000 ortelius-cli-9.3.273/ortelius_cli.egg-info/requires.txt
--rw-r--r--   0 steve      (502) staff       (20)       10 2024-04-10 17:20:03.000000 ortelius-cli-9.3.273/ortelius_cli.egg-info/top_level.txt
--rw-r--r--   0 steve      (502) staff       (20)       38 2024-04-10 17:20:04.010617 ortelius-cli-9.3.273/setup.cfg
--rw-r--r--   0 steve      (502) staff       (20)     1069 2024-04-10 17:19:43.000000 ortelius-cli-9.3.273/setup.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-05-23 17:02:39.662061 ortelius_cli-9.3.274/
+-rw-r--r--   0 steve      (502) staff       (20)    10480 2023-12-11 19:25:24.000000 ortelius_cli-9.3.274/LICENSE
+-rw-r--r--   0 steve      (502) staff       (20)       17 2023-12-11 19:25:24.000000 ortelius_cli-9.3.274/MANIFEST.in
+-rw-r--r--   0 steve      (502) staff       (20)    12461 2024-05-23 17:02:39.660884 ortelius_cli-9.3.274/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      818 2023-12-11 19:25:24.000000 ortelius_cli-9.3.274/README.md
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-05-23 17:02:39.638552 ortelius_cli-9.3.274/bin/
+-rwxr-xr-x   0 steve      (502) staff       (20)    71895 2024-05-23 17:02:09.000000 ortelius_cli-9.3.274/bin/dh
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-05-23 17:02:39.641035 ortelius_cli-9.3.274/deployhub/
+-rw-r--r--   0 steve      (502) staff       (20)       65 2024-05-23 17:02:09.000000 ortelius_cli-9.3.274/deployhub/__init__.py
+-rw-r--r--   0 steve      (502) staff       (20)    71203 2024-04-09 22:35:31.000000 ortelius_cli-9.3.274/deployhub/dhapi.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-05-23 17:02:39.646950 ortelius_cli-9.3.274/doc/
+-rw-r--r--   0 steve      (502) staff       (20)    23768 2023-12-11 19:25:24.000000 ortelius_cli-9.3.274/doc/deployhub.md
+-rw-r--r--   0 steve      (502) staff       (20)    11674 2023-12-11 19:25:24.000000 ortelius_cli-9.3.274/doc/dh.md
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-05-23 17:02:39.653341 ortelius_cli-9.3.274/ortelius_cli.egg-info/
+-rw-r--r--   0 steve      (502) staff       (20)    12461 2024-05-23 17:02:39.000000 ortelius_cli-9.3.274/ortelius_cli.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      292 2024-05-23 17:02:39.000000 ortelius_cli-9.3.274/ortelius_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (502) staff       (20)        1 2024-05-23 17:02:39.000000 ortelius_cli-9.3.274/ortelius_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (502) staff       (20)       68 2024-05-23 17:02:39.000000 ortelius_cli-9.3.274/ortelius_cli.egg-info/requires.txt
+-rw-r--r--   0 steve      (502) staff       (20)       10 2024-05-23 17:02:39.000000 ortelius_cli-9.3.274/ortelius_cli.egg-info/top_level.txt
+-rw-r--r--   0 steve      (502) staff       (20)       38 2024-05-23 17:02:39.662284 ortelius_cli-9.3.274/setup.cfg
+-rw-r--r--   0 steve      (502) staff       (20)     1069 2024-05-23 17:02:09.000000 ortelius_cli-9.3.274/setup.py
```

### Comparing `ortelius-cli-9.3.273/LICENSE` & `ortelius_cli-9.3.274/LICENSE`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.273/PKG-INFO` & `ortelius_cli-9.3.274/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortelius-cli
-Version: 9.3.273
+Version: 9.3.274
 Home-page: https://ortelius.io
 Author: Steve Taylor
 Author-email: steve@deployhub.com
 License: Apache-2.0
 Project-URL: Project Repo, https://github.com/ortelius/ortelius-cli
 Project-URL: Issues, https://github.com/ortelius/ortelius/issues
 Project-URL: Ortelius CLI Documentation, https://github.com/ortelius/ortelius-cli/blob/main/doc/dh.md
```

### Comparing `ortelius-cli-9.3.273/README.md` & `ortelius_cli-9.3.274/README.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.273/bin/dh` & `ortelius_cli-9.3.274/bin/dh`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     `--todom` To Domain
 
 """
 
 # To generate markdown use:
 # pydoc-markdown -I bin | awk '/dh.main/ {p=1}; p==0 {print}'
 
-__version__ = "9.3.273"
+__version__ = "9.3.274"
 
 import json
 import os
 import re
 import stat
 import sys
 from datetime import datetime
@@ -795,14 +795,20 @@
                 dockerrepo = attrs.get("DockerRepo", "")
                 if ":" in dockerrepo:
                     parts = dockerrepo.split(":")
                     attrs["DockerRepo"] = parts[0]
                     if attrs.get("DockerTag", None) is None:
                         attrs["DockerTag"] = parts[1]
 
+            if attrs.get("DockerTag", None) is not None:
+                dockerrepo = attrs.get("DockerRepo", "")
+                dockertag  = attrs.get("DockerTag", "")
+
+                attrs['Purl'] = docker_tag_to_purl(dockerrepo + ':' + dockertag)
+
             attrs["GitBranch"] = attrs.get("GitBranch", os.getenv("GIT_BRANCH", ""))
             attrs["GitBranchCreateCommit"] = attrs.get("GitBranchCreateCommit", os.getenv("GIT_BRANCH_CREATE_COMMIT", ""))
             attrs["GitBranchCreateTimestamp"] = attrs.get("GitBranchCreateTimestamp", os.getenv("GIT_BRANCH_CREATE_TIMESTAMP", ""))
             attrs["GitBranchParent"] = attrs.get("GitBranchParent", os.getenv("GIT_BRANCH_PARENT", ""))
             attrs["GitCommit"] = attrs.get("GitCommit", os.getenv("GIT_COMMIT", os.getenv("SHORT_SHA", "")))
             attrs["GitCommitAuthors"] = attrs.get("GitCommitAuthors", os.getenv("GIT_COMMIT_AUTHORS", ""))
             attrs["GitCommittersCnt"] = attrs.get("GitCommittersCnt", os.getenv("GIT_COMMITTERS_CNT", ""))
@@ -1651,10 +1657,28 @@
 
     for obj in allobjs.get(objtype, []):
         pprint(obj)
         jstr = json.dumps(obj, indent=2)
         data = dhapi.post_json(dhurl + "/dmadminweb/API/import/", jstr, cookies)
         pprint(data)
 
+def docker_tag_to_purl(docker_tag):
+    """
+    Converts a Docker tag to a Package URL (purl).
+    
+    Args:
+        docker_tag (str): The Docker tag to convert. Example: 'quay.io/deployhub/dh-ms-general:svccat-v11.0.265-gb537b3'
+        
+    Returns:
+        str: The corresponding purl.
+    """
+    # Split the docker tag into registry, namespace/repository, and tag
+    registry_repo, tag = docker_tag.split(':')
+    registry, repo = registry_repo.split('/', 1)
+    
+    # Construct the purl
+    purl = f"pkg:docker/{registry}/{repo}@{tag}"
+    
+    return purl
 
 if __name__ == "__main__":
     main()  # pyright: ignore [reportGeneralTypeIssues, reportCallIssue] # pylint: disable=no-value-for-parameter
```

### Comparing `ortelius-cli-9.3.273/deployhub/dhapi.py` & `ortelius_cli-9.3.274/deployhub/dhapi.py`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.273/doc/deployhub.md` & `ortelius_cli-9.3.274/doc/deployhub.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.273/doc/dh.md` & `ortelius_cli-9.3.274/doc/dh.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.273/ortelius_cli.egg-info/PKG-INFO` & `ortelius_cli-9.3.274/ortelius_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortelius-cli
-Version: 9.3.273
+Version: 9.3.274
 Home-page: https://ortelius.io
 Author: Steve Taylor
 Author-email: steve@deployhub.com
 License: Apache-2.0
 Project-URL: Project Repo, https://github.com/ortelius/ortelius-cli
 Project-URL: Issues, https://github.com/ortelius/ortelius/issues
 Project-URL: Ortelius CLI Documentation, https://github.com/ortelius/ortelius-cli/blob/main/doc/dh.md
```

### Comparing `ortelius-cli-9.3.273/setup.py` & `ortelius_cli-9.3.274/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "Issues": "https://github.com/ortelius/ortelius/issues",
         "Ortelius CLI Documentation": "https://github.com/ortelius/ortelius-cli/blob/main/doc/dh.md",
         "Python Python API Documentation": "https://github.com/ortelius/ortelius-cli/blob/main/doc/deployhub.md",
     },
     author="Steve Taylor",
     author_email="steve@deployhub.com",
     name="ortelius-cli",
-    version="9.3.273",
+    version="9.3.274",
     packages=[
         "deployhub",
     ],
     scripts=["bin/dh"],
     license="Apache-2.0",
     long_description=open("doc/dh.md").read(),
     long_description_content_type="text/markdown",
```

