# Comparing `tmp/seam-0.8.0.tar.gz` & `tmp/seam-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seam-0.8.0.tar", max compression
+gzip compressed data, was "seam-0.9.0.tar", max compression
```

## Comparing `seam-0.8.0.tar` & `seam-0.9.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0     1087 2024-05-22 14:09:41.498841 seam-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0    10091 2024-05-22 14:09:41.498841 seam-0.8.0/README.rst
--rw-r--r--   0        0        0      725 2024-05-22 14:09:41.502841 seam-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      397 2024-05-22 14:09:41.502841 seam-0.8.0/seam/__init__.py
--rw-r--r--   0        0        0     4076 2024-05-22 14:09:41.502841 seam-0.8.0/seam/auth.py
--rw-r--r--   0        0        0     1184 2024-05-22 14:09:41.502841 seam-0.8.0/seam/client.py
--rw-r--r--   0        0        0       72 2024-05-22 14:09:41.502841 seam-0.8.0/seam/constants.py
--rw-r--r--   0        0        0     2018 2024-05-22 14:09:41.502841 seam-0.8.0/seam/options.py
--rw-r--r--   0        0        0      623 2024-05-22 14:09:41.502841 seam-0.8.0/seam/parse_options.py
--rw-r--r--   0        0        0    11865 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/access_codes.py
--rw-r--r--   0        0        0      881 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/access_codes_simulate.py
--rw-r--r--   0        0        0     3858 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/access_codes_unmanaged.py
--rw-r--r--   0        0        0     1824 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs.py
--rw-r--r--   0        0        0     2380 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs_access_groups.py
--rw-r--r--   0        0        0      699 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs_credential_pools.py
--rw-r--r--   0        0        0     1798 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs_credential_provisioning_automations.py
--rw-r--r--   0        0        0     4879 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs_credentials.py
--rw-r--r--   0        0        0     2144 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs_entrances.py
--rw-r--r--   0        0        0     1437 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs_systems.py
--rw-r--r--   0        0        0     6362 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs_users.py
--rw-r--r--   0        0        0     3964 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/action_attempts.py
--rw-r--r--   0        0        0     5651 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/client_sessions.py
--rw-r--r--   0        0        0     3241 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/connect_webviews.py
--rw-r--r--   0        0        0     2447 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/connected_accounts.py
--rw-r--r--   0        0        0     4737 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/devices.py
--rw-r--r--   0        0        0      537 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/devices_simulate.py
--rw-r--r--   0        0        0     3281 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/devices_unmanaged.py
--rw-r--r--   0        0        0     2396 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/events.py
--rw-r--r--   0        0        0     4174 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/locks.py
--rw-r--r--   0        0        0      776 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/networks.py
--rw-r--r--   0        0        0      757 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/noise_sensors.py
--rw-r--r--   0        0        0     4317 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/noise_sensors_noise_thresholds.py
--rw-r--r--   0        0        0      614 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/noise_sensors_simulate.py
--rw-r--r--   0        0        0     1081 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/phones.py
--rw-r--r--   0        0        0     1205 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/phones_simulate.py
--rw-r--r--   0        0        0     1436 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/routes.py
--rw-r--r--   0        0        0     8846 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/thermostats.py
--rw-r--r--   0        0        0     6910 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/thermostats_climate_setting_schedules.py
--rw-r--r--   0        0        0    64963 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/types.py
--rw-r--r--   0        0        0     6558 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/user_identities.py
--rw-r--r--   0        0        0     2892 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/user_identities_enrollment_automations.py
--rw-r--r--   0        0        0      864 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/utils/deep_attr_dict.py
--rw-r--r--   0        0        0     1799 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/webhooks.py
--rw-r--r--   0        0        0     2124 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/workspaces.py
--rw-r--r--   0        0        0     2583 2024-05-22 14:09:41.502841 seam-0.8.0/seam/seam.py
--rw-r--r--   0        0        0     2545 2024-05-22 14:09:41.502841 seam-0.8.0/seam/seam_multi_workspace.py
--rw-r--r--   0        0        0     1027 2024-05-22 14:09:41.502841 seam-0.8.0/seam/token.py
--rw-r--r--   0        0        0     3487 2024-05-22 14:09:41.502841 seam-0.8.0/seam/types.py
--rw-r--r--   0        0        0    10840 1970-01-01 00:00:00.000000 seam-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-22 14:33:39.025524 seam-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0    11114 2024-05-22 14:33:39.025524 seam-0.9.0/README.rst
+-rw-r--r--   0        0        0      742 2024-05-22 14:33:39.025524 seam-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      411 2024-05-22 14:33:39.025524 seam-0.9.0/seam/__init__.py
+-rw-r--r--   0        0        0     4076 2024-05-22 14:33:39.025524 seam-0.9.0/seam/auth.py
+-rw-r--r--   0        0        0     1184 2024-05-22 14:33:39.025524 seam-0.9.0/seam/client.py
+-rw-r--r--   0        0        0       72 2024-05-22 14:33:39.025524 seam-0.9.0/seam/constants.py
+-rw-r--r--   0        0        0     2018 2024-05-22 14:33:39.025524 seam-0.9.0/seam/options.py
+-rw-r--r--   0        0        0      623 2024-05-22 14:33:39.029524 seam-0.9.0/seam/parse_options.py
+-rw-r--r--   0        0        0    11865 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/access_codes.py
+-rw-r--r--   0        0        0      881 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/access_codes_simulate.py
+-rw-r--r--   0        0        0     3858 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/access_codes_unmanaged.py
+-rw-r--r--   0        0        0     1824 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/acs.py
+-rw-r--r--   0        0        0     2380 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/acs_access_groups.py
+-rw-r--r--   0        0        0      699 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/acs_credential_pools.py
+-rw-r--r--   0        0        0     1798 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/acs_credential_provisioning_automations.py
+-rw-r--r--   0        0        0     4879 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/acs_credentials.py
+-rw-r--r--   0        0        0     2144 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/acs_entrances.py
+-rw-r--r--   0        0        0     1437 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/acs_systems.py
+-rw-r--r--   0        0        0     6362 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/acs_users.py
+-rw-r--r--   0        0        0     3964 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/action_attempts.py
+-rw-r--r--   0        0        0     5651 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/client_sessions.py
+-rw-r--r--   0        0        0     3241 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/connect_webviews.py
+-rw-r--r--   0        0        0     2447 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/connected_accounts.py
+-rw-r--r--   0        0        0     4737 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/devices.py
+-rw-r--r--   0        0        0      537 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/devices_simulate.py
+-rw-r--r--   0        0        0     3281 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/devices_unmanaged.py
+-rw-r--r--   0        0        0     2396 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/events.py
+-rw-r--r--   0        0        0     4174 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/locks.py
+-rw-r--r--   0        0        0      776 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/networks.py
+-rw-r--r--   0        0        0      757 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/noise_sensors.py
+-rw-r--r--   0        0        0     4317 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/noise_sensors_noise_thresholds.py
+-rw-r--r--   0        0        0      614 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/noise_sensors_simulate.py
+-rw-r--r--   0        0        0     1081 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/phones.py
+-rw-r--r--   0        0        0     1205 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/phones_simulate.py
+-rw-r--r--   0        0        0     1436 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/routes.py
+-rw-r--r--   0        0        0     8846 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/thermostats.py
+-rw-r--r--   0        0        0     6910 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/thermostats_climate_setting_schedules.py
+-rw-r--r--   0        0        0    64963 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/types.py
+-rw-r--r--   0        0        0     6558 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/user_identities.py
+-rw-r--r--   0        0        0     2892 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/user_identities_enrollment_automations.py
+-rw-r--r--   0        0        0      864 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/utils/deep_attr_dict.py
+-rw-r--r--   0        0        0     1799 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/webhooks.py
+-rw-r--r--   0        0        0     2124 2024-05-22 14:33:39.029524 seam-0.9.0/seam/routes/workspaces.py
+-rw-r--r--   0        0        0     2583 2024-05-22 14:33:39.029524 seam-0.9.0/seam/seam.py
+-rw-r--r--   0        0        0     2545 2024-05-22 14:33:39.029524 seam-0.9.0/seam/seam_multi_workspace.py
+-rw-r--r--   0        0        0      340 2024-05-22 14:33:39.029524 seam-0.9.0/seam/seam_webhook.py
+-rw-r--r--   0        0        0     1027 2024-05-22 14:33:39.029524 seam-0.9.0/seam/token.py
+-rw-r--r--   0        0        0     3487 2024-05-22 14:33:39.029524 seam-0.9.0/seam/types.py
+-rw-r--r--   0        0        0    11901 1970-01-01 00:00:00.000000 seam-0.9.0/PKG-INFO
```

### Comparing `seam-0.8.0/LICENSE.txt` & `seam-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/README.rst` & `seam-0.9.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -205,14 +205,53 @@
 
   # Use the factory method
   seam = SeamMultiWorkspace.from_personal_access_token("your-personal-access-token")
 
   # List workspaces authorized for this Personal Access Token
   workspaces = seam.workspaces.list()
 
