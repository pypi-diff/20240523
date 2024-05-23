# Comparing `tmp/pulumi_twingate-3.0.3.dev0.tar.gz` & `tmp/pulumi_twingate-3.0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_twingate-3.0.3.dev0.tar", last modified: Thu May  2 20:16:17 2024, max compression
+gzip compressed data, was "pulumi_twingate-3.0.4.dev0.tar", last modified: Thu May 23 14:36:39 2024, max compression
```

## Comparing `pulumi_twingate-3.0.3.dev0.tar` & `pulumi_twingate-3.0.4.dev0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:17.732144 pulumi_twingate-3.0.3.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-02 20:16:17.732144 pulumi_twingate-3.0.3.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:17.732144 pulumi_twingate-3.0.3.dev0/pulumi_twingate/
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:17.732144 pulumi_twingate-3.0.3.dev0/pulumi_twingate/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10292 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_remote_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_remote_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_security_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_security_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    21219 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    27880 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11643 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12361 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_connector_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    14760 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_remote_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    34418 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_service_account_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    17041 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:16:17.732144 pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:16:17.732144 pulumi_twingate-3.0.3.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-02 20:16:17.000000 pulumi_twingate-3.0.3.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:39.944333 pulumi_twingate-3.0.4.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-23 14:36:39.944333 pulumi_twingate-3.0.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:39.944333 pulumi_twingate-3.0.4.dev0/pulumi_twingate/
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:39.944333 pulumi_twingate-3.0.4.dev0/pulumi_twingate/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10292 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_remote_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_remote_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_security_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_security_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21219 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27880 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11643 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12361 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_connector_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13091 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_remote_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32742 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14836 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_service_account_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17041 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:39.944333 pulumi_twingate-3.0.4.dev0/pulumi_twingate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/pulumi_twingate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:36:39.944333 pulumi_twingate-3.0.4.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-23 14:36:39.000000 pulumi_twingate-3.0.4.dev0/setup.py
```

### Comparing `pulumi_twingate-3.0.3.dev0/PKG-INFO` & `pulumi_twingate-3.0.4.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_twingate
-Version: 3.0.3.dev0
+Version: 3.0.4.dev0
 Summary: A Pulumi package for creating and managing Twingate cloud resources.
 Home-page: https://www.twingate.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Twingate/pulumi-twingate
 Keywords: pulumi twingate category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_twingate-3.0.3.dev0/README.md` & `pulumi_twingate-3.0.4.dev0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/__init__.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/_inputs.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/_utilities.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/config/vars.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_connector.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_connectors.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_connectors.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_group.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_groups.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_remote_network.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_remote_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_remote_networks.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_remote_networks.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_resource.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_resources.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_resources.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_security_policies.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_security_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_security_policy.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_service_accounts.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_service_accounts.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_user.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/get_twingate_users.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/get_twingate_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/outputs.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/provider.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_connector.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_connector_tokens.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_connector_tokens.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_group.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_group.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,16 +16,14 @@
     def __init__(__self__, *,
                  is_authoritative: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  security_policy_id: Optional[pulumi.Input[str]] = None,
                  user_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a TwingateGroup resource.
-        :param pulumi.Input[bool] is_authoritative: Determines whether User assignments to this Group will override any existing assignments. Default is `true`. If set to
-               `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[str] name: The name of the group
         :param pulumi.Input[str] security_policy_id: Defines which Security Policy applies to this Group. The Security Policy ID can be obtained from the `get_twingate_security_policy` and `get_twingate_security_policies` data sources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] user_ids: List of User IDs that have permission to access the Group.
         """
         if is_authoritative is not None:
             pulumi.set(__self__, "is_authoritative", is_authoritative)
         if name is not None:
@@ -34,18 +32,14 @@
             pulumi.set(__self__, "security_policy_id", security_policy_id)
         if user_ids is not None:
             pulumi.set(__self__, "user_ids", user_ids)
 
     @property
     @pulumi.getter(name="isAuthoritative")
     def is_authoritative(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Determines whether User assignments to this Group will override any existing assignments. Default is `true`. If set to
-        `false`, assignments made outside of Terraform will be ignored.
-        """
         return pulumi.get(self, "is_authoritative")
 
     @is_authoritative.setter
     def is_authoritative(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_authoritative", value)
 
     @property
@@ -90,16 +84,14 @@
     def __init__(__self__, *,
                  is_authoritative: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  security_policy_id: Optional[pulumi.Input[str]] = None,
                  user_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering TwingateGroup resources.
-        :param pulumi.Input[bool] is_authoritative: Determines whether User assignments to this Group will override any existing assignments. Default is `true`. If set to
-               `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[str] name: The name of the group
         :param pulumi.Input[str] security_policy_id: Defines which Security Policy applies to this Group. The Security Policy ID can be obtained from the `get_twingate_security_policy` and `get_twingate_security_policies` data sources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] user_ids: List of User IDs that have permission to access the Group.
         """
         if is_authoritative is not None:
             pulumi.set(__self__, "is_authoritative", is_authoritative)
         if name is not None:
@@ -108,18 +100,14 @@
             pulumi.set(__self__, "security_policy_id", security_policy_id)
         if user_ids is not None:
             pulumi.set(__self__, "user_ids", user_ids)
 
     @property
     @pulumi.getter(name="isAuthoritative")
     def is_authoritative(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Determines whether User assignments to this Group will override any existing assignments. Default is `true`. If set to
-        `false`, assignments made outside of Terraform will be ignored.
-        """
         return pulumi.get(self, "is_authoritative")
 
     @is_authoritative.setter
     def is_authoritative(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_authoritative", value)
 
     @property
@@ -185,16 +173,14 @@
 
         ```sh
         $ pulumi import twingate:index/twingateGroup:TwingateGroup aws R3JvdXA6MzQ4OTE=
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] is_authoritative: Determines whether User assignments to this Group will override any existing assignments. Default is `true`. If set to
-               `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[str] name: The name of the group
         :param pulumi.Input[str] security_policy_id: Defines which Security Policy applies to this Group. The Security Policy ID can be obtained from the `get_twingate_security_policy` and `get_twingate_security_policies` data sources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] user_ids: List of User IDs that have permission to access the Group.
         """
         ...
     @overload
     def __init__(__self__,
@@ -268,16 +254,14 @@
         """
         Get an existing TwingateGroup resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] is_authoritative: Determines whether User assignments to this Group will override any existing assignments. Default is `true`. If set to
