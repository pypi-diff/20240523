# Comparing `tmp/py_consul-1.5.0.tar.gz` & `tmp/py_consul-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_consul-1.5.0.tar", last modified: Wed May 15 13:31:14 2024, max compression
+gzip compressed data, was "py_consul-1.5.1.tar", last modified: Thu May 23 13:59:09 2024, max compression
```

## Comparing `py_consul-1.5.0.tar` & `py_consul-1.5.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:14.813481 py_consul-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-15 13:31:03.000000 py_consul-1.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-15 13:31:03.000000 py_consul-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 13:31:03.000000 py_consul-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-15 13:31:14.813481 py_consul-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-15 13:31:03.000000 py_consul-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:14.809481 py_consul-1.5.0/consul/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/aio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:14.809481 py_consul-1.5.0/consul/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:14.809481 py_consul-1.5.0/consul/api/acl/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/acl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/acl/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/acl/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    15942 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    14039 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/kv.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7580 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/api/txn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-15 13:31:03.000000 py_consul-1.5.0/consul/std.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:14.809481 py_consul-1.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:03.000000 py_consul-1.5.0/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-05-15 13:31:03.000000 py_consul-1.5.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:14.813481 py_consul-1.5.0/py_consul.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-15 13:31:14.000000 py_consul-1.5.0/py_consul.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-15 13:31:14.000000 py_consul-1.5.0/py_consul.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:31:14.000000 py_consul-1.5.0/py_consul.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 13:31:14.000000 py_consul-1.5.0/py_consul.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-15 13:31:14.000000 py_consul-1.5.0/py_consul.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-15 13:31:03.000000 py_consul-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 13:31:03.000000 py_consul-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 13:31:14.813481 py_consul-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-15 13:31:03.000000 py_consul-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:31:14.813481 py_consul-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-15 13:31:04.000000 py_consul-1.5.0/tests/test_aio.py
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-05-15 13:31:04.000000 py_consul-1.5.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-15 13:31:04.000000 py_consul-1.5.0/tests/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-15 13:31:04.000000 py_consul-1.5.0/tests/test_std.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-15 13:31:04.000000 py_consul-1.5.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-15 13:31:03.000000 py_consul-1.5.0/tests-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:59:09.672180 py_consul-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-23 13:58:55.000000 py_consul-1.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-23 13:58:55.000000 py_consul-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-23 13:58:55.000000 py_consul-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-23 13:59:09.672180 py_consul-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-23 13:58:55.000000 py_consul-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:59:09.664179 py_consul-1.5.1/consul/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/aio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:59:09.668180 py_consul-1.5.1/consul/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:59:09.668180 py_consul-1.5.1/consul/api/acl/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/acl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/acl/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/acl/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15942 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14039 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/kv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7580 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/api/txn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-23 13:58:55.000000 py_consul-1.5.1/consul/std.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:59:09.668180 py_consul-1.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:58:55.000000 py_consul-1.5.1/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-05-23 13:58:55.000000 py_consul-1.5.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:59:09.672180 py_consul-1.5.1/py_consul.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-23 13:59:09.000000 py_consul-1.5.1/py_consul.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-23 13:59:09.000000 py_consul-1.5.1/py_consul.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:59:09.000000 py_consul-1.5.1/py_consul.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 13:59:09.000000 py_consul-1.5.1/py_consul.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-23 13:59:09.000000 py_consul-1.5.1/py_consul.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-23 13:58:55.000000 py_consul-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 13:58:55.000000 py_consul-1.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 13:59:09.672180 py_consul-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-23 13:58:55.000000 py_consul-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:59:09.672180 py_consul-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-23 13:58:56.000000 py_consul-1.5.1/tests/test_aio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-05-23 13:58:56.000000 py_consul-1.5.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-23 13:58:56.000000 py_consul-1.5.1/tests/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-23 13:58:56.000000 py_consul-1.5.1/tests/test_std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-23 13:58:56.000000 py_consul-1.5.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-23 13:58:55.000000 py_consul-1.5.1/tests-requirements.txt
```

### Comparing `py_consul-1.5.0/CHANGELOG.md` & `py_consul-1.5.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Change log
 
+## 1.5.1
+
+- **feature:** Implement creation of policies.
+- **feature:** Integrate policy addition during token creation.
+
 ## 1.5.0
 
 - **[Breaking]** ACL endpoint change, consul.acl is now consul.acl.token
 - **feature:** add consul.acl.policy.list and acl.policy.read
 
 ## 1.4.1
