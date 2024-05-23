# Comparing `tmp/cdk-fsx-ontap-1.0.8.tar.gz` & `tmp/cdk-fsx-ontap-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-fsx-ontap-1.0.8.tar", last modified: Sun Sep 17 06:46:51 2023, max compression
+gzip compressed data, was "cdk-fsx-ontap-1.0.9.tar", last modified: Fri Oct  6 14:25:28 2023, max compression
```

## Comparing `cdk-fsx-ontap-1.0.8.tar` & `cdk-fsx-ontap-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 06:46:51.427058 cdk-fsx-ontap-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-09-17 06:46:38.000000 cdk-fsx-ontap-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-09-17 06:46:38.000000 cdk-fsx-ontap-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-09-17 06:46:51.427058 cdk-fsx-ontap-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-09-17 06:46:38.000000 cdk-fsx-ontap-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-09-17 06:46:38.000000 cdk-fsx-ontap-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-17 06:46:51.427058 cdk-fsx-ontap-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2023-09-17 06:46:38.000000 cdk-fsx-ontap-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 06:46:51.423057 cdk-fsx-ontap-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 06:46:51.427058 cdk-fsx-ontap-1.0.8/src/cdk_fsx_ontap/
--rw-r--r--   0 runner    (1001) docker     (127)     8852 2023-09-17 06:46:38.000000 cdk-fsx-ontap-1.0.8/src/cdk_fsx_ontap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 06:46:51.427058 cdk-fsx-ontap-1.0.8/src/cdk_fsx_ontap/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-09-17 06:46:38.000000 cdk-fsx-ontap-1.0.8/src/cdk_fsx_ontap/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1218207 2023-09-17 06:46:38.000000 cdk-fsx-ontap-1.0.8/src/cdk_fsx_ontap/_jsii/cdk-fsx-ontap@1.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-17 06:46:38.000000 cdk-fsx-ontap-1.0.8/src/cdk_fsx_ontap/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 06:46:51.427058 cdk-fsx-ontap-1.0.8/src/cdk_fsx_ontap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-09-17 06:46:51.000000 cdk-fsx-ontap-1.0.8/src/cdk_fsx_ontap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-09-17 06:46:51.000000 cdk-fsx-ontap-1.0.8/src/cdk_fsx_ontap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-17 06:46:51.000000 cdk-fsx-ontap-1.0.8/src/cdk_fsx_ontap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-09-17 06:46:51.000000 cdk-fsx-ontap-1.0.8/src/cdk_fsx_ontap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-17 06:46:51.000000 cdk-fsx-ontap-1.0.8/src/cdk_fsx_ontap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:25:28.966192 cdk-fsx-ontap-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-10-06 14:25:12.000000 cdk-fsx-ontap-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-06 14:25:12.000000 cdk-fsx-ontap-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-10-06 14:25:28.966192 cdk-fsx-ontap-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-10-06 14:25:12.000000 cdk-fsx-ontap-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-06 14:25:12.000000 cdk-fsx-ontap-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-06 14:25:28.966192 cdk-fsx-ontap-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2023-10-06 14:25:12.000000 cdk-fsx-ontap-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:25:28.962192 cdk-fsx-ontap-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:25:28.962192 cdk-fsx-ontap-1.0.9/src/cdk_fsx_ontap/
+-rw-r--r--   0 runner    (1001) docker     (127)     8852 2023-10-06 14:25:12.000000 cdk-fsx-ontap-1.0.9/src/cdk_fsx_ontap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:25:28.966192 cdk-fsx-ontap-1.0.9/src/cdk_fsx_ontap/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2023-10-06 14:25:12.000000 cdk-fsx-ontap-1.0.9/src/cdk_fsx_ontap/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1218209 2023-10-06 14:25:12.000000 cdk-fsx-ontap-1.0.9/src/cdk_fsx_ontap/_jsii/cdk-fsx-ontap@1.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 14:25:12.000000 cdk-fsx-ontap-1.0.9/src/cdk_fsx_ontap/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:25:28.966192 cdk-fsx-ontap-1.0.9/src/cdk_fsx_ontap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-10-06 14:25:28.000000 cdk-fsx-ontap-1.0.9/src/cdk_fsx_ontap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2023-10-06 14:25:28.000000 cdk-fsx-ontap-1.0.9/src/cdk_fsx_ontap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 14:25:28.000000 cdk-fsx-ontap-1.0.9/src/cdk_fsx_ontap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-06 14:25:28.000000 cdk-fsx-ontap-1.0.9/src/cdk_fsx_ontap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-06 14:25:28.000000 cdk-fsx-ontap-1.0.9/src/cdk_fsx_ontap.egg-info/top_level.txt
```

### Comparing `cdk-fsx-ontap-1.0.8/LICENSE` & `cdk-fsx-ontap-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-fsx-ontap-1.0.8/PKG-INFO` & `cdk-fsx-ontap-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-fsx-ontap
-Version: 1.0.8
+Version: 1.0.9
 Summary: CDK construct for Amazon FSx for Netapp ONTAP
 Home-page: https://rafalkrol.xyz
 Author: Rafal Krol<ameotoko1+github@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/rafalkrol-xyz/cdk-fsx-ontap
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-fsx-ontap-1.0.8/README.md` & `cdk-fsx-ontap-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk-fsx-ontap-1.0.8/setup.py` & `cdk-fsx-ontap-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-fsx-ontap",
-    "version": "1.0.8",
+    "version": "1.0.9",
     "description": "CDK construct for Amazon FSx for Netapp ONTAP",
     "license": "MIT",
     "url": "https://rafalkrol.xyz",
     "long_description_content_type": "text/markdown",
     "author": "Rafal Krol<ameotoko1+github@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_fsx_ontap",
         "cdk_fsx_ontap._jsii"
     ],
     "package_data": {
         "cdk_fsx_ontap._jsii": [
-            "cdk-fsx-ontap@1.0.8.jsii.tgz"
+            "cdk-fsx-ontap@1.0.9.jsii.tgz"
         ],
         "cdk_fsx_ontap": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.85.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.88.0, <2.0.0",
+        "jsii>=1.89.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-fsx-ontap-1.0.8/src/cdk_fsx_ontap/__init__.py` & `cdk-fsx-ontap-1.0.9/src/cdk_fsx_ontap/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-fsx-ontap-1.0.8/src/cdk_fsx_ontap/_jsii/cdk-fsx-ontap@1.0.8.jsii.tgz` & `cdk-fsx-ontap-1.0.9/src/cdk_fsx_ontap/_jsii/cdk-fsx-ontap@1.0.9.jsii.tgz`

 * *Files 5% similar despite different names*

#### Comparing `cdk-fsx-ontap@1.0.8.jsii.tgz-content` & `cdk-fsx-ontap@1.0.9.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'fingerprint'": "'BzXapHn8wTj95N98qWxPNGZTY3EF4DLq2lH+arL+sSM='", "'version'": "'1.0.9'"}*

```diff
@@ -3473,15 +3473,15 @@
             }
         }
     },
     "description": "CDK construct for Amazon FSx for Netapp ONTAP",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "01Mg6nV6bidebMfyx99tQkQSCdJHG8a2mNFgb/kC4oo=",
+    "fingerprint": "BzXapHn8wTj95N98qWxPNGZTY3EF4DLq2lH+arL+sSM=",
     "homepage": "https://rafalkrol.xyz",
     "jsiiVersion": "5.0.19 (build bf5f37b)",
     "keywords": [
         "aws",
         "awscdk",
         "cdk",
         "fsx",
@@ -3704,9 +3704,9 @@
                         "primitive": "string"
                     }
                 }
             ],
             "symbolId": "src/index:FsxOntapProps"
         }
     },
-    "version": "1.0.8"
+    "version": "1.0.9"
 }
```

##### package/lib/index.js

###### js-beautify {}

```diff
@@ -131,11 +131,11 @@
         fsxSecurityGroup.addIngressRule(securityGroupSource, aws_ec2_1.Port.udp(4046));
         fsxSecurityGroup.addIngressRule(securityGroupSource, aws_ec2_1.Port.udp(4049));
     }
 }
 _a = JSII_RTTI_SYMBOL_1;
 FsxOntap[_a] = {
     fqn: "cdk-fsx-ontap.FsxOntap",
-    version: "1.0.8"
+    version: "1.0.9"
 };
 exports.FsxOntap = FsxOntap;
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiaW5kZXguanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvaW5kZXgudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSw2Q0FBK0Q7QUFDL0QsaURBQXFFO0FBQ3JFLHVFQUF3RDtBQUN4RCwyQ0FBdUM7QUEwQnZDLE1BQWEsUUFBUyxTQUFRLHNCQUFTO0lBS3JDLFlBQVksS0FBZ0IsRUFBRSxFQUFVLEVBQUUsS0FBb0I7UUFDNUQsS0FBSyxDQUFDLEtBQUssRUFBRSxFQUFFLENBQUMsQ0FBQztRQUpWLGNBQVMsR0FBVyxVQUFVLENBQUM7UUFDL0IsY0FBUyxHQUFXLFVBQVUsQ0FBQztRQUt0QyxNQUFNLElBQUksR0FBRyxLQUFLLENBQUMsSUFBSSxJQUFJLFdBQVcsQ0FBQztRQUV2QyxJQUFJLEtBQUssQ0FBQyxTQUFTLEVBQUU7WUFDbkIsSUFBSSxDQUFDLFNBQVMsR0FBRyxLQUFLLENBQUMsU0FBUyxDQUFDO1NBQ2xDO1FBRUQsSUFBSSxLQUFLLENBQUMsU0FBUyxFQUFFO1lBQ25CLElBQUksQ0FBQyxTQUFTLEdBQUcsS0FBSyxDQUFDLFNBQVMsQ0FBQztTQUNsQztRQUVELE1BQU0sR0FBRyxHQUFHLEtBQUssQ0FBQyxHQUFHLENBQUM7UUFDdEI7Ozs7VUFJRTtRQUNGLE1BQU0sb0JBQW9CLEdBQUcsR0FBRyxDQUFDLGNBQWMsQ0FBQyxLQUFLLENBQUMsQ0FBQyxFQUFFLENBQUMsQ0FBQyxDQUFDO1FBRTVELElBQUksb0JBQW9CLENBQUMsTUFBTSxLQUFLLENBQUMsSUFBSSxvQkFBb0IsQ0FBQyxNQUFNLEtBQUssQ0FBQyxFQUFFO1lBQzFFLE1BQU0sSUFBSSxLQUFLLENBQUMsaUdBQWlHLENBQUMsQ0FBQztTQUNwSDtRQUVELG9FQUFvRTtRQUNwRSxNQUFNLGdCQUFnQixHQUFHLElBQUksMkJBQU0sQ0FBQyxJQUFJLEVBQUUsR0FBRyxJQUFJLEVBQUUsRUFBRTtZQUNuRCxvQkFBb0IsRUFBRTtnQkFDcEIsa0JBQWtCLEVB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bUJBQW1CLEVBQUUsY0FBSSxDQUFDLEdBQUcsQ0FBQyxHQUFHLENBQUMsQ0FBQyxDQUFDO1FBQ3BFLGdCQUFnQixDQUFDLGNBQWMsQ0FBQyxtQkFBbUIsRUFBRSxjQUFJLENBQUMsR0FBRyxDQUFDLEdBQUcsQ0FBQyxDQUFDLENBQUM7UUFDcEUsZ0JBQWdCLENBQUMsY0FBYyxDQUFDLG1CQUFtQixFQUFFLGNBQUksQ0FBQyxHQUFHLENBQUMsR0FBRyxDQUFDLENBQUMsQ0FBQztRQUNwRSxnQkFBZ0IsQ0FBQyxjQUFjLENBQUMsbUJBQW1CLEVBQUUsY0FBSSxDQUFDLEdBQUcsQ0FBQyxHQUFHLENBQUMsQ0FBQyxDQUFDO1FBQ3BFLGdCQUFnQixDQUFDLGNBQWMsQ0FBQyxtQkFBbUIsRUFBRSxjQUFJLENBQUMsR0FBRyxDQUFDLElBQUksQ0FBQyxDQUFDLENBQUM7UUFDckUsZ0JBQWdCLENBQUMsY0FBYyxDQUFDLG1CQUFtQixFQUFFLGNBQUksQ0FBQyxHQUFHLENBQUMsSUFBSSxDQUFDLENBQUMsQ0FBQztRQUNyRSxnQkFBZ0IsQ0FBQyxjQUFjLENBQUMsbUJBQW1CLEVBQUUsY0FBSSxDQUFDLEdBQUcsQ0FBQyxJQUFJLENBQUMsQ0FBQyxDQUFDO1FBQ3JFLGdCQUFnQixDQUFDLGNBQWMsQ0FBQyxtQkFBbUIsRUFBRSxjQUFJLENBQUMsR0FBRyxDQUFDLElBQUksQ0FBQyxDQUFDLENBQUM7UUFDckUsZ0JBQWdCLENBQUMsY0FBYyxDQUFDLG1CQUFtQixFQUFFLGNBQUksQ0FBQyxHQUFHLENBQUMsS0FBSyxDQUFDLENBQUMsQ0FBQztRQUN0RSxnQkFBZ0IsQ0FBQyxjQUFjLENBQUMsbUJBQW1CLEVBQUUsY0FBSSxDQUFDLEdBQUcsQ0FBQyxLQUFLLENBQUMsQ0FBQyxDQUFDO1FBQ3RFLGdCQUFnQixDQUFDLGNBQWMsQ0FBQyxtQkFBbUIsRUFBRSxjQUFJLENBQUMsR0FBRyxDQUFDLEdBQUcsQ0FBQyxDQUFDLENBQUM7UUFDcEUsZ0JBQWdCLENBQUMsY0FBYyxDQUFDLG1CQUFtQixFQUFFLGNBQUksQ0FBQyxHQUFHLENBQUMsR0FBRyxDQUFDLENBQUMsQ0FBQztRQUNwRSxnQkFBZ0IsQ0FBQyxjQUFjLENBQUMsbUJBQW1CLEVBQUUsY0FBSSxDQUFDLEdBQUcsQ0FBQyxHQUFHLENBQUMsQ0FBQyxDQUFDO1FBQ3BFLGdCQUFnQixDQUFDLGNBQWMsQ0FBQyxtQkFBbUIsRUFBRSxjQUFJLENBQUMsR0FBRyxDQUFDLEdBQUcsQ0FBQyxDQUFDLENBQUM7UUFDcEUsZ0JBQWdCLENBQUMsY0FBYyxDQUFDLG1CQUFtQixFQUFFLGNBQUksQ0FBQyxHQUFHLENBQUMsR0FBRyxDQUFDLENBQUMsQ0FBQztRQUNwRSxnQkFBZ0IsQ0FBQyxjQUFjLENBQUMsbUJBQW1CLEVBQUUsY0FBSSxDQUFDLEdBQUcsQ0FBQyxHQUFHLENBQUMsQ0FBQyxDQUFDO1FBQ3BFLGdCQUFnQixDQUFDLGNBQWMsQ0FBQyxtQkFBbUIsRUFBRSxjQUFJLENBQUMsR0FBRyxDQUFDLEdBQUcsQ0FBQyxDQUFDLENBQUM7UUFDcEUsZ0JBQWdCLENBQUMsY0FBYyxDQUFDLG1CQUFtQixFQUFFLGNBQUksQ0FBQyxHQUFHLENBQUMsSUFBSSxDQUFDLENBQUMsQ0FBQztRQUNyRSxnQkFBZ0IsQ0FBQyxjQUFjLENBQUMsbUJBQW1CLEVBQUUsY0FBSSxDQUFDLEdBQUcsQ0FBQyxJQUFJLENBQUMsQ0FBQyxDQUFDO1FBQ3JFLGdCQUFnQixDQUFDLGNBQWMsQ0FBQyxtQkFBbUIsRUFBRSxjQUFJLENBQUMsR0FBRyxDQUFDLElBQUksQ0FBQyxDQUFDLENBQUM7UUFDckUsZ0JBQWdCLENBQUMsY0FBYyxDQUFDLG1CQUFtQixFQUFFLGNBQUksQ0FBQyxHQUFHLENBQUMsSUFBSSxDQUFDLENBQUMsQ0FBQztJQUN2RSxDQUFDOzs7O0FBaEpVLDRCQUFRIiwic291cmNlc0NvbnRlbnQiOlsiaW1wb3J0IHsgU3RhY2ssIGF3c19mc3ggYXMgZnN4LCBDZm5PdXRwdXQgfSBmcm9tICdhd3MtY2RrLWxpYic7XG5pbXBvcnQgeyBTZWN1cml0eUdyb3VwLCBWcGMsIFBlZXIsIFBvcnQgfSBmcm9tICdhd3MtY2RrLWxpYi9hd3MtZWMyJztcbmltcG9ydCB7IFNlY3JldCB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1zZWNyZXRzbWFuYWdlcic7XG5pbXBvcnQgeyBDb25zdHJ1Y3QgfSBmcm9tICdjb25zdHJ1Y3RzJztcblxuZXhwb3J0IGludGVyZmFjZSBGc3hPbnRhcFByb3BzIHtcbiAgLyoqXG4gICAqIE5hbWUgb2YgdGhlIEZTeCBmb3IgTmV0QXBwIE9OVEFQIFN0b3JhZ2UgVmlydHVhbCBNYWNoaW5lIChTVk0pLlxuICAgKiBBbHNvIHVzZWQgaW4gcmVzb3VyY2UgSUQgY3JlYXRpb24sIGUuZy4gYCR7bmFtZX0tcmVzb3VyY2UtdHlwZWAuXG4gICAqIEBkZWZhdWx0ICdmc3gtb250YXAnXG4gICAqL1xuICByZWFkb25seSBuYW1lPzogc3RyaW5nO1xuICAvKipcbiAgICogUGF0aCB0byBtb3VudCB0aGUgRlN4IGZvciBOZXRBcHAgT05UQVAgaW5zdGFuY2UuXG4gICAqIEBkZWZhdWx0ICcvbW50L2ZzeCdcbiAgICovXG4gIHJlYWRvbmx5IG1vdW50UGF0aD86IHN0cmluZztcbiAgLyoqXG4gICAqIE5hbWUgb2YgdGhlIG1vdW50IHBvaW50LlxuICAgKiBAZGVmYXVsdCAnL2RhdGF2b2wnXG4gICAqL1xuICByZWFkb25seSBtb3VudE5hbWU/OiBzdHJpbmc7XG4gIC8qKlxuICAgKiBWUEMgaW4gd2hpY2ggdGhlIEZTeCBmb3IgTmV0QXBwIE9OVEFQIGluc3RhbmNlIHdpbGwgYmUgY3JlYXRlZC5cbiAgICovXG4gIHJlYWRvbmx5IHZwYzogVnBjO1xuICByZWFkb25seSBzZWN1cml0eUdyb3VwU291cmNlOiBTZWN1cml0eUdyb3VwO1xufVxuXG5leHBvcnQgY2xhc3MgRnN4T250YXAgZXh0ZW5kcyBDb25zdHJ1Y3Qge1xuICByZWFkb25seSBkbnNOYW1lOiBzdHJpbmcgfCB1bmRlZmluZWQ7XG4gIHJlYWRvbmx5IG1vdW50UGF0aDogc3RyaW5nID0gJy9tbnQvZnN4JztcbiAgcmVhZG9ubHkgbW91bnROYW1lOiBzdHJpbmcgPSAnL2RhdGF2b2wnO1xuXG4gIGNvbnN0cnVjdG9yKHNjb3BlOiBDb25zdHJ1Y3QsIGlkOiBzdHJpbmcsIHByb3BzOiBGc3hPbnRhcFByb3BzKSB7XG4gICAgc3VwZXIoc2NvcGUsIGlkKTtcblxuICAgIGNvbnN0IG5hbWUgPSBwcm9wcy5uYW1lID8/ICdmc3gtb250YXAnO1xuXG4gICAgaWYgKHByb3BzLm1vdW50TmFtZSkge1xuICAgICAgdGhpcy5tb3VudE5hbWUgPSBwcm9wcy5tb3VudE5hbWU7XG4gICAgfVxuXG4gICAgaWYgKHByb3BzLm1vdW50UGF0aCkge1xuICAgICAgdGhpcy5tb3VudFBhdGggPSBwcm9wcy5tb3VudFBhdGg7XG4gICAgfVxuXG4gICAgY29uc3QgdnBjID0gcHJvcHMudnBjO1xuICAgIC8qKlxuICAgICogQW1hem9uIEZTeCBmb3IgTmV0QXBwIE9OVEFQIGFjY2VwdHMgZWl0aGVyIG9uZSBvciB0d28gc3VibmV0cy5cbiAgICAqIE5CLCB0aGlzIGNvbnN0cnVjdCByZXF1aXJlcyB0aGVtIHRvIGJlIHByaXZhdGUgb25lcy5cbiAgICAqIEBzZWUgaHR0cHM6Ly9kb2NzLmF3cy5hbWF6b24uY29tL2ZzeC9sYXRlc3QvT05UQVBHdWlkZS9oaWdoLWF2YWlsYWJpbGl0eS1BWi5odG1sXG4gICAgKi9cbiAgICBjb25zdCBwcml2YXRlU3VibmV0c0ZvckZzeCA9IHZwYy5wcml2YXRlU3VibmV0cy5zbGljZSgwLCAyKTtcblxuICAgIGlmIChwcml2YXRlU3VibmV0c0ZvckZzeC5sZW5ndGggIT09IDIgJiYgcHJpdmF0ZVN1Ym5ldHNGb3JGc3gubGVuZ3RoICE9PSAxKSB7XG4gICAgICB0aHJvdyBuZXcgRXJyb3IoJ0ZTeCBmb3IgTmV0QXBwIE9OVEFQIGFjY2VwdHMgZWl0aGVyIG9uZSBvciB0d28gc3VibmV0cy4gTW9yZW92ZXIsIHRoZXkgbXVzdCBiZSBwcml2YXRlIHN1Ym5ldHMhJyk7XG4gICAgfVxuXG4gICAgLy8gQ3JlYXRlIGEgcmFuZG9tIHBhc3N3b3JkIGZvciB0aGUgRlN4IGZvciBOZXRBcHAgT05UQVAgYWRtaW4gdXNlci5cbiAgICBjb25zdCBmc3hBZG1pblBhc3N3b3JkID0gbmV3IFNlY3JldCh0aGlzLCBgJHtuYW1lfWAsIHtcbiAgICAgIGdlbmVyYXRlU2VjcmV0U3RyaW5nOiB7XG4gICAgICAgIGV4Y2x1ZGVQdW5jdHVhdGlvbjogdHJ1ZSxcbiAgICAgIH0sXG4gICAgfSk7XG5cbiAgICBjb25zdCBmc3hTZWN1cml0eUdyb3VwID0gbmV3IFNlY3VyaXR5R3JvdXAodGhpcywgYCR7bmFtZX0tZnN4LXNlY3VyaXR5LWdyb3VwYCwge1xuICAgICAgdnBjLFxuICAgICAgZGVzY3JpcHRpb246ICdUaGUgc2VjdXJpdHkgZ3JvdXAgZm9yIHRoZSBGU3ggZm9yIE5ldEFwcCBPTlRBUCBzZXJ2aWNlJyxcbiAgICAgIGFsbG93QWxsT3V0Ym91bmQ6IHRydWUsXG4gICAgfSk7XG4gICAgdGhpcy5hZGRJbmdyZXNzVG9Gc3hGcm9tU291cmNlU2cocHJvcHMuc2VjdXJpdHlHcm91cFNvdXJjZSwgZnN4U2VjdXJpdHlHcm91cCk7XG5cbiAgICBjb25zdCBjZm5GaWxlU3lzdGVtID0gbmV3IGZzeC5DZm5GaWxlU3lzdGVtKHRoaXMsIGAke25hbWV9LWZpbGVzeXN0ZW1gLCB7XG4gICAgICBmaWxlU3lzdGVtVHlwZTogJ09OVEFQJyxcbiAgICAgIHN1Ym5ldElkczogcHJpdmF0ZVN1Ym5ldHNGb3JGc3gubWFwKHMgPT4gcy5zdWJuZXRJZCksXG5cbiAgICAgIG9udGFwQ29uZmlndXJhdGlvbjoge1xuICAgICAgICBmc3hBZG1pblBhc3N3b3JkOiBmc3hBZG1pblBhc3N3b3JkLnNlY3JldFZhbHVlLnRvU3RyaW5nKCksXG4gICAgICAgIGRlcGxveW1lbnRUeXBlOiBwcml2YXRlU3VibmV0c0ZvckZzeC5sZW5ndGggPT09IDIgPyAnTVVMVElfQVpfMScgOiAnU0lOR0xFX0FaXzEnLFxuICAgICAgICBkaXNrSW9wc0NvbmZpZ3VyYXRpb246IHtcbiAgICAgICAgICBpb3BzOiA0MDAwMCxcbiAgICAgICAgICBtb2RlOiAnVVNFUl9QUk9WSVNJT05FRCcsXG4gICAgICAgIH0sXG4gICAgICAgIHByZWZlcnJlZFN1Ym5ldElkOiBwcml2YXRlU3VibmV0c0ZvckZzeFswXS5zdWJuZXRJZCxcbiAgICAgICAgcm91dGVUYWJsZUlkczogcHJpdmF0ZVN1Ym5ldHNGb3JGc3gubWFwKHMgPT4gcy5yb3V0ZVRhYmxlLnJvdXRlVGFibGVJZCksXG4gICAgICAgIHRocm91Z2hwdXRDYXBhY2l0eTogMjU2LFxuICAgICAgfSxcbiAgICAgIHNlY3VyaXR5R3JvdXBJZHM6IFtmc3hTZWN1cml0eUdyb3VwLnNlY3VyaXR5R3JvdXBJZF0sXG4gICAgICBzdG9yYWdlQ2FwYWNpdHk6IDEwMjQwLFxuICAgICAgc3RvcmFnZVR5cGU6ICdTU0QnLFxuICAgIH0pO1xuXG4gICAgY29uc3Qgc3ZtID0gbmV3IGZzeC5DZm5TdG9yYWdlVmlydHVhbE1hY2hpbmUodGhpcywgYCR7bmFtZX0tc3ZtYCwge1xuICAgICAgbmFtZSxcbiAgICAgIGZpbGVTeXN0ZW1JZDogY2ZuRmlsZVN5c3RlbS5yZWYsXG4gICAgICByb290Vm9sdW1lU2VjdXJpdHlTdHlsZTogJ01JWEVEJyxcbiAgICB9KTtcblxuICAgIG5ldyBmc3guQ2ZuVm9sdW1lKHRoaXMsIGAke25hbWV9LXZvbHVtZWAsIHtcbiAgICAgIC8qKlxuICAgICAgICogQSB2b2x1bWUgbmFtZSBtdXN0IGJlZ2luIHdpdGggYSBsZXR0ZXIgb3IgdW5kZXJzY29yZSxcbiAgICAgICAqIGNhbiBvbmx5IGNvbnRhaW4gYWxwaGFudW1lcmljIGNoYXJhY3RlcnMgb3IgdW5kZXJzY29yZXMgKGBfYCksXG4gICAgICAgKiBhbmQgY2Fubm90IGV4Y2VlZCAyMDMgY2hhcmFjdGVycyBpbiBsZW5ndGhcbiAgICAgICAqL1xuICAgICAgbmFtZTpcbiAgICAgICAgdGhpcy50cmltU3RyaW5nQXQyMDNyZENoYXJhY3RlcihcbiAgICAgICAgICB0aGlzLnJlbW92ZU5vbkFscGhhbnVtZXJpY09yVW5kZXJzY29yZXMoXG4gICAgICAgICAgICB0aGlzLnJlcGxhY2VEYXNoZXNXaXRoVW5kZXJzY29yZXMobmFtZSksXG4gICAgICAgICAgKS5jb25jYXQoJ3ZvbHVtZScpKSxcbiAgICAgIHZvbHVtZVR5cGU6ICdPTlRBUCcsXG4gICAgICBvbnRhcENvbmZpZ3VyYXRpb246IHtcbiAgICAgICAganVuY3Rpb25QYXRoOiB0aGlzLm1vdW50TmFtZSxcbiAgICAgICAgc2VjdXJpdHlTdHlsZTogJ01JWEVEJyxcbiAgICAgICAgc2l6ZUluTWVnYWJ5dGVzOiAnMTAyNDAwJyxcbiAgICAgICAgc3RvcmFnZVZpcnR1YWxNYWNoaW5lSWQ6IHN2bS5yZWYsXG4gICAgICAgIHN0b3JhZ2VFZmZpY2llbmN5RW5hYmxlZDogJ3RydWUnLFxuICAgICAgfSxcbiAgICB9KTtcblxuICAgIHRoaXMuZG5zTmFtZSA9IGAke3N2bS5sb2dpY2FsSWR9LiR7Y2ZuRmlsZVN5c3RlbS5yZWZ9LmZzeC4ke1N0YWNrLm9mKHRoaXMpLnJlZ2lvbn0uYW1hem9uYXdzLmNvbWA7XG5cbiAgICBuZXcgQ2ZuT3V0cHV0KHRoaXMsIGAke25hbWV9LWZzeC1hZG1pbi1wYXNzd29yZC1uYW1lYCwge1xuICAgICAgdmFsdWU6IGZzeEFkbWluUGFzc3dvcmQuc2VjcmV0TmFtZSxcbiAgICB9KTtcbiAgfVxuXG4gIHByaXZhdGUgcmVwbGFjZURhc2hlc1dpdGhVbmRlcnNjb3JlcyhzdHI6IHN0cmluZyk6IHN0cmluZyB7XG4gICAgcmV0dXJuIHN0ci5yZXBsYWNlKC8tL2csICdfJyk7XG4gIH1cblxuICBwcml2YXRlIHJlbW92ZU5vbkFscGhhbnVtZXJpY09yVW5kZXJzY29yZXMoc3RyOiBzdHJpbmcpOiBzdHJpbmcge1xuICAgIHJldHVybiBzdHIucmVwbGFjZSgvW15hLXpBLVowLTlfXS9nLCAnJyk7XG4gIH1cblxuICBwcml2YXRlIHRyaW1TdHJpbmdBdDIwM3JkQ2hhcmFjdGVyKHN0cjogc3RyaW5nKTogc3RyaW5nIHtcbiAgICByZXR1cm4gc3RyLnN1YnN0cmluZygwLCAyMDIpO1xuICB9XG5cbiAgLyoqXG4gICogQ29uZmlndXJlIFNlY3VyaXR5IEdyb3VwIGZvciBGc1hcbiAgKiBAc2VlIGh0dHBzOi8vZG9jcy5hd3MuYW1hem9uLmNvbS9mc3gvbGF0ZXN0L09OVEFQR3VpZGUvbGltaXQtYWNjZXNzLXNlY3VyaXR5LWdyb3Vwcy5odG1sXG4gICovXG4gIHByaXZhdGUgYWRkSW5ncmVzc1RvRnN4RnJvbVNvdXJjZVNnKHNlY3VyaXR5R3JvdXBTb3VyY2U6IFNlY3VyaXR5R3JvdXAsIGZzeFNlY3VyaXR5R3JvdXA6IFNlY3VyaXR5R3JvdXApOiB2b2lkIHtcbiAgICBmc3hTZWN1cml0eUdyb3VwLmFkZEluZ3Jlc3NSdWxlKFBlZXIuYW55SXB2NCgpLCBQb3J0LnRjcCgyMDQ5KSwgJ0FsbG93IDIwNDkgaW5ib3VuZCBmcm9tIGFueXdoZXJlJyk7XG4gICAgZnN4U2VjdXJpdHlHcm91cC5hZGRJbmdyZXNzUnVsZShzZWN1cml0eUdyb3VwU291cmNlLCBQb3J0LmljbXBQaW5nKCkpO1xuICAgIGZzeFNlY3VyaXR5R3JvdXAuYWRkSW5ncmVzc1J1bGUoc2VjdXJpdHlHcm91cFNvdXJjZSwgUG9ydC50Y3AoMjIpKTtcbiAgICBmc3hTZWN1cml0eUdyb3VwLmFkZEluZ3Jlc3NSdWxlKHNlY3VyaXR5R3JvdXBTb3VyY2UsIFBvcnQudGNwKDExMSkpO1xuICAgIGZzeFNlY3VyaXR5R3JvdXAuYWRkSW5ncmVzc1J1bGUoc2VjdXJpdHlHcm91cFNvdXJjZSwgUG9ydC50Y3AoMTM1KSk7XG4gICAgZnN4U2VjdXJpdHlHcm91cC5hZGRJbmdyZXNzUnVsZShzZWN1cml0eUdyb3VwU291cmNlLCBQb3J0LnRjcCgxMzkpKTtcbiAgICBmc3hTZWN1cml0eUdyb3VwLmFkZEluZ3Jlc3NSdWxlKHNlY3VyaXR5R3JvdXBTb3VyY2UsIFBvcnQudGNwKDE2MSkpO1xuICAgIGZzeFNlY3VyaXR5R3JvdXAuYWRkSW5ncmVzc1J1bGUoc2VjdXJpdHlHcm91cFNvdXJjZSwgUG9ydC50Y3AoMTYyKSk7XG4gICAgZnN4U2VjdXJpdHlHcm91cC5hZGRJbmdyZXNzUnVsZShzZWN1cml0eUdyb3VwU291cmNlLCBQb3J0LnRjcCg0NDMpKTtcbiAgICBmc3hTZWN1cml0eUdyb3VwLmFkZEluZ3Jlc3NSdWxlKHNlY3VyaXR5R3JvdXBTb3VyY2UsIFBvcnQudGNwKDQ0NSkpO1xuICAgIGZzeFNlY3VyaXR5R3JvdXAuYWRkSW5ncmVzc1J1bGUoc2VjdXJpdHlHcm91cFNvdXJjZSwgUG9ydC50Y3AoNjM1KSk7XG4gICAgZnN4U2VjdXJpdHlHcm91cC5hZGRJbmdyZXNzUnVsZShzZWN1cml0eUdyb3VwU291cmNlLCBQb3J0LnRjcCg3NDkpKTtcbiAgICBmc3hTZWN1cml0eUdyb3VwLmFkZEluZ3Jlc3NSdWxlKHNlY3VyaXR5R3JvdXBTb3VyY2UsIFBvcnQudGNwKDIwNDkpKTtcbiAgICBmc3hTZWN1cml0eUdyb3VwLmFkZEluZ3Jlc3NSdWxlKHNlY3VyaXR5R3JvdXBTb3VyY2UsIFBvcnQudGNwKDMyNjApKTtcbiAgICBmc3hTZWN1cml0eUdyb3VwLmFkZEluZ3Jlc3NSdWxlKHNlY3VyaXR5R3JvdXBTb3VyY2UsIFBvcnQudGNwKDQwNDUpKTtcbiAgICBmc3hTZWN1cml0eUdyb3VwLmFkZEluZ3Jlc3NSdWxlKHNlY3VyaXR5R3JvdXBTb3VyY2UsIFBvcnQudGNwKDQwNDYpKTtcbiAgICBmc3hTZWN1cml0eUdyb3VwLmFkZEluZ3Jlc3NSdWxlKHNlY3VyaXR5R3JvdXBTb3VyY2UsIFBvcnQudGNwKDExMTA0KSk7XG4gICAgZnN4U2VjdXJpdHlHcm91cC5hZGRJbmdyZXNzUnVsZShzZWN1cml0eUdyb3VwU291cmNlLCBQb3J0LnRjcCgxMTEwNSkpO1xuICAgIGZzeFNlY3VyaXR5R3JvdXAuYWRkSW5ncmVzc1J1bGUoc2VjdXJpdHlHcm91cFNvdXJjZSwgUG9ydC51ZHAoMTExKSk7XG4gICAgZnN4U2VjdXJpdHlHcm91cC5hZGRJbmdyZXNzUnVsZShzZWN1cml0eUdyb3VwU291cmNlLCBQb3J0LnVkcCgxMzUpKTtcbiAgICBmc3hTZWN1cml0eUdyb3VwLmFkZEluZ3Jlc3NSdWxlKHNlY3VyaXR5R3JvdXBTb3VyY2UsIFBvcnQudWRwKDEzNykpO1xuICAgIGZzeFNlY3VyaXR5R3JvdXAuYWRkSW5ncmVzc1J1bGUoc2VjdXJpdHlHcm91cFNvdXJjZSwgUG9ydC51ZHAoMTM5KSk7XG4gICAgZnN4U2VjdXJpdHlHcm91cC5hZGRJbmdyZXNzUnVsZShzZWN1cml0eUdyb3VwU291cmNlLCBQb3J0LnVkcCgxNjEpKTtcbiAgICBmc3hTZWN1cml0eUdyb3VwLmFkZEluZ3Jlc3NSdWxlKHNlY3VyaXR5R3JvdXBTb3VyY2UsIFBvcnQudWRwKDE2MikpO1xuICAgIGZzeFNlY3VyaXR5R3JvdXAuYWRkSW5ncmVzc1J1bGUoc2VjdXJpdHlHcm91cFNvdXJjZSwgUG9ydC51ZHAoNjM1KSk7XG4gICAgZnN4U2VjdXJpdHlHcm91cC5hZGRJbmdyZXNzUnVsZShzZWN1cml0eUdyb3VwU291cmNlLCBQb3J0LnVkcCgyMDQ5KSk7XG4gICAgZnN4U2VjdXJpdHlHcm91cC5hZGRJbmdyZXNzUnVsZShzZWN1cml0eUdyb3VwU291cmNlLCBQb3J0LnVkcCg0MDQ1KSk7XG4gICAgZnN4U2VjdXJpdHlHcm91cC5hZGRJbmdyZXNzUnVsZShzZWN1cml0eUdyb3VwU291cmNlLCBQb3J0LnVkcCg0MDQ2KSk7XG4gICAgZnN4U2VjdXJpdHlHcm91cC5hZGRJbmdyZXNzUnVsZShzZWN1cml0eUdyb3VwU291cmNlLCBQb3J0LnVkcCg0MDQ5KSk7XG4gIH1cbn1cbiJdfQ==
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.967391304347826%*

 * *Differences: {"'devDependencies'": "{'eslint-import-resolver-typescript': '^3.6.1', 'jsii-diff': '^1.89.0', "*

 * *                      "'jsii-docgen': '^9.2.2', 'jsii-pacmak': '^1.89.0', 'projen': '^0.73.44'}",*

 * * "'version'": "'1.0.9'"}*

```diff
@@ -11,25 +11,25 @@
         "@types/node": "^16",
         "@typescript-eslint/eslint-plugin": "^6",
         "@typescript-eslint/parser": "^6",
         "aws-cdk-lib": "2.85.0",
         "constructs": "10.0.5",
         "eslint": "^8",
         "eslint-import-resolver-node": "^0.3.9",
-        "eslint-import-resolver-typescript": "^3.6.0",
+        "eslint-import-resolver-typescript": "^3.6.1",
         "eslint-plugin-import": "^2.28.1",
         "jest": "^29.7.0",
         "jest-junit": "^15",
         "jsii": "~5.0.0",
-        "jsii-diff": "^1.88.0",
-        "jsii-docgen": "^9.1.2",
-        "jsii-pacmak": "^1.88.0",
+        "jsii-diff": "^1.89.0",
+        "jsii-docgen": "^9.2.2",
+        "jsii-pacmak": "^1.89.0",
         "jsii-rosetta": "~5.0.0",
         "npm-check-updates": "^16",
-        "projen": "^0.73.22",
+        "projen": "^0.73.44",
         "standard-version": "^9",
         "ts-jest": "^29.1.1",
         "ts-node": "^10.9.1",
         "typescript": "^5.2.2"
     },
     "homepage": "https://rafalkrol.xyz",
     "jest": {
@@ -126,9 +126,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "1.0.8"
+    "version": "1.0.9"
 }
```

### Comparing `cdk-fsx-ontap-1.0.8/src/cdk_fsx_ontap.egg-info/PKG-INFO` & `cdk-fsx-ontap-1.0.9/src/cdk_fsx_ontap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-fsx-ontap
-Version: 1.0.8
+Version: 1.0.9
 Summary: CDK construct for Amazon FSx for Netapp ONTAP
 Home-page: https://rafalkrol.xyz
 Author: Rafal Krol<ameotoko1+github@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/rafalkrol-xyz/cdk-fsx-ontap
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