+Webhooks
+~~~~~~~~
+
+The Seam API implements webhooks using `Svix <https://www.svix.com>`_. This SDK exports a thin wrapper ``SeamWebhook`` around the svix package. Use it to parse and validate Seam webhook events.
+
+Refer to the `Svix docs on Consuming Webhooks <https://docs.svix.com/receiving/introduction>`_ for an in-depth guide on best-practices for handling webhooks in your application.
+
+.. code-block:: python
+
+  import os
+
+  from flask import Flask, request
+  from seam import SeamWebhook
+
+  app = Flask(__name__)
+
+  webhook = SeamWebhook(os.getenv('SEAM_WEBHOOK_SECRET'))
+
+  @app.route('/webhook', methods=['POST'])
+  def handle_webhook():
+      try:
+          data = webhook.verify(request.get_data(), request.headers)
+      except Exception:
+          return 'Bad Request', 400
+
+      try:
+          store_event(data)
+      except Exception:
+            return 'Internal Server Error', 500
+
+      return '', 204
+
+  def store_event(data):
+      print(data)
+
+  if __name__ == '__main__':
+      app.run(port=8080)
+
+
 Advanced Usage
 ~~~~~~~~~~~~~~
 
 Setting the endpoint
 ^^^^^^^^^^^^^^^^^^^^
 
 Some contexts may need to override the API endpoint,
