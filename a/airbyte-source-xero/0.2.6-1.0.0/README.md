# Comparing `tmp/airbyte_source_xero-0.2.6.tar.gz` & `tmp/airbyte_source_xero-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_xero-0.2.6.tar", max compression
+gzip compressed data, was "airbyte_source_xero-1.0.0.tar", max compression
```

## Comparing `airbyte_source_xero-0.2.6.tar` & `airbyte_source_xero-1.0.0.tar`

### file list

```diff
@@ -1,65 +1,9 @@
--rw-r--r--   0        0        0     4460 2024-05-19 23:00:37.135106 airbyte_source_xero-0.2.6/README.md
--rw-r--r--   0        0        0      731 2024-05-19 23:04:53.203544 airbyte_source_xero-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      120 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/__init__.py
--rw-r--r--   0        0        0      704 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/bootstrap.md
--rw-r--r--   0        0        0     2151 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/oauth.py
--rw-r--r--   0        0        0      224 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/run.py
--rw-r--r--   0        0        0     1218 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/accounts.json
--rw-r--r--   0        0        0      684 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/addresses.json
--rw-r--r--   0        0        0      286 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/allocations.json
--rw-r--r--   0        0        0      137 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/attachments.json
--rw-r--r--   0        0        0     1550 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/bank_transactions.json
--rw-r--r--   0        0        0      952 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/bank_transfers.json
--rw-r--r--   0        0        0      351 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/branding_themes.json
--rw-r--r--   0        0        0      323 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/contact_groups.json
--rw-r--r--   0        0        0     4460 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/contacts.json
--rw-r--r--   0        0        0     1940 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/credit_notes.json
--rw-r--r--   0        0        0      194 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/currencies.json
--rw-r--r--   0        0        0      297 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/customers.json
--rw-r--r--   0        0        0      467 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/employees.json
--rw-r--r--   0        0        0      929 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/expense_claims.json
--rw-r--r--   0        0        0     2938 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/invoices.json
--rw-r--r--   0        0        0     1620 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/items.json
--rw-r--r--   0        0        0     1785 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/journals.json
--rw-r--r--   0        0        0      801 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/line_items.json
--rw-r--r--   0        0        0      755 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/linked_transactions.json
--rw-r--r--   0        0        0     1588 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/manual_journals.json
--rw-r--r--   0        0        0     2250 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/nested_invoice.json
--rw-r--r--   0        0        0     2447 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/organisations.json
--rw-r--r--   0        0        0     1589 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/overpayments.json
--rw-r--r--   0        0        0      593 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/payment_terms.json
--rw-r--r--   0        0        0     1767 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/payments.json
--rw-r--r--   0        0        0      336 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/phones.json
--rw-r--r--   0        0        0     1588 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/prepayments.json
--rw-r--r--   0        0        0     2204 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/purchase_orders.json
--rw-r--r--   0        0        0     1546 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/quotes.json
--rw-r--r--   0        0        0     1252 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/receipts.json
--rw-r--r--   0        0        0     1718 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/repeating_invoices.json
--rw-r--r--   0        0        0     1218 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/accounts.json
--rw-r--r--   0        0        0      684 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/addresses.json
--rw-r--r--   0        0        0      286 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/allocations.json
--rw-r--r--   0        0        0      137 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/attachments.json
--rw-r--r--   0        0        0      351 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/branding_themes.json
--rw-r--r--   0        0        0      323 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/contact_groups.json
--rw-r--r--   0        0        0     4460 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/contacts.json
--rw-r--r--   0        0        0     1940 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/credit_notes.json
--rw-r--r--   0        0        0      801 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/line_items.json
--rw-r--r--   0        0        0     2250 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/nested_invoice.json
--rw-r--r--   0        0        0     1589 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/overpayments.json
--rw-r--r--   0        0        0      593 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/payment_terms.json
--rw-r--r--   0        0        0     1767 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/payments.json
--rw-r--r--   0        0        0      336 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/phones.json
--rw-r--r--   0        0        0     1588 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/prepayments.json
--rw-r--r--   0        0        0     1252 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/receipts.json
--rw-r--r--   0        0        0     1718 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/repeating_invoices.json
--rw-r--r--   0        0        0     1258 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/tracking_categories.json
--rw-r--r--   0        0        0      608 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/users.json
--rw-r--r--   0        0        0      204 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/validation_errors.json
--rw-r--r--   0        0        0     1282 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/tax_rates.json
--rw-r--r--   0        0        0     1258 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/tracking_categories.json
--rw-r--r--   0        0        0      608 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/users.json
--rw-r--r--   0        0        0      204 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/validation_errors.json
--rw-r--r--   0        0        0     3844 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/source.py
--rw-r--r--   0        0        0     3085 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/spec.yaml
--rw-r--r--   0        0        0     7358 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/streams.py
--rw-r--r--   0        0        0     5158 1970-01-01 00:00:00.000000 airbyte_source_xero-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     5119 2024-05-22 22:30:15.409653 airbyte_source_xero-1.0.0/README.md
+-rw-r--r--   0        0        0      132 2024-05-22 22:30:15.409653 airbyte_source_xero-1.0.0/main.py
+-rw-r--r--   0        0        0      754 2024-05-22 22:35:14.018701 airbyte_source_xero-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      120 2024-05-22 22:30:15.409653 airbyte_source_xero-1.0.0/source_xero/__init__.py
+-rw-r--r--   0        0        0     4006 2024-05-22 22:30:15.409653 airbyte_source_xero-1.0.0/source_xero/components.py
+-rw-r--r--   0        0        0    60056 2024-05-22 22:30:15.409653 airbyte_source_xero-1.0.0/source_xero/manifest.yaml
+-rw-r--r--   0        0        0      224 2024-05-22 22:30:15.409653 airbyte_source_xero-1.0.0/source_xero/run.py
+-rw-r--r--   0        0        0      473 2024-05-22 22:30:15.409653 airbyte_source_xero-1.0.0/source_xero/source.py
+-rw-r--r--   0        0        0     5835 1970-01-01 00:00:00.000000 airbyte_source_xero-1.0.0/PKG-INFO
```

### Comparing `airbyte_source_xero-0.2.6/README.md` & `airbyte_source_xero-1.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,91 +1,111 @@
 # Xero source connector
 
 
