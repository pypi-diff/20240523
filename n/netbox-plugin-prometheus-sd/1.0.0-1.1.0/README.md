# Comparing `tmp/netbox_plugin_prometheus_sd-1.0.0.tar.gz` & `tmp/netbox_plugin_prometheus_sd-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_plugin_prometheus_sd-1.0.0.tar", max compression
+gzip compressed data, was "netbox_plugin_prometheus_sd-1.1.0.tar", max compression
```

## Comparing `netbox_plugin_prometheus_sd-1.0.0.tar` & `netbox_plugin_prometheus_sd-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2024-05-07 22:22:07.539324 netbox_plugin_prometheus_sd-1.0.0/LICENSE
--rw-r--r--   0        0        0     5730 2024-05-07 22:22:07.539324 netbox_plugin_prometheus_sd-1.0.0/README.md
--rw-r--r--   0        0        0      488 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/__init__.py
--rw-r--r--   0        0        0     7032 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/serializers.py
--rw-r--r--   0        0        0      381 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/urls.py
--rw-r--r--   0        0        0     5992 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/utils.py
--rw-r--r--   0        0        0     3360 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/views.py
--rw-r--r--   0        0        0     2031 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/filtersets.py
--rw-r--r--   0        0        0       50 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/__init__.py
--rw-r--r--   0        0        0     3535 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/test_api.py
--rw-r--r--   0        0        0     1304 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/test_filtersets.py
--rwxr-xr-x   0        0        0    15114 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/test_serializers.py
--rw-r--r--   0        0        0     7157 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/utils.py
--rw-r--r--   0        0        0      616 2024-05-07 22:22:18.271447 netbox_plugin_prometheus_sd-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6386 1970-01-01 00:00:00.000000 netbox_plugin_prometheus_sd-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-22 21:25:02.135733 netbox_plugin_prometheus_sd-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5793 2024-05-22 21:25:02.135733 netbox_plugin_prometheus_sd-1.1.0/README.md
+-rw-r--r--   0        0        0      605 2024-05-23 08:44:01.533118 netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 21:25:02.135733 netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/api/__init__.py
+-rw-r--r--   0        0        0     7032 2024-05-22 21:25:02.136733 netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/api/serializers.py
+-rw-r--r--   0        0        0      381 2024-05-22 21:25:02.136733 netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/api/urls.py
+-rw-r--r--   0        0        0     5992 2024-05-22 21:25:02.136733 netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/api/utils.py
+-rw-r--r--   0        0        0     3360 2024-05-22 21:25:02.136733 netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/api/views.py
+-rw-r--r--   0        0        0     2306 2024-05-23 08:44:01.533118 netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/filtersets.py
+-rw-r--r--   0        0        0       50 2024-05-22 21:25:02.136733 netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/tests/__init__.py
+-rw-r--r--   0        0        0     3701 2024-05-23 08:44:01.534118 netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/tests/test_api.py
+-rw-r--r--   0        0        0     1304 2024-05-22 21:25:02.136733 netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/tests/test_filtersets.py
+-rwxr-xr-x   0        0        0    15114 2024-05-22 21:25:02.136733 netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/tests/test_serializers.py
+-rw-r--r--   0        0        0     7157 2024-05-22 21:25:02.136733 netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/tests/utils.py
+-rw-r--r--   0        0        0      617 2024-05-23 10:13:42.968080 netbox_plugin_prometheus_sd-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6449 1970-01-01 00:00:00.000000 netbox_plugin_prometheus_sd-1.1.0/PKG-INFO
```

### Comparing `netbox_plugin_prometheus_sd-1.0.0/LICENSE` & `netbox_plugin_prometheus_sd-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-1.0.0/README.md` & `netbox_plugin_prometheus_sd-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,68 @@
+Metadata-Version: 2.1
+Name: netbox-plugin-prometheus-sd
+Version: 1.1.0
+Summary: A Netbox plugin to provide Netbox entires to Prometheus HTTP service discovery
+License: MIT
+Author: Felix Peters
+Author-email: felix.peters@breuninger.de
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+
 # netbox-plugin-prometheus-sd
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![CI](https://github.com/FlxPeters/netbox-plugin-prometheus-sd/workflows/CI/badge.svg?event=push)](https://github.com/FlxPeters/netbox-plugin-prometheus-sd/actions?query=workflow%3ACI)
 [![PyPI](https://img.shields.io/pypi/v/netbox-plugin-prometheus-sd)](https://pypi.org/project/netbox-plugin-prometheus-sd/)
 
-Provide Prometheus http_sd compatible API Endpoint with data from Netbox.
+[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/flxpeters)
+
+Provide Prometheus `http_sd` compatible API Endpoint with data from Netbox.
 
-HTTP SD is a new feature in Prometheus 2.28.0 that allows hosts to be found via a URL instead of just files.
-This plugin implements API endpoints in Netbox to make devices, IPs and virtual machines available to Prometheus.
+HTTP SD is a feature since Prometheus 2.28.0 that allows hosts to be found via a URL instead of just files.
+This plugin implements API endpoints in Netbox to make devices, services, IPs and virtual machines available to Prometheus.
 
 ## Compatibility
 
-We aim to support the latest major versions of Netbox. For now we Support Netbox `3.2`, `3.3`, `3.4` and `3.5` including bugfix versions.
-Check the `.github/workflows/ci.yml` pipeline for the current tested builds. Other versions may work, but we do not test them explicitly.
-All relevant target versions are tested in CI. Have a look at the Github Actions definition for the current build targets.
+We aim to support the latest major versions of Netbox. For now we support Netbox `>= 3.3` including bugfix versions.
+
+Check the `.github/workflows/ci.yml` pipeline for the current tested builds.
+Other versions may work, but we do not test them explicitly. All relevant target versions are tested in CI.
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip
 
-    pip install netbox-plugin-prometheus-sd
+```bash
+pip install netbox-plugin-prometheus-sd
+```
 
 Enable the plugin in /opt/netbox/netbox/netbox/configuration.py:
 
+```python
     PLUGINS = ['netbox_prometheus_sd']
+```
 
-The plugin has not further plugin configuration at the moment.
+The plugin has not further plugin configuration.
 
 ## Usage
 
 The plugin only provides a new API endpoint on the Netbox API. There is no further action required after installation.
 
 ### API
 
 The plugin reuses Netbox API view sets with new serializers for Prometheus.
-This means that all filters that can be used on the Netbox api can also be used to filter Prometheus targets.
+This means that all filters that can be used on the Netbox API can also be used to filter Prometheus targets.
 Paging is disabled because Prometheus does not support paged results.
 
 The plugin also reuses the Netbox authentication and permission model.
 Depending on the Netbox configuration, a token with valid object permissions must be passed to Netbox.
 
 ```
 GET        /api/plugins/prometheus-sd/devices/              Get a list of devices in a prometheus compatible format
@@ -53,39 +77,41 @@
 The lookup is only executed against the `tenant` attribute of the object associated with the service.
 
 ### Config context
 
 The plugin can also discover extra config to inject in the HTTP SD JSON from the config context of the devices/virtual machines.
 If you have a `prometheus-plugin-prometheus-sd` entry in your config context with the following schema it will be automatically picked up:
 
-```
+```yaml
 prometheus-plugin-prometheus-sd:
   - metrics_path: /not/metrics
     port: 4242
     scheme: https
   - port: 4243
 ```
 
 This allow you to configure those values directly into netbox instead of doing that inside the Prometheus
 config and filtering each scenario by a specific tag for instance.
 
 If there is only one entry you can also use this form:
 
-```
+```yaml
 prometheus-plugin-prometheus-sd:
   metrics_path: /not/metrics
   port: 4242
   scheme: https
 ```
 
 ### Example
 
-A working example on how to use this plugin with Prometheus is located at the `example` folder. Netbox content is created by using Netbox docker initializers.
+A working example on how to use this plugin with Prometheus is located at the `example` folder.
+Netbox content is created by using Netbox docker initializers.
 
-The demo data doesn't make sense, but they are good enough for demonstrating how to configure Prometheus and get demo data to Prometheus service discovery.
+The demo data doesn't make sense, but they are good enough for demonstrating how to configure Prometheus
+and get demo data to Prometheus service discovery.
 
 Go to the `example` folder and run `docker-compose up`. Prometheus should get available on `http://localhost:9090`.
 
 Push some example devices and objects to Netbox using the initializers:
 
 ```
 docker-compose exec  netbox /opt/netbox/netbox/manage.py load_initializer_data --path /opt/netbox/initializers
@@ -100,28 +126,28 @@
 
 All code to run in docker is located under `develop`.
 To start a virtual env managed by poetry run `poetry shell`.
 All following commands are started inside this environment.
 
 In order to run tests invoke the test steps
 
-``` bash
+```bash
 # Build Docker images
 invoke build
 
 # Execute all tests
 invoke tests
 
 # Execute unit tests only
 invoke unittest
 ```
 
 Features should be covered by a unit test, but some times it's easier to develop on an running system.
 
-``` bash
+```bash
 # Start a local Netbox with docker
 invoke start
 
 # Create an user named `admin`
 invoke create-user
 ```
 
@@ -133,7 +159,8 @@
 ## Conventional Commits
 
 This repository follows the Conventional Commits specification for versioning and changelog generation.
 Conventional Commits provide a standardized way of writing commit messages to convey semantic meaning
 about the changes made. Each commit message follows a defined format that includes a type,
 an optional scope, and a message. The types typically include features, fixes, documentation, and more.
 By adhering to this convention, we ensure clear and automated versioning, release notes, and changelog generation.
+
```

### Comparing `netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/serializers.py` & `netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/utils.py` & `netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/api/utils.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/views.py` & `netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/filtersets.py` & `netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/filtersets.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Filtersets have been renamed, we support both
 # https://github.com/netbox-community/netbox/commit/1024782b9e0abb48f6da65f8248741227d53dbed#diff-d9224204dab475bbe888868c02235b8ef10f07c9201c45c90804d395dc161c40
 from django.db.models import Q
 from django.utils.translation import gettext as _
 
-from utilities.filters import MultiValueCharFilter, MultiValueNumberFilter
+from utilities.filters import MultiValueCharFilter, MultiValueNumberFilter, NumericArrayFilter
 
 try:
     from ipam.filtersets import ServiceFilterSet as NetboxServiceFilterSet
 except ImportError:
     from ipam.filters import ServiceFilterSet as NetboxServiceFilterSet
 
 
@@ -25,14 +25,21 @@
     )
 
     tenant = MultiValueCharFilter(
         method='filter_by_tenant_slug',
         label=_('Tenant (slug)'),
     )
 
+    # fix to make the test_missing_filters pass
+    # see: https://github.com/netbox-community/netbox/blob/master/netbox/utilities/testing/filtersets.py#L98
+    ports = NumericArrayFilter(
+        field_name='ports',
+        lookup_expr='contains'
+    )
+
     # pylint: disable=unused-argument
     def filter_by_cluster_tenant_id(self, queryset, name, value):
         return queryset.filter(
             Q(device__cluster__tenant_id__in=value) |
             Q(virtual_machine__cluster__tenant_id__in=value)
         )
```

### Comparing `netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/test_api.py` & `netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/tests/test_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import json
 
+try:
+    from users.models import ObjectPermission
+    from users.models import User
+    from core.models import ObjectType
+
+except ImportError:
+    # Fallback for old NetBox versions < 4.0
+    from django.contrib.contenttypes.models import ContentType as ObjectType
+    from django.contrib.auth.models import User
+
 from django.test import TestCase
-from django.contrib.contenttypes.models import ContentType
-from django.contrib.auth.models import User
 
 from rest_framework.test import APIClient
 from rest_framework import status
 
-from users.models import ObjectPermission
-
 from . import utils
 
 
 class ApiEndpointTests(TestCase):
     """Test cases for ensuring API endpoint is working properly."""
 
     def setUp(self):
@@ -21,24 +27,24 @@
 
         # Create test user and view permissions
         user = User.objects.create_user("username", "Pas$w0rd")
         obj_perm = ObjectPermission(name="test", actions=["view"])
         obj_perm.save()
         obj_perm.users.add(user)  # pylint: disable=no-member
         obj_perm.object_types.add(  # pylint: disable=no-member
-            ContentType.objects.get(app_label="dcim", model="device")
+            ObjectType.objects.get(app_label="dcim", model="device")
         )
         obj_perm.object_types.add(  # pylint: disable=no-member
-            ContentType.objects.get(app_label="ipam", model="ipaddress")
+            ObjectType.objects.get(app_label="ipam", model="ipaddress")
         )
         obj_perm.object_types.add(  # pylint: disable=no-member
-            ContentType.objects.get(app_label="ipam", model="service")
+            ObjectType.objects.get(app_label="ipam", model="service")
         )
         obj_perm.object_types.add(  # pylint: disable=no-member
-            ContentType.objects.get(app_label="virtualization", model="virtualmachine")
+            ObjectType.objects.get(app_label="virtualization", model="virtualmachine")
         )
         self.client.force_authenticate(user)
 
     def test_endpoint_device(self):
         """Ensure device endpoint returns a valid response"""
 
         for i in range(1, 61):
```

### Comparing `netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/test_filtersets.py` & `netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/tests/test_filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/test_serializers.py` & `netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/utils.py` & `netbox_plugin_prometheus_sd-1.1.0/netbox_prometheus_sd/tests/utils.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-1.0.0/pyproject.toml` & `netbox_plugin_prometheus_sd-1.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netbox-plugin-prometheus-sd"
-version = "1.0.0" # placeholder
+version = "v1.1.0" # placeholder
 description = "A Netbox plugin to provide Netbox entires to Prometheus HTTP service discovery"
 authors = ["Felix Peters <felix.peters@breuninger.de>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "netbox_prometheus_sd" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
 black = "^24.4"
 invoke = "^2.2.0"
-pylint = "^3.1.0"
+pylint = "^3.1.1"
 pylint-django = "^2.5.5"
 yamllint = "^1.35.1"
 typed-ast = "^1.5.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `netbox_plugin_prometheus_sd-1.0.0/PKG-INFO` & `netbox_plugin_prometheus_sd-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,51 @@
-Metadata-Version: 2.1
-Name: netbox-plugin-prometheus-sd
-Version: 1.0.0
-Summary: A Netbox plugin to provide Netbox entires to Prometheus HTTP service discovery
-License: MIT
-Author: Felix Peters
-Author-email: felix.peters@breuninger.de
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-
 # netbox-plugin-prometheus-sd
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![CI](https://github.com/FlxPeters/netbox-plugin-prometheus-sd/workflows/CI/badge.svg?event=push)](https://github.com/FlxPeters/netbox-plugin-prometheus-sd/actions?query=workflow%3ACI)
 [![PyPI](https://img.shields.io/pypi/v/netbox-plugin-prometheus-sd)](https://pypi.org/project/netbox-plugin-prometheus-sd/)
 
-Provide Prometheus http_sd compatible API Endpoint with data from Netbox.
+[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/flxpeters)
+
+Provide Prometheus `http_sd` compatible API Endpoint with data from Netbox.
 
-HTTP SD is a new feature in Prometheus 2.28.0 that allows hosts to be found via a URL instead of just files.
-This plugin implements API endpoints in Netbox to make devices, IPs and virtual machines available to Prometheus.
+HTTP SD is a feature since Prometheus 2.28.0 that allows hosts to be found via a URL instead of just files.
+This plugin implements API endpoints in Netbox to make devices, services, IPs and virtual machines available to Prometheus.
 
 ## Compatibility
 
-We aim to support the latest major versions of Netbox. For now we Support Netbox `3.2`, `3.3`, `3.4` and `3.5` including bugfix versions.
-Check the `.github/workflows/ci.yml` pipeline for the current tested builds. Other versions may work, but we do not test them explicitly.
-All relevant target versions are tested in CI. Have a look at the Github Actions definition for the current build targets.
+We aim to support the latest major versions of Netbox. For now we support Netbox `>= 3.3` including bugfix versions.
+
+Check the `.github/workflows/ci.yml` pipeline for the current tested builds.
+Other versions may work, but we do not test them explicitly. All relevant target versions are tested in CI.
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip
 
-    pip install netbox-plugin-prometheus-sd
+```bash
+pip install netbox-plugin-prometheus-sd
+```
 
 Enable the plugin in /opt/netbox/netbox/netbox/configuration.py:
 
+```python
     PLUGINS = ['netbox_prometheus_sd']
+```
 
-The plugin has not further plugin configuration at the moment.
+The plugin has not further plugin configuration.
 
 ## Usage
 
 The plugin only provides a new API endpoint on the Netbox API. There is no further action required after installation.
 
 ### API
 
 The plugin reuses Netbox API view sets with new serializers for Prometheus.
-This means that all filters that can be used on the Netbox api can also be used to filter Prometheus targets.
+This means that all filters that can be used on the Netbox API can also be used to filter Prometheus targets.
 Paging is disabled because Prometheus does not support paged results.
 
 The plugin also reuses the Netbox authentication and permission model.
 Depending on the Netbox configuration, a token with valid object permissions must be passed to Netbox.
 
 ```
 GET        /api/plugins/prometheus-sd/devices/              Get a list of devices in a prometheus compatible format
@@ -70,39 +60,41 @@
 The lookup is only executed against the `tenant` attribute of the object associated with the service.
 
 ### Config context
 
 The plugin can also discover extra config to inject in the HTTP SD JSON from the config context of the devices/virtual machines.
 If you have a `prometheus-plugin-prometheus-sd` entry in your config context with the following schema it will be automatically picked up:
 
-```
+```yaml
 prometheus-plugin-prometheus-sd:
   - metrics_path: /not/metrics
     port: 4242
     scheme: https
   - port: 4243
 ```
 
 This allow you to configure those values directly into netbox instead of doing that inside the Prometheus
 config and filtering each scenario by a specific tag for instance.
 
 If there is only one entry you can also use this form:
 
-```
+```yaml
 prometheus-plugin-prometheus-sd:
   metrics_path: /not/metrics
   port: 4242
   scheme: https
 ```
 
 ### Example
 
-A working example on how to use this plugin with Prometheus is located at the `example` folder. Netbox content is created by using Netbox docker initializers.
+A working example on how to use this plugin with Prometheus is located at the `example` folder.
+Netbox content is created by using Netbox docker initializers.
 
-The demo data doesn't make sense, but they are good enough for demonstrating how to configure Prometheus and get demo data to Prometheus service discovery.
+The demo data doesn't make sense, but they are good enough for demonstrating how to configure Prometheus
+and get demo data to Prometheus service discovery.
 
 Go to the `example` folder and run `docker-compose up`. Prometheus should get available on `http://localhost:9090`.
 
 Push some example devices and objects to Netbox using the initializers:
 
 ```
 docker-compose exec  netbox /opt/netbox/netbox/manage.py load_initializer_data --path /opt/netbox/initializers
@@ -117,28 +109,28 @@
 
 All code to run in docker is located under `develop`.
 To start a virtual env managed by poetry run `poetry shell`.
 All following commands are started inside this environment.
 
 In order to run tests invoke the test steps
 
-``` bash
+```bash
 # Build Docker images
 invoke build
 
 # Execute all tests
 invoke tests
 
 # Execute unit tests only
 invoke unittest
 ```
 
 Features should be covered by a unit test, but some times it's easier to develop on an running system.
 
-``` bash
+```bash
 # Start a local Netbox with docker
 invoke start
 
 # Create an user named `admin`
 invoke create-user
 ```
 
@@ -150,8 +142,7 @@
 ## Conventional Commits
 
 This repository follows the Conventional Commits specification for versioning and changelog generation.
 Conventional Commits provide a standardized way of writing commit messages to convey semantic meaning
 about the changes made. Each commit message follows a defined format that includes a type,
 an optional scope, and a message. The types typically include features, fixes, documentation, and more.
 By adhering to this convention, we ensure clear and automated versioning, release notes, and changelog generation.
-
```