```

### Comparing `seam-0.8.0/pyproject.toml` & `seam-0.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "seam"
-version = "0.8.0"
+version = "0.9.0"
 description = "SDK for the Seam API written in Python."
 authors = ["Seam Labs, Inc. <engineering@getseam.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/seamapi/python-next"
 repository = "https://github.com/seamapi/python-next"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 dataclasses-json = "^0.6.4"
 niquests = "^3.6.4"
+svix = "^1.24.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 pylint = "^3.1.0"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 pytest-runner = "^6.0.0"
```

### Comparing `seam-0.8.0/seam/auth.py` & `seam-0.9.0/seam/auth.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/client.py` & `seam-0.9.0/seam/client.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/options.py` & `seam-0.9.0/seam/options.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/parse_options.py` & `seam-0.9.0/seam/parse_options.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/access_codes.py` & `seam-0.9.0/seam/routes/access_codes.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/access_codes_simulate.py` & `seam-0.9.0/seam/routes/access_codes_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/access_codes_unmanaged.py` & `seam-0.9.0/seam/routes/access_codes_unmanaged.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/acs.py` & `seam-0.9.0/seam/routes/acs.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/acs_access_groups.py` & `seam-0.9.0/seam/routes/acs_access_groups.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/acs_credential_pools.py` & `seam-0.9.0/seam/routes/acs_credential_pools.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/acs_credential_provisioning_automations.py` & `seam-0.9.0/seam/routes/acs_credential_provisioning_automations.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/acs_credentials.py` & `seam-0.9.0/seam/routes/acs_credentials.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/acs_entrances.py` & `seam-0.9.0/seam/routes/acs_entrances.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/acs_systems.py` & `seam-0.9.0/seam/routes/acs_systems.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/acs_users.py` & `seam-0.9.0/seam/routes/acs_users.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/action_attempts.py` & `seam-0.9.0/seam/routes/action_attempts.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/client_sessions.py` & `seam-0.9.0/seam/routes/client_sessions.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/connect_webviews.py` & `seam-0.9.0/seam/routes/connect_webviews.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/connected_accounts.py` & `seam-0.9.0/seam/routes/connected_accounts.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/devices.py` & `seam-0.9.0/seam/routes/devices.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/devices_simulate.py` & `seam-0.9.0/seam/routes/devices_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/devices_unmanaged.py` & `seam-0.9.0/seam/routes/devices_unmanaged.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/events.py` & `seam-0.9.0/seam/routes/events.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/locks.py` & `seam-0.9.0/seam/routes/locks.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/networks.py` & `seam-0.9.0/seam/routes/networks.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/noise_sensors.py` & `seam-0.9.0/seam/routes/noise_sensors.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/noise_sensors_noise_thresholds.py` & `seam-0.9.0/seam/routes/noise_sensors_noise_thresholds.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/noise_sensors_simulate.py` & `seam-0.9.0/seam/routes/noise_sensors_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/phones.py` & `seam-0.9.0/seam/routes/phones.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/phones_simulate.py` & `seam-0.9.0/seam/routes/phones_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/routes.py` & `seam-0.9.0/seam/routes/routes.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/thermostats.py` & `seam-0.9.0/seam/routes/thermostats.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/thermostats_climate_setting_schedules.py` & `seam-0.9.0/seam/routes/thermostats_climate_setting_schedules.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/types.py` & `seam-0.9.0/seam/routes/types.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/user_identities.py` & `seam-0.9.0/seam/routes/user_identities.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/user_identities_enrollment_automations.py` & `seam-0.9.0/seam/routes/user_identities_enrollment_automations.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/utils/deep_attr_dict.py` & `seam-0.9.0/seam/routes/utils/deep_attr_dict.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/webhooks.py` & `seam-0.9.0/seam/routes/webhooks.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/routes/workspaces.py` & `seam-0.9.0/seam/routes/workspaces.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/seam.py` & `seam-0.9.0/seam/seam.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/seam_multi_workspace.py` & `seam-0.9.0/seam/seam_multi_workspace.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/token.py` & `seam-0.9.0/seam/token.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/seam/types.py` & `seam-0.9.0/seam/types.py`

 * *Files identical despite different names*

### Comparing `seam-0.8.0/PKG-INFO` & `seam-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: seam
-Version: 0.8.0
+Version: 0.9.0
 Summary: SDK for the Seam API written in Python.
 Home-page: https://github.com/seamapi/python-next
 License: MIT
 Author: Seam Labs, Inc.
 Author-email: engineering@getseam.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
 Requires-Dist: niquests (>=3.6.4,<4.0.0)
+Requires-Dist: svix (>=1.24.0,<2.0.0)
 Project-URL: Repository, https://github.com/seamapi/python-next
 Description-Content-Type: text/x-rst
 
 Seam Python SDK
 ===============
 
 |PyPI| |GitHub Actions|
@@ -225,14 +226,53 @@
 
   # Use the factory method
   seam = SeamMultiWorkspace.from_personal_access_token("your-personal-access-token")
 
   # List workspaces authorized for this Personal Access Token
   workspaces = seam.workspaces.list()
 
+Webhooks
+~~~~~~~~
+
+The Seam API implements webhooks using `Svix <https://www.svix.com>`_. This SDK exports a thin wrapper ``SeamWebhook`` around the svix package. Use it to parse and validate Seam webhook events.
+
+Refer to the `Svix docs on Consuming Webhooks <https://docs.svix.com/receiving/introduction>`_ for an in-depth guide on best-practices for handling webhooks in your application.
+
+.. code-block:: python
+
+  import os
+
+  from flask import Flask, request
+  from seam import SeamWebhook
+
+  app = Flask(__name__)
+
+  webhook = SeamWebhook(os.getenv('SEAM_WEBHOOK_SECRET'))
+
+  @app.route('/webhook', methods=['POST'])
+  def handle_webhook():
+      try:
+          data = webhook.verify(request.get_data(), request.headers)
+      except Exception:
+          return 'Bad Request', 400
+
+      try:
+          store_event(data)
+      except Exception:
+            return 'Internal Server Error', 500
+
+      return '', 204
+
+  def store_event(data):
+      print(data)
+
+  if __name__ == '__main__':
+      app.run(port=8080)
+
+
 Advanced Usage
 ~~~~~~~~~~~~~~
 
 Setting the endpoint
 ^^^^^^^^^^^^^^^^^^^^
 
 Some contexts may need to override the API endpoint,
```