-This is the repository for the Xero source connector, written in Python.
+This is the repository for the Xero configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/xero).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
 
 
 ### Installing the connector
+
 From this connector directory, run:
 ```bash
 poetry install --with dev
 ```
 
 
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/xero)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_xero/spec.yaml` file.
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `spec` inside `manifest.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `sample_files/sample_config.json` for a sample config file.
+See `integration_tests/sample_config.json` for a sample config file.
 
 
 ### Locally running the connector
+
+
 ```
 poetry run source-xero spec
 poetry run source-xero check --config secrets/config.json
 poetry run source-xero discover --config secrets/config.json
-poetry run source-xero read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-xero read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
-### Running unit tests
-To run unit tests locally, from the connector directory run:
+### Running tests
+
+To run tests locally, from the connector directory run:
+
 ```
-poetry run pytest unit_tests
+poetry run pytest tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-xero build
 ```
 
 An image will be available on your host with the tag `airbyte/source-xero:dev`.
+An image will be available on your host with the tag `airbyte/source-xero:dev`.
 
 
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-xero:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-xero:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-xero:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-xero:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-xero test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
+
 All of your dependencies should be managed via Poetry. 
 To add a new dependency, run:
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-xero test`
 2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
     - bump the `dockerImageTag` value in in `metadata.yaml`
     - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/xero.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/xero.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_xero-0.2.6/pyproject.toml` & `airbyte_source_xero-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.6"
+version = "1.0.0"
 name = "airbyte-source-xero"
-description = "Source implementation for Xero."
+description = "Source implementation for xero."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
 documentation = "https://docs.airbyte.com/integrations/sources/xero"
 homepage = "https://airbyte.com"
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_xero" },
+    { include = "main.py" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "0.80.0"
+airbyte-cdk = "^1"
+pytz = "*"
 
 [tool.poetry.scripts]
 source-xero = "source_xero.run:run"
 
 [tool.poetry.group.dev.dependencies]
-requests-mock = "^1.9.3"
-pytest-mock = "^3.6.1"
-pytest = "^6.1"
+requests-mock = "*"
+pytest-mock = "*"
+pytest = "*"
```

### Comparing `airbyte_source_xero-0.2.6/PKG-INFO` & `airbyte_source_xero-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,110 +1,131 @@
 Metadata-Version: 2.1
 Name: airbyte-source-xero
-Version: 0.2.6
-Summary: Source implementation for Xero.
+Version: 1.0.0
+Summary: Source implementation for xero.
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
+Requires-Dist: airbyte-cdk (>=1,<2)
+Requires-Dist: pytz
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/xero
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Xero source connector
 
 
-This is the repository for the Xero source connector, written in Python.
+This is the repository for the Xero configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/xero).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
 
 
 ### Installing the connector
+
 From this connector directory, run:
 ```bash
 poetry install --with dev
 ```
 
 
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/xero)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_xero/spec.yaml` file.
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `spec` inside `manifest.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `sample_files/sample_config.json` for a sample config file.
+See `integration_tests/sample_config.json` for a sample config file.
 
 
 ### Locally running the connector
+
+
 ```
 poetry run source-xero spec
 poetry run source-xero check --config secrets/config.json
 poetry run source-xero discover --config secrets/config.json
-poetry run source-xero read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-xero read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
-### Running unit tests
-To run unit tests locally, from the connector directory run:
+### Running tests
+
+To run tests locally, from the connector directory run:
+
 ```
-poetry run pytest unit_tests
+poetry run pytest tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-xero build
 ```
 
 An image will be available on your host with the tag `airbyte/source-xero:dev`.
+An image will be available on your host with the tag `airbyte/source-xero:dev`.
 
 
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-xero:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-xero:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-xero:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-xero:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-xero test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
+
 All of your dependencies should be managed via Poetry. 
 To add a new dependency, run:
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-xero test`
 2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
     - bump the `dockerImageTag` value in in `metadata.yaml`
     - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/xero.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/xero.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

