# Comparing `tmp/airbyte_source_snapchat_marketing-0.6.1.tar.gz` & `tmp/airbyte_source_snapchat_marketing-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_snapchat_marketing-0.6.1.tar", max compression
+gzip compressed data, was "airbyte_source_snapchat_marketing-0.6.2.tar", max compression
```

## Comparing `airbyte_source_snapchat_marketing-0.6.1.tar` & `airbyte_source_snapchat_marketing-0.6.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4712 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/README.md
--rw-r--r--   0        0        0      815 2024-05-07 12:32:32.839530 airbyte_source_snapchat_marketing-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1156 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/__init__.py
--rw-r--r--   0        0        0      264 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/run.py
--rw-r--r--   0        0        0     2621 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/adaccounts.json
--rw-r--r--   0        0        0     1656 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/ads.json
--rw-r--r--   0        0        0     8945 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/adsquads.json
--rw-r--r--   0        0        0     9688 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/basic_stats.json
--rw-r--r--   0        0        0     1659 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/campaigns.json
--rw-r--r--   0        0        0     3783 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/creatives.json
--rw-r--r--   0        0        0     2391 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/media.json
--rw-r--r--   0        0        0     3489 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/organizations.json
--rw-r--r--   0        0        0     2062 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/segments.json
--rw-r--r--   0        0        0    31941 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/source.py
--rw-r--r--   0        0        0     3503 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/spec.json
--rw-r--r--   0        0        0     5452 1970-01-01 00:00:00.000000 airbyte_source_snapchat_marketing-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     4722 2024-05-23 14:18:32.716943 airbyte_source_snapchat_marketing-0.6.2/README.md
+-rw-r--r--   0        0        0      815 2024-05-23 14:23:18.908814 airbyte_source_snapchat_marketing-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1156 2024-05-23 14:18:32.716943 airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/__init__.py
+-rw-r--r--   0        0        0      264 2024-05-23 14:18:32.716943 airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/run.py
+-rw-r--r--   0        0        0     2621 2024-05-23 14:18:32.716943 airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/adaccounts.json
+-rw-r--r--   0        0        0     1656 2024-05-23 14:18:32.716943 airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/ads.json
+-rw-r--r--   0        0        0     8945 2024-05-23 14:18:32.716943 airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/adsquads.json
+-rw-r--r--   0        0        0     9688 2024-05-23 14:18:32.716943 airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/basic_stats.json
+-rw-r--r--   0        0        0     1659 2024-05-23 14:18:32.716943 airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/campaigns.json
+-rw-r--r--   0        0        0     3783 2024-05-23 14:18:32.716943 airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/creatives.json
+-rw-r--r--   0        0        0     2391 2024-05-23 14:18:32.716943 airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/media.json
+-rw-r--r--   0        0        0     3489 2024-05-23 14:18:32.716943 airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/organizations.json
+-rw-r--r--   0        0        0     2062 2024-05-23 14:18:32.716943 airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/segments.json
+-rw-r--r--   0        0        0    30575 2024-05-23 14:18:32.716943 airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/source.py
+-rw-r--r--   0        0        0     3503 2024-05-23 14:18:32.716943 airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/spec.json
+-rw-r--r--   0        0        0     5462 1970-01-01 00:00:00.000000 airbyte_source_snapchat_marketing-0.6.2/PKG-INFO
```

### Comparing `airbyte_source_snapchat_marketing-0.6.1/README.md` & `airbyte_source_snapchat_marketing-0.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Snapchat-Marketing source connector
 