```

### Comparing `py_consul-1.5.0/LICENSE` & `py_consul-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/PKG-INFO` & `py_consul-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-consul
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python client for Consul (http://www.consul.io/)
 Home-page: https://github.com/criteo-forks/py-consul
 Author: Criteo
 Author-email: github@criteo.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -85,14 +85,19 @@
 
 - To add tests for your new features, if applicable
 - To add docstrings for new API features you may add
 
 
 # Change log
 
+## 1.5.1
+
+- **feature:** Implement creation of policies.
+- **feature:** Integrate policy addition during token creation.
+
 ## 1.5.0
 
 - **[Breaking]** ACL endpoint change, consul.acl is now consul.acl.token
 - **feature:** add consul.acl.policy.list and acl.policy.read
 
 ## 1.4.1
```

### Comparing `py_consul-1.5.0/README.md` & `py_consul-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/aio.py` & `py_consul-1.5.1/consul/aio.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/api/acl/token.py` & `py_consul-1.5.1/consul/api/acl/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,36 +63,40 @@
         return self.agent.http.put(
             CB.json(),
             f"/v1/acl/token/{accessor_id}/clone",
             params=params,
             data=json.dumps(json_data),
         )
 
-    def create(self, token=None, accessor_id=None, secret_id=None, description=""):
+    def create(self, token=None, accessor_id=None, secret_id=None, policies_id=None, description=""):
         """
         Create a token (optionally identified by *secret_id* and *accessor_id*).
         This is a privileged endpoint, and requires a token with acl:write.
         :param token: token with acl:write capability
         :param accessor_id: The accessor ID of the token to create
         :param secret_id: The secret ID of the token to create
         :param description: Optional new token description
+        :param policies: Optional list of policies id
         :return: The cloned token information
         """
         params = []
         token = token or self.agent.token
         if token:
             params.append(("token", token))
 
         json_data = {}
         if accessor_id:
             json_data["AccessorID"] = accessor_id
         if secret_id:
             json_data["SecretID"] = secret_id
         if description:
             json_data["Description"] = description
+        if policies_id:
+            json_data["Policies"] = [{"ID": policy} for policy in policies_id]
+
         return self.agent.http.put(
             CB.json(),
             "/v1/acl/token",
             params=params,
             data=json.dumps(json_data),
         )
```

### Comparing `py_consul-1.5.0/consul/api/agent.py` & `py_consul-1.5.1/consul/api/agent.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/api/catalog.py` & `py_consul-1.5.1/consul/api/catalog.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/api/connect.py` & `py_consul-1.5.1/consul/api/connect.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/api/coordinates.py` & `py_consul-1.5.1/consul/api/coordinates.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/api/event.py` & `py_consul-1.5.1/consul/api/event.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/api/health.py` & `py_consul-1.5.1/consul/api/health.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/api/kv.py` & `py_consul-1.5.1/consul/api/kv.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/api/query.py` & `py_consul-1.5.1/consul/api/query.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/api/session.py` & `py_consul-1.5.1/consul/api/session.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/api/status.py` & `py_consul-1.5.1/consul/api/status.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/api/txn.py` & `py_consul-1.5.1/consul/api/txn.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/base.py` & `py_consul-1.5.1/consul/base.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/callback.py` & `py_consul-1.5.1/consul/callback.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/check.py` & `py_consul-1.5.1/consul/check.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/consul/std.py` & `py_consul-1.5.1/consul/std.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/docs/conf.py` & `py_consul-1.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/py_consul.egg-info/PKG-INFO` & `py_consul-1.5.1/py_consul.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-consul
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python client for Consul (http://www.consul.io/)
 Home-page: https://github.com/criteo-forks/py-consul
 Author: Criteo
 Author-email: github@criteo.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -85,14 +85,19 @@
 
 - To add tests for your new features, if applicable
 - To add docstrings for new API features you may add
 
 
 # Change log
 
+## 1.5.1
+
+- **feature:** Implement creation of policies.
+- **feature:** Integrate policy addition during token creation.
+
 ## 1.5.0
 
 - **[Breaking]** ACL endpoint change, consul.acl is now consul.acl.token
 - **feature:** add consul.acl.policy.list and acl.policy.read
 
 ## 1.4.1
```

### Comparing `py_consul-1.5.0/py_consul.egg-info/SOURCES.txt` & `py_consul-1.5.1/py_consul.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/pyproject.toml` & `py_consul-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/setup.py` & `py_consul-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/tests/test_aio.py` & `py_consul-1.5.1/tests/test_aio.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/tests/test_base.py` & `py_consul-1.5.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/tests/test_callback.py` & `py_consul-1.5.1/tests/test_callback.py`

 * *Files identical despite different names*

### Comparing `py_consul-1.5.0/tests/test_utils.py` & `py_consul-1.5.1/tests/test_utils.py`

 * *Files identical despite different names*

