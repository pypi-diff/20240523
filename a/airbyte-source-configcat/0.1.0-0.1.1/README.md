# Comparing `tmp/airbyte-source-configcat-0.1.0.tar.gz` & `tmp/airbyte_source_configcat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-configcat-0.1.0.tar", last modified: Wed Jan 31 01:05:15 2024, max compression
+gzip compressed data, was "airbyte_source_configcat-0.1.1.tar", max compression
```

## Comparing `airbyte-source-configcat-0.1.0.tar` & `airbyte_source_configcat-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 01:05:15.791975 airbyte-source-configcat-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     4222 2024-01-31 01:05:15.791975 airbyte-source-configcat-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4041 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 01:05:15.787975 airbyte-source-configcat-0.1.0/airbyte_source_configcat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4222 2024-01-31 01:05:15.000000 airbyte-source-configcat-0.1.0/airbyte_source_configcat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      921 2024-01-31 01:05:15.000000 airbyte-source-configcat-0.1.0/airbyte_source_configcat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 01:05:15.000000 airbyte-source-configcat-0.1.0/airbyte_source_configcat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-01-31 01:05:15.000000 airbyte-source-configcat-0.1.0/airbyte_source_configcat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-31 01:05:15.000000 airbyte-source-configcat-0.1.0/airbyte_source_configcat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-01-31 01:05:15.000000 airbyte-source-configcat-0.1.0/airbyte_source_configcat.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 01:05:15.787975 airbyte-source-configcat-0.1.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       85 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      119 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       63 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4083 2024-01-31 01:05:15.791975 airbyte-source-configcat-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      930 2024-01-31 01:05:13.000000 airbyte-source-configcat-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 01:05:15.787975 airbyte-source-configcat-0.1.0/source_configcat/
--rw-r--r--   0 root         (0) root         (0)      130 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/source_configcat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2900 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/source_configcat/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      239 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/source_configcat/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 01:05:15.787975 airbyte-source-configcat-0.1.0/source_configcat/schemas/
--rw-r--r--   0 root         (0) root         (0)      502 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/source_configcat/schemas/environments.json
--rw-r--r--   0 root         (0) root         (0)      240 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/source_configcat/schemas/organization_members.json
--rw-r--r--   0 root         (0) root         (0)      199 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/source_configcat/schemas/organizations.json
--rw-r--r--   0 root         (0) root         (0)      400 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/source_configcat/schemas/products.json
--rw-r--r--   0 root         (0) root         (0)      283 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/source_configcat/schemas/tags.json
--rw-r--r--   0 root         (0) root         (0)      478 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/source_configcat/source.py
--rw-r--r--   0 root         (0) root         (0)      688 2024-01-31 00:49:03.000000 airbyte-source-configcat-0.1.0/source_configcat/spec.yaml
+-rw-r--r--   0        0        0     4550 2024-05-22 22:14:29.126326 airbyte_source_configcat-0.1.1/README.md
+-rw-r--r--   0        0        0      760 2024-05-22 22:20:17.807724 airbyte_source_configcat-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-05-22 22:14:29.130326 airbyte_source_configcat-0.1.1/source_configcat/__init__.py
+-rw-r--r--   0        0        0     2900 2024-05-22 22:14:29.130326 airbyte_source_configcat-0.1.1/source_configcat/manifest.yaml
+-rw-r--r--   0        0        0      239 2024-05-22 22:14:29.130326 airbyte_source_configcat-0.1.1/source_configcat/run.py
+-rw-r--r--   0        0        0      502 2024-05-22 22:14:29.130326 airbyte_source_configcat-0.1.1/source_configcat/schemas/environments.json
+-rw-r--r--   0        0        0      240 2024-05-22 22:14:29.130326 airbyte_source_configcat-0.1.1/source_configcat/schemas/organization_members.json
+-rw-r--r--   0        0        0      199 2024-05-22 22:14:29.130326 airbyte_source_configcat-0.1.1/source_configcat/schemas/organizations.json
+-rw-r--r--   0        0        0      400 2024-05-22 22:14:29.130326 airbyte_source_configcat-0.1.1/source_configcat/schemas/products.json
+-rw-r--r--   0        0        0      283 2024-05-22 22:14:29.130326 airbyte_source_configcat-0.1.1/source_configcat/schemas/tags.json
+-rw-r--r--   0        0        0      478 2024-05-22 22:14:29.130326 airbyte_source_configcat-0.1.1/source_configcat/source.py
+-rw-r--r--   0        0        0      688 2024-05-22 22:14:29.130326 airbyte_source_configcat-0.1.1/source_configcat/spec.yaml
+-rw-r--r--   0        0        0     5262 1970-01-01 00:00:00.000000 airbyte_source_configcat-0.1.1/PKG-INFO
```

### Comparing `airbyte-source-configcat-0.1.0/PKG-INFO` & `airbyte_source_configcat-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-configcat
-Version: 0.1.0
+Version: 0.1.1
 Summary: Source implementation for Configcat.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (==1.0.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/configcat
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Configcat Source
+# Configcat source connector
 
-This is the repository for the Configcat configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/configcat).
 
+This is the repository for the Configcat source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/configcat).
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/configcat)
+## Local development
+
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/configcat)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_configcat/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source configcat test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-configcat spec
+poetry run source-configcat check --config secrets/config.json
+poetry run source-configcat discover --config secrets/config.json
+poetry run source-configcat read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-configcat build
 ```
 
-An image will be built with the tag `airbyte/source-configcat:dev`.
+An image will be available on your host with the tag `airbyte/source-configcat:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-configcat:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-configcat:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-configcat:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-configcat:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-configcat:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-configcat test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-configcat test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/configcat.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/configcat.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-configcat-0.1.0/README.md` & `airbyte_source_configcat-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,91 @@
-# Configcat Source
+# Configcat source connector
 
-This is the repository for the Configcat configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/configcat).
+
+This is the repository for the Configcat source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/configcat).
 
 ## Local development
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/configcat)
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/configcat)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_configcat/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source configcat test creds`
-and place them into `secrets/config.json`.
 
-### Locally running the connector docker image
+### Locally running the connector
+```
+poetry run source-configcat spec
+poetry run source-configcat check --config secrets/config.json
+poetry run source-configcat discover --config secrets/config.json
+poetry run source-configcat read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-configcat build
 ```
 
-An image will be built with the tag `airbyte/source-configcat:dev`.
+An image will be available on your host with the tag `airbyte/source-configcat:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-configcat:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-configcat:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-configcat:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-configcat:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-configcat:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-configcat test
 ```
 
 ### Customizing acceptance Tests
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-## Dependency Management
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
 
-### Publishing a new version of the connector
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-configcat test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/configcat.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/configcat.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-configcat-0.1.0/source_configcat/manifest.yaml` & `airbyte_source_configcat-0.1.1/source_configcat/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-configcat-0.1.0/source_configcat/spec.yaml` & `airbyte_source_configcat-0.1.1/source_configcat/spec.yaml`

 * *Files identical despite different names*