-
 This is the repository for the Snapchat-Marketing source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/snapchat-marketing).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/snapchat-marketing)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_snapchat_marketing/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-snapchat-marketing spec
 poetry run source-snapchat-marketing check --config secrets/config.json
 poetry run source-snapchat-marketing discover --config secrets/config.json
 poetry run source-snapchat-marketing read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-snapchat-marketing build
 ```
 
 An image will be available on your host with the tag `airbyte/source-snapchat-marketing:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-snapchat-marketing:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-snapchat-marketing:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-snapchat-marketing:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-snapchat-marketing:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-snapchat-marketing test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-snapchat-marketing test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/snapchat-marketing.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_snapchat_marketing-0.6.1/pyproject.toml` & `airbyte_source_snapchat_marketing-0.6.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.6.1"
+version = "0.6.2"
 name = "airbyte-source-snapchat-marketing"
 description = "Source implementation for Snapchat Marketing."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_snapchat_marketing" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "0.80.0"
+airbyte-cdk = "0.90.0"
 
 [tool.poetry.scripts]
 source-snapchat-marketing = "source_snapchat_marketing.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest-mock = "^3.6.1"
 pytest = "^6.1"
```

### Comparing `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/__init__.py` & `airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/adaccounts.json` & `airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/adaccounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/ads.json` & `airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/ads.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/adsquads.json` & `airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/adsquads.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/basic_stats.json` & `airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/basic_stats.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/campaigns.json` & `airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/creatives.json` & `airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/creatives.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/media.json` & `airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/media.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/organizations.json` & `airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/organizations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/segments.json` & `airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/schemas/segments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/source.py` & `airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 import pendulum
 import requests
 from airbyte_cdk.models import SyncMode
 from airbyte_cdk.sources import AbstractSource
 from airbyte_cdk.sources.streams import Stream
 from airbyte_cdk.sources.streams.core import IncrementalMixin, package_name_from_class
 from airbyte_cdk.sources.streams.http import HttpStream