-               `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[str] name: The name of the group
         :param pulumi.Input[str] security_policy_id: Defines which Security Policy applies to this Group. The Security Policy ID can be obtained from the `get_twingate_security_policy` and `get_twingate_security_policies` data sources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] user_ids: List of User IDs that have permission to access the Group.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _TwingateGroupState.__new__(_TwingateGroupState)
@@ -287,18 +271,14 @@
         __props__.__dict__["security_policy_id"] = security_policy_id
         __props__.__dict__["user_ids"] = user_ids
         return TwingateGroup(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="isAuthoritative")
     def is_authoritative(self) -> pulumi.Output[bool]:
-        """
-        Determines whether User assignments to this Group will override any existing assignments. Default is `true`. If set to
-        `false`, assignments made outside of Terraform will be ignored.
-        """
         return pulumi.get(self, "is_authoritative")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         The name of the group
```

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_remote_network.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_remote_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_resource.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,14 @@
         The set of arguments for constructing a TwingateResource resource.
         :param pulumi.Input[str] address: The Resource's IP/CIDR or FQDN/DNS zone
         :param pulumi.Input[str] remote_network_id: Remote Network ID where the Resource lives
         :param pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessGroupArgs']]] access_groups: Restrict access to certain group
         :param pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessServiceArgs']]] access_services: Restrict access to certain service account
         :param pulumi.Input[str] alias: Set a DNS alias address for the Resource. Must be a DNS-valid name string.
         :param pulumi.Input[bool] is_active: Set the resource as active or inactive. Default is `true`.
-        :param pulumi.Input[bool] is_authoritative: Determines whether assignments in the access block will override any existing assignments. Default is `true`. If set to
-               `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[bool] is_browser_shortcut_enabled: Controls whether an "Open in Browser" shortcut will be shown for this Resource in the Twingate Client. Default is `false`.
         :param pulumi.Input[bool] is_visible: Controls whether this Resource will be visible in the main Resource list in the Twingate Client. Default is `true`.
         :param pulumi.Input[str] name: The name of the Resource
         :param pulumi.Input['TwingateResourceProtocolsArgs'] protocols: Restrict access to certain protocols and ports. By default or when this argument is not defined, there is no restriction, and all protocols and ports are allowed.
         :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
         """
         pulumi.set(__self__, "address", address)
@@ -138,18 +136,14 @@
     @is_active.setter
     def is_active(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_active", value)
 
     @property
     @pulumi.getter(name="isAuthoritative")
     def is_authoritative(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Determines whether assignments in the access block will override any existing assignments. Default is `true`. If set to
-        `false`, assignments made outside of Terraform will be ignored.
-        """
         return pulumi.get(self, "is_authoritative")
 
     @is_authoritative.setter
     def is_authoritative(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_authoritative", value)
 
     @property
@@ -231,16 +225,14 @@
         """
         Input properties used for looking up and filtering TwingateResource resources.
         :param pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessGroupArgs']]] access_groups: Restrict access to certain group
         :param pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessServiceArgs']]] access_services: Restrict access to certain service account
         :param pulumi.Input[str] address: The Resource's IP/CIDR or FQDN/DNS zone
         :param pulumi.Input[str] alias: Set a DNS alias address for the Resource. Must be a DNS-valid name string.
         :param pulumi.Input[bool] is_active: Set the resource as active or inactive. Default is `true`.
-        :param pulumi.Input[bool] is_authoritative: Determines whether assignments in the access block will override any existing assignments. Default is `true`. If set to
-               `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[bool] is_browser_shortcut_enabled: Controls whether an "Open in Browser" shortcut will be shown for this Resource in the Twingate Client. Default is `false`.
         :param pulumi.Input[bool] is_visible: Controls whether this Resource will be visible in the main Resource list in the Twingate Client. Default is `true`.
         :param pulumi.Input[str] name: The name of the Resource
         :param pulumi.Input['TwingateResourceProtocolsArgs'] protocols: Restrict access to certain protocols and ports. By default or when this argument is not defined, there is no restriction, and all protocols and ports are allowed.
         :param pulumi.Input[str] remote_network_id: Remote Network ID where the Resource lives
         :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
         """
@@ -328,18 +320,14 @@
     @is_active.setter
     def is_active(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_active", value)
 
     @property
     @pulumi.getter(name="isAuthoritative")
     def is_authoritative(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Determines whether assignments in the access block will override any existing assignments. Default is `true`. If set to
-        `false`, assignments made outside of Terraform will be ignored.
-        """
         return pulumi.get(self, "is_authoritative")
 
     @is_authoritative.setter
     def is_authoritative(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_authoritative", value)
 
     @property
@@ -445,16 +433,14 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TwingateResourceAccessGroupArgs']]]] access_groups: Restrict access to certain group
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TwingateResourceAccessServiceArgs']]]] access_services: Restrict access to certain service account
         :param pulumi.Input[str] address: The Resource's IP/CIDR or FQDN/DNS zone
         :param pulumi.Input[str] alias: Set a DNS alias address for the Resource. Must be a DNS-valid name string.
         :param pulumi.Input[bool] is_active: Set the resource as active or inactive. Default is `true`.
-        :param pulumi.Input[bool] is_authoritative: Determines whether assignments in the access block will override any existing assignments. Default is `true`. If set to
-               `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[bool] is_browser_shortcut_enabled: Controls whether an "Open in Browser" shortcut will be shown for this Resource in the Twingate Client. Default is `false`.
         :param pulumi.Input[bool] is_visible: Controls whether this Resource will be visible in the main Resource list in the Twingate Client. Default is `true`.
         :param pulumi.Input[str] name: The name of the Resource
         :param pulumi.Input[pulumi.InputType['TwingateResourceProtocolsArgs']] protocols: Restrict access to certain protocols and ports. By default or when this argument is not defined, there is no restriction, and all protocols and ports are allowed.
         :param pulumi.Input[str] remote_network_id: Remote Network ID where the Resource lives
         :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
         """
@@ -555,16 +541,14 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TwingateResourceAccessGroupArgs']]]] access_groups: Restrict access to certain group
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TwingateResourceAccessServiceArgs']]]] access_services: Restrict access to certain service account
         :param pulumi.Input[str] address: The Resource's IP/CIDR or FQDN/DNS zone
         :param pulumi.Input[str] alias: Set a DNS alias address for the Resource. Must be a DNS-valid name string.
         :param pulumi.Input[bool] is_active: Set the resource as active or inactive. Default is `true`.
-        :param pulumi.Input[bool] is_authoritative: Determines whether assignments in the access block will override any existing assignments. Default is `true`. If set to
-               `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[bool] is_browser_shortcut_enabled: Controls whether an "Open in Browser" shortcut will be shown for this Resource in the Twingate Client. Default is `false`.
         :param pulumi.Input[bool] is_visible: Controls whether this Resource will be visible in the main Resource list in the Twingate Client. Default is `true`.
         :param pulumi.Input[str] name: The name of the Resource
         :param pulumi.Input[pulumi.InputType['TwingateResourceProtocolsArgs']] protocols: Restrict access to certain protocols and ports. By default or when this argument is not defined, there is no restriction, and all protocols and ports are allowed.
         :param pulumi.Input[str] remote_network_id: Remote Network ID where the Resource lives
         :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
         """
@@ -625,18 +609,14 @@
         Set the resource as active or inactive. Default is `true`.
         """
         return pulumi.get(self, "is_active")
 
     @property
     @pulumi.getter(name="isAuthoritative")
     def is_authoritative(self) -> pulumi.Output[bool]:
-        """
-        Determines whether assignments in the access block will override any existing assignments. Default is `true`. If set to
-        `false`, assignments made outside of Terraform will be ignored.
-        """
         return pulumi.get(self, "is_authoritative")
 
     @property
     @pulumi.getter(name="isBrowserShortcutEnabled")
     def is_browser_shortcut_enabled(self) -> pulumi.Output[bool]:
         """
         Controls whether an "Open in Browser" shortcut will be shown for this Resource in the Twingate Client. Default is `false`.
```

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_service_account.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_service_account_key.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_service_account_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,14 @@
                  is_active: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  service_account_id: Optional[pulumi.Input[str]] = None,
                  token: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering TwingateServiceAccountKey resources.
         :param pulumi.Input[int] expiration_time: Specifies how many days until a Service Account Key expires. This should be an integer between 0 and 365 representing the number of days until the Service Account Key will expire. Defaults to 0, meaning the key will never expire.
-        :param pulumi.Input[bool] is_active: If the value of this attribute changes to false, Terraform will destroy and recreate the resource.
         :param pulumi.Input[str] name: The name of the Service Key
         :param pulumi.Input[str] service_account_id: The id of the Service Account
         :param pulumi.Input[str] token: Autogenerated Service Key token. Used to configure a Twingate Client running in headless mode.
         """
         if expiration_time is not None:
             pulumi.set(__self__, "expiration_time", expiration_time)
         if is_active is not None:
@@ -104,17 +103,14 @@
     @expiration_time.setter
     def expiration_time(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "expiration_time", value)
 
     @property
     @pulumi.getter(name="isActive")
     def is_active(self) -> Optional[pulumi.Input[bool]]:
-        """
-        If the value of this attribute changes to false, Terraform will destroy and recreate the resource.
-        """
         return pulumi.get(self, "is_active")
 
     @is_active.setter
     def is_active(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_active", value)
 
     @property
@@ -266,15 +262,14 @@
         Get an existing TwingateServiceAccountKey resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] expiration_time: Specifies how many days until a Service Account Key expires. This should be an integer between 0 and 365 representing the number of days until the Service Account Key will expire. Defaults to 0, meaning the key will never expire.
-        :param pulumi.Input[bool] is_active: If the value of this attribute changes to false, Terraform will destroy and recreate the resource.
         :param pulumi.Input[str] name: The name of the Service Key
         :param pulumi.Input[str] service_account_id: The id of the Service Account
         :param pulumi.Input[str] token: Autogenerated Service Key token. Used to configure a Twingate Client running in headless mode.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _TwingateServiceAccountKeyState.__new__(_TwingateServiceAccountKeyState)
@@ -293,17 +288,14 @@
         Specifies how many days until a Service Account Key expires. This should be an integer between 0 and 365 representing the number of days until the Service Account Key will expire. Defaults to 0, meaning the key will never expire.
         """
         return pulumi.get(self, "expiration_time")
 
     @property
     @pulumi.getter(name="isActive")
     def is_active(self) -> pulumi.Output[bool]:
-        """
-        If the value of this attribute changes to false, Terraform will destroy and recreate the resource.
-        """
         return pulumi.get(self, "is_active")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         The name of the Service Key
```

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate/twingate_user.py` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate/twingate_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/PKG-INFO` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-twingate
-Version: 3.0.3.dev0
+Version: 3.0.4.dev0
 Summary: A Pulumi package for creating and managing Twingate cloud resources.
 Home-page: https://www.twingate.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Twingate/pulumi-twingate
 Keywords: pulumi twingate category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_twingate-3.0.3.dev0/pulumi_twingate.egg-info/SOURCES.txt` & `pulumi_twingate-3.0.4.dev0/pulumi_twingate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.3.dev0/setup.py` & `pulumi_twingate-3.0.4.dev0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.0.3dev0"
+VERSION = "3.0.4dev0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "twingate Pulumi Package - Development Version"
```