-from airbyte_cdk.sources.streams.http.auth import Oauth2Authenticator
-from airbyte_cdk.sources.streams.http.exceptions import DefaultBackoffException
+from airbyte_cdk.sources.streams.http.requests_native_auth import Oauth2Authenticator
 from airbyte_cdk.sources.utils.schema_helpers import ResourceSchemaLoader
 
 # https://marketingapi.snapchat.com/docs/#core-metrics
 # https://marketingapi.snapchat.com/docs/#metrics-and-supported-granularities
 METRICS = [
     "android_installs",
     "attachment_avg_view_time_millis",
@@ -246,15 +245,15 @@
     def stream_slices(self, **kwargs) -> Iterable[Optional[Mapping[str, Any]]]:
 
         stream_state = kwargs.get("stream_state")
         self.initial_state = stream_state.get(self.cursor_field) if stream_state else self.start_date
         self.max_state = self.initial_state
 
         parent_stream = self.parent(
-            authenticator=self.authenticator,
+            authenticator=self._session.auth,
             start_date=self.start_date,
             end_date=self.end_date,
             action_report_time=self.action_report_time,
             swipe_up_attribution_window=self.swipe_up_attribution_window,
             view_attribution_window=self.view_attribution_window,
         )
         stream_slices = get_parent_ids(parent_stream)
@@ -375,15 +374,15 @@
     def parent(self) -> SnapchatMarketingStream:
         """Stream Class to extract entity ids from"""
 
     def stream_slices(self, **kwargs) -> Iterable[Optional[Mapping[str, Any]]]:
         """Each stream slice represents each entity id from parent stream"""
 
         parent_stream = self.parent(
-            authenticator=self.authenticator,
+            authenticator=self._session.auth,
             start_date=self.start_date,
             end_date=self.end_date,
             action_report_time=self.action_report_time,
             swipe_up_attribution_window=self.swipe_up_attribution_window,
             view_attribution_window=self.view_attribution_window,
         )
         self.parent_name = parent_stream.name
@@ -753,52 +752,21 @@
 
 class CampaignsStatsLifetime(Lifetime, Stats):
     """Campaigns stats with Lifetime granularity: https://marketingapi.snapchat.com/docs/#get-campaign-stats"""
 
     parent = Campaigns
 
 
-class SnapchatOauth2Authenticator(Oauth2Authenticator):
-    @backoff.on_exception(
-        backoff.expo,
-        DefaultBackoffException,
-        on_backoff=lambda details: logger.info(
-            f"Caught retryable error after {details['tries']} tries. Waiting {details['wait']} seconds then retrying..."
-        ),
-        max_time=300,
-    )
-    def refresh_access_token(self) -> Tuple[str, int]:
-        """
-        returns a tuple of (access_token, token_lifespan_in_seconds)
-        """
-        try:
-            response = requests.request(
-                method="POST",
-                url=self.token_refresh_endpoint,
-                data=self.get_refresh_request_body(),
-                headers=self.get_refresh_access_token_headers(),
-            )
-            response.raise_for_status()
-            response_json = response.json()
-            return response_json["access_token"], response_json["expires_in"]
-        except requests.exceptions.RequestException as e:
-            if e.response.status_code == 429 or e.response.status_code >= 500:
-                raise DefaultBackoffException(request=e.response.request, response=e.response)
-            raise
-        except Exception as e:
-            raise Exception(f"Error while refreshing access token: {e}") from e
-
-
 # Source
 class SourceSnapchatMarketing(AbstractSource):
     """Source Snapchat Marketing helps to retrieve the different Ad data from Snapchat business account"""
 
     def check_connection(self, logger, config) -> Tuple[bool, any]:
         try:
-            auth = SnapchatOauth2Authenticator(
+            auth = Oauth2Authenticator(
                 token_refresh_endpoint="https://accounts.snapchat.com/login/oauth2/access_token",
                 client_id=config["client_id"],
                 client_secret=config["client_secret"],
                 refresh_token=config["refresh_token"],
             )
             token = auth.get_access_token()
             url = f"{SnapchatMarketingStream.url_base}me"
@@ -816,15 +784,15 @@
         DELAYED_DAYS = 2
 
         # Start/End dates should better be in YYYY-MM-DD format:
         # 1. minutes are not supported
         # 2. when timezone is not specified, default account's timezone will be used automatically
         default_end_date = pendulum.now().subtract(days=DELAYED_DAYS).to_date_string()
         kwargs = {
-            "authenticator": SnapchatOauth2Authenticator(
+            "authenticator": Oauth2Authenticator(
                 token_refresh_endpoint="https://accounts.snapchat.com/login/oauth2/access_token",
                 client_id=config["client_id"],
                 client_secret=config["client_secret"],
                 refresh_token=config["refresh_token"],
             ),
             "start_date": config["start_date"],
             "end_date": config.get("end_date", default_end_date),
```

### Comparing `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/spec.json` & `airbyte_source_snapchat_marketing-0.6.2/source_snapchat_marketing/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.6.1/PKG-INFO` & `airbyte_source_snapchat_marketing-0.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,110 +1,124 @@
 Metadata-Version: 2.1
 Name: airbyte-source-snapchat-marketing
-Version: 0.6.1
+Version: 0.6.2
 Summary: Source implementation for Snapchat Marketing.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (==0.80.0)
+Requires-Dist: airbyte-cdk (==0.90.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/snapchat-marketing
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Snapchat-Marketing source connector
 
-
 This is the repository for the Snapchat-Marketing source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/snapchat-marketing).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/snapchat-marketing)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_snapchat_marketing/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-snapchat-marketing spec
 poetry run source-snapchat-marketing check --config secrets/config.json
 poetry run source-snapchat-marketing discover --config secrets/config.json
 poetry run source-snapchat-marketing read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-snapchat-marketing build
 ```
 
 An image will be available on your host with the tag `airbyte/source-snapchat-marketing:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-snapchat-marketing:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-snapchat-marketing:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-snapchat-marketing:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-snapchat-marketing:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-snapchat-marketing test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-snapchat-marketing test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/snapchat-marketing.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

