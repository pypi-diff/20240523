# Comparing `tmp/dlt_init_openapi-0.0.5a2.tar.gz` & `tmp/dlt_init_openapi-0.0.5a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt_init_openapi-0.0.5a2.tar", max compression
+gzip compressed data, was "dlt_init_openapi-0.0.5a3.tar", max compression
```

## Comparing `dlt_init_openapi-0.0.5a2.tar` & `dlt_init_openapi-0.0.5a3.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0      840 2024-05-22 13:53:17.730342 dlt_init_openapi-0.0.5a2/CHANGELOG.md
--rw-r--r--   0        0        0     1111 2024-05-10 11:31:42.794290 dlt_init_openapi-0.0.5a2/LICENSE
--rw-r--r--   0        0        0     6195 2024-05-22 13:45:51.993375 dlt_init_openapi-0.0.5a2/README.md
--rw-r--r--   0        0        0     4712 2024-05-21 17:28:54.409899 dlt_init_openapi-0.0.5a2/dlt_init_openapi/__init__.py
--rw-r--r--   0        0        0       28 2024-05-21 17:28:54.410188 dlt_init_openapi-0.0.5a2/dlt_init_openapi/__main__.py
--rw-r--r--   0        0        0     4422 2024-05-22 13:45:51.993633 dlt_init_openapi-0.0.5a2/dlt_init_openapi/cli/__init__.py
--rw-r--r--   0        0        0     1151 2024-05-21 17:28:54.410397 dlt_init_openapi-0.0.5a2/dlt_init_openapi/cli/cli_endpoint_selection.py
--rw-r--r--   0        0        0     3320 2024-05-22 13:45:51.993782 dlt_init_openapi-0.0.5a2/dlt_init_openapi/config.py
--rw-r--r--   0        0        0       29 2024-05-21 17:28:54.410699 dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/__init__.py
--rw-r--r--   0        0        0      664 2024-05-21 17:28:54.410787 dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/base_detector.py
--rw-r--r--   0        0        0    22081 2024-05-21 17:28:54.410925 dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/__init__.py
--rw-r--r--   0        0        0     1048 2024-05-21 17:28:54.411220 dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/const.py
--rw-r--r--   0        0        0     1774 2024-05-21 17:28:54.411298 dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/primary_key.py
--rw-r--r--   0        0        0      686 2024-05-21 17:28:54.411376 dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/utils.py
--rw-r--r--   0        0        0     1573 2024-05-21 17:28:54.411449 dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/warnings.py
--rw-r--r--   0        0        0       47 2024-05-21 17:28:54.411692 dlt_init_openapi-0.0.5a2/dlt_init_openapi/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-21 17:28:54.411786 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/__init__.py
--rw-r--r--   0        0        0       57 2024-05-21 17:28:54.411874 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/config.py
--rw-r--r--   0        0        0       44 2024-05-21 17:28:54.412149 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/const.py
--rw-r--r--   0        0        0     2839 2024-05-21 17:28:54.412231 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/context.py
--rw-r--r--   0        0        0     9840 2024-05-22 13:45:51.994295 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/endpoints.py
--rw-r--r--   0        0        0     1376 2024-05-21 17:28:54.412635 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/errors.py
--rw-r--r--   0        0        0      704 2024-05-21 17:28:54.412728 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/info.py
--rw-r--r--   0        0        0    12896 2024-05-21 17:28:54.412851 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/models.py
--rw-r--r--   0        0        0     3303 2024-05-21 17:28:54.412942 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/openapi_parser.py
--rw-r--r--   0        0        0      670 2024-05-21 17:28:54.413023 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/pagination.py
--rw-r--r--   0        0        0     2766 2024-05-21 17:28:54.413107 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/parameters.py
--rw-r--r--   0        0        0        0 2024-05-21 17:28:54.413182 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/properties/__init__.py
--rw-r--r--   0        0        0     2365 2024-05-21 17:28:54.413458 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/properties/converter.py
--rw-r--r--   0        0        0      499 2024-05-21 17:28:54.413846 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/security.py
--rw-r--r--   0        0        0     2360 2024-05-21 17:28:54.413941 dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/types.py
--rw-r--r--   0        0        0       26 2024-05-21 17:28:54.414020 dlt_init_openapi-0.0.5a2/dlt_init_openapi/py.typed
--rw-r--r--   0        0        0        0 2024-05-21 17:28:54.414102 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/__init__.py
--rw-r--r--   0        0        0      516 2024-05-21 17:28:54.414198 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/base_renderer.py
--rw-r--r--   0        0        0     5869 2024-05-22 13:45:51.994512 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/__init__.py
--rw-r--r--   0        0        0      682 2024-05-21 17:28:54.414420 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/README.md.j2
--rw-r--r--   0        0        0      519 2024-05-22 13:45:51.994842 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/dlt_config.toml.j2
--rw-r--r--   0        0        0      148 2024-05-22 13:45:51.995003 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/dlt_secrets.toml.j2
--rw-r--r--   0        0        0      479 2024-05-22 13:45:51.995143 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/pipeline.py.j2
--rw-r--r--   0        0        0       11 2024-05-21 17:28:54.415547 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/requirements.txt.j2
--rw-r--r--   0        0        0     3774 2024-05-22 13:45:51.995284 dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/source.py.j2
--rw-r--r--   0        0        0      199 2024-05-21 17:28:54.415943 dlt_init_openapi-0.0.5a2/dlt_init_openapi/typing.py
--rw-r--r--   0        0        0        0 2024-05-21 17:28:54.416023 dlt_init_openapi-0.0.5a2/dlt_init_openapi/utils/__init__.py
--rw-r--r--   0        0        0     4137 2024-05-22 13:45:51.995498 dlt_init_openapi-0.0.5a2/dlt_init_openapi/utils/misc.py
--rw-r--r--   0        0        0     3851 2024-05-21 17:28:54.416842 dlt_init_openapi-0.0.5a2/dlt_init_openapi/utils/paths.py
--rw-r--r--   0        0        0     1162 2024-05-21 17:28:54.416919 dlt_init_openapi-0.0.5a2/dlt_init_openapi/utils/update_rest_api.py
--rw-r--r--   0        0        0     2536 2024-05-22 13:53:17.730687 dlt_init_openapi-0.0.5a2/pyproject.toml
--rw-r--r--   0        0        0     7781 1970-01-01 00:00:00.000000 dlt_init_openapi-0.0.5a2/PKG-INFO
+-rw-r--r--   0        0        0     1142 2024-05-23 07:45:35.046477 dlt_init_openapi-0.0.5a3/CHANGELOG.md
+-rw-r--r--   0        0        0     1111 2024-05-10 11:31:42.794290 dlt_init_openapi-0.0.5a3/LICENSE
+-rw-r--r--   0        0        0     6921 2024-05-23 07:11:02.287005 dlt_init_openapi-0.0.5a3/README.md
+-rw-r--r--   0        0        0     4712 2024-05-23 04:47:13.947771 dlt_init_openapi-0.0.5a3/dlt_init_openapi/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-23 04:47:13.947847 dlt_init_openapi-0.0.5a3/dlt_init_openapi/__main__.py
+-rw-r--r--   0        0        0     4422 2024-05-23 05:53:21.140594 dlt_init_openapi-0.0.5a3/dlt_init_openapi/cli/__init__.py
+-rw-r--r--   0        0        0     1151 2024-05-23 04:47:13.947996 dlt_init_openapi-0.0.5a3/dlt_init_openapi/cli/cli_endpoint_selection.py
+-rw-r--r--   0        0        0     3320 2024-05-23 05:53:21.140714 dlt_init_openapi-0.0.5a3/dlt_init_openapi/config.py
+-rw-r--r--   0        0        0       29 2024-05-23 04:47:13.948156 dlt_init_openapi-0.0.5a3/dlt_init_openapi/detector/__init__.py
+-rw-r--r--   0        0        0      664 2024-05-23 04:47:13.948219 dlt_init_openapi-0.0.5a3/dlt_init_openapi/detector/base_detector.py
+-rw-r--r--   0        0        0    22100 2024-05-23 07:11:02.287272 dlt_init_openapi-0.0.5a3/dlt_init_openapi/detector/default/__init__.py
+-rw-r--r--   0        0        0     1048 2024-05-23 04:47:13.948475 dlt_init_openapi-0.0.5a3/dlt_init_openapi/detector/default/const.py
+-rw-r--r--   0        0        0     1774 2024-05-23 04:47:13.948547 dlt_init_openapi-0.0.5a3/dlt_init_openapi/detector/default/primary_key.py
+-rw-r--r--   0        0        0      686 2024-05-23 04:47:13.948609 dlt_init_openapi-0.0.5a3/dlt_init_openapi/detector/default/utils.py
+-rw-r--r--   0        0        0     1573 2024-05-23 04:47:13.948668 dlt_init_openapi-0.0.5a3/dlt_init_openapi/detector/default/warnings.py
+-rw-r--r--   0        0        0       47 2024-05-23 04:47:13.948754 dlt_init_openapi-0.0.5a3/dlt_init_openapi/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-23 04:47:13.948783 dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-23 04:47:13.948849 dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/config.py
+-rw-r--r--   0        0        0       44 2024-05-23 04:47:13.948951 dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/const.py
+-rw-r--r--   0        0        0     2839 2024-05-23 04:47:13.949026 dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/context.py
+-rw-r--r--   0        0        0     9840 2024-05-23 05:53:21.141505 dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/endpoints.py
+-rw-r--r--   0        0        0     1376 2024-05-23 04:47:13.949244 dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/errors.py
+-rw-r--r--   0        0        0      704 2024-05-23 04:47:13.949307 dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/info.py
+-rw-r--r--   0        0        0    12896 2024-05-23 04:47:13.949454 dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/models.py
+-rw-r--r--   0        0        0     4264 2024-05-23 07:11:02.287939 dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/openapi_parser.py
+-rw-r--r--   0        0        0      670 2024-05-23 04:47:13.949606 dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/pagination.py
+-rw-r--r--   0        0        0     2766 2024-05-23 04:47:13.949686 dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/parameters.py
+-rw-r--r--   0        0        0        0 2024-05-23 04:47:13.949744 dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/properties/__init__.py
+-rw-r--r--   0        0        0     2365 2024-05-23 04:47:13.949854 dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/properties/converter.py
+-rw-r--r--   0        0        0      562 2024-05-23 07:11:02.288112 dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/security.py
+-rw-r--r--   0        0        0     2360 2024-05-23 04:47:13.950009 dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/types.py
+-rw-r--r--   0        0        0       26 2024-05-23 04:47:13.950067 dlt_init_openapi-0.0.5a3/dlt_init_openapi/py.typed
+-rw-r--r--   0        0        0        0 2024-05-23 04:47:13.950094 dlt_init_openapi-0.0.5a3/dlt_init_openapi/renderer/__init__.py
+-rw-r--r--   0        0        0      516 2024-05-23 04:47:13.950163 dlt_init_openapi-0.0.5a3/dlt_init_openapi/renderer/base_renderer.py
+-rw-r--r--   0        0        0     6123 2024-05-23 07:43:30.108512 dlt_init_openapi-0.0.5a3/dlt_init_openapi/renderer/default/__init__.py
+-rw-r--r--   0        0        0      684 2024-05-23 07:11:02.288285 dlt_init_openapi-0.0.5a3/dlt_init_openapi/renderer/default/templates/README.md.j2
+-rw-r--r--   0        0        0      519 2024-05-23 05:53:21.142183 dlt_init_openapi-0.0.5a3/dlt_init_openapi/renderer/default/templates/dlt_config.toml.j2
+-rw-r--r--   0        0        0      279 2024-05-23 07:43:30.108700 dlt_init_openapi-0.0.5a3/dlt_init_openapi/renderer/default/templates/dlt_secrets.toml.j2
+-rw-r--r--   0        0        0       62 2024-05-23 07:43:30.108831 dlt_init_openapi-0.0.5a3/dlt_init_openapi/renderer/default/templates/gitignore.j2
+-rw-r--r--   0        0        0      479 2024-05-23 05:53:21.142413 dlt_init_openapi-0.0.5a3/dlt_init_openapi/renderer/default/templates/pipeline.py.j2
+-rw-r--r--   0        0        0       11 2024-05-23 04:47:13.950645 dlt_init_openapi-0.0.5a3/dlt_init_openapi/renderer/default/templates/requirements.txt.j2
+-rw-r--r--   0        0        0     3831 2024-05-23 07:11:02.288645 dlt_init_openapi-0.0.5a3/dlt_init_openapi/renderer/default/templates/source.py.j2
+-rw-r--r--   0        0        0      199 2024-05-23 04:47:13.950759 dlt_init_openapi-0.0.5a3/dlt_init_openapi/typing.py
+-rw-r--r--   0        0        0        0 2024-05-23 04:47:13.950790 dlt_init_openapi-0.0.5a3/dlt_init_openapi/utils/__init__.py
+-rw-r--r--   0        0        0     4137 2024-05-23 05:53:21.142935 dlt_init_openapi-0.0.5a3/dlt_init_openapi/utils/misc.py
+-rw-r--r--   0        0        0     3851 2024-05-23 04:47:13.950988 dlt_init_openapi-0.0.5a3/dlt_init_openapi/utils/paths.py
+-rw-r--r--   0        0        0     1167 2024-05-23 07:11:02.288801 dlt_init_openapi-0.0.5a3/dlt_init_openapi/utils/update_rest_api.py
+-rw-r--r--   0        0        0     2536 2024-05-23 07:45:42.515129 dlt_init_openapi-0.0.5a3/pyproject.toml
+-rw-r--r--   0        0        0     8507 1970-01-01 00:00:00.000000 dlt_init_openapi-0.0.5a3/PKG-INFO
```

### Comparing `dlt_init_openapi-0.0.5a2/CHANGELOG.md` & `dlt_init_openapi-0.0.5a3/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 [Go to GitHub Releases](https://github.com/dlt-hub/dlt-init-openapi/releases)
 
+0.0.5a3
+* Render gitignore file and add source section to secrets.toml even if there are no secrets detected
+* Updated readme with feedback from users and added pip instructions
+* Make "username" a secret on basic auth
+* Prevent openapi 2.0 specs with helpful output on how to migrate
+* Fix e2e tests
+
 0.0.5a2
 * Better fallbacks for paginator and json_path if detection failed
 * Add telemetry on init command
 * Sanitze and snake case folders and files output
 
 0.0.5a1
 * pypi package and rename, pyproject fixes 0.0.5a1 pypi release
```

### Comparing `dlt_init_openapi-0.0.5a2/LICENSE` & `dlt_init_openapi-0.0.5a3/LICENSE`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/README.md` & `dlt_init_openapi-0.0.5a3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,62 +8,70 @@
 version 3 first with one of many available converters.
 
 
 ## Prior work
 This project started as a fork of [openapi-python-client](https://github.com/openapi-generators/openapi-python-client). Pretty much all parts are heavily changed or completely replaced, but some lines of code still exist and we like to acknowledge the many good ideas we got from the original project :)
 
 
+## Support
+If you need support for this tool, [join our slack community](https://dlthub.com/community) and ask for help on the technical help channel. We're usually around to help you out or discuss features :)
+
+
 ## Features
 The dlt-init-openapi generates code from an OpenAPI spec that you can use to extract data from a `rest_api` into any [`destination`](https://dlthub.com/docs/dlt-ecosystem/destinations/) (e.g. Postgres, BigQuery, Redshift...) `dlt` supports.
 
 Features include
 
-* [Pagination](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#pagination) discovery
-* Primary key discovery
-* Endpoint relationship mapping into `dlt` [`transformers`](https://dlthub.com/docs/general-usage/resource#process-resources-with-dlttransformer) (e.g. /users/ -> /user/{id})
-* Payload JSON path [data selector](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#data-selection) discovery for nested results
-* [Authentication](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#authentication) discovery
+* **[Pagination](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#pagination) discovery** for each endpoint
+* **Primary key discovery** for each entity
+* **Endpoint relationship mapping** into `dlt` [`transformers`](https://dlthub.com/docs/general-usage/resource#process-resources-with-dlttransformer) (e.g. /users/ -> /user/{id})
+* **Payload JSON path [data selector](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#data-selection) discovery** for results nested in the returned json
+* **[Authentication](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#authentication)** discovery for an API
 
 ## Setup
 
-You will need Python 3.9 installed, as well as [`poetry`](https://python-poetry.org/docs/) to install dependencies.
+You will need Python 3.9 or higher installed, as well as pip.
 
 ```console
-# 1. Checkout this repository locally
-$ git clone git@github.com:dlt-hub/dlt-init-openapi.git
-
-# 2. Install required poetry dependencies
-$ poetry install
+# 1. install this tool locally
+$ pip install dlt-init-openapi
 
-# 3. Start the poetry shell
-$ poetry shell
+# 2. Show the version of the installed package to verify it worked
+$ dlt-init-openapi --version
 ```
 
 ## Basic Usage
 
 Let's create an example pipeline from the [PokeAPI spec](https://raw.githubusercontent.com/cliffano/pokeapi-clients/ec9a2707ef2a85f41b747d8df013e272ef650ec5/specification/pokeapi.yml). You can point to any other OpenAPI Spec instead if you like.
 
 ```console
-# 1. Run the generator with the dlt-init-openapi init command:
+# 1.a. Run the generator with the dlt-init-openapi init command:
 $ dlt-init-openapi init pokemon --url https://raw.githubusercontent.com/cliffano/pokeapi-clients/ec9a2707ef2a85f41b747d8df013e272ef650ec5/specification/pokeapi.yml
 
+# 1.b. If you have a local file, you can use the --path flag:
+$ dlt-init-openapi init pokemon --path ./my_specs/pokeapi.yml
+
 # 2. You can now pick the endpoints you need from the popup
 
 # 3. After selecting your pokemon endpoints and hitting Enter, your pipeline will be rendered
 
-# 4. Go to the created pipeline folder and run your pipeline
+# 4. If you have any kind of authentication on your pipeline (this example has not), open the `.dlt/secrets.toml` and provide the credentials. You can find further settings in the `.dlt/config.toml`.
+
+# 5. Go to the created pipeline folder and run your pipeline
 $ cd pokemon-pipeline
 $ PROGRESS=enlighten python pipeline.py # we use enlighten for a nice progress bar :)
 
-# 5. Print the pipeline info to console to see what got loaded
+# 6. Print the pipeline info to console to see what got loaded
 $ dlt pipeline pokemon_pipeline info
 
-# 6. You can now also install streamlit to see a preview of the data
+# 7. You can now also install streamlit to see a preview of the data
 $ pip install pandas streamlit
 $ dlt pipeline pokemon_pipeline show
+
+# 8. You can go to our docs at https://dlthub.com/docs to learn how modify the generated pipeline to load to many destinations, place schema contracts on your pipeline and many other things.
 ```
 
 ## What will be created?
 When you run the `init` command above, the following files will be generated:
 
 * `./pokemon-pipeline` - a folder containing the full project.
 * `./pokemon-pipeline/pipeline.py` - a file which you can execute to run your pipeline.
```

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/__init__.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/cli/__init__.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/cli/cli_endpoint_selection.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/cli/cli_endpoint_selection.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/config.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/config.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/base_detector.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/detector/base_detector.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/__init__.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/detector/default/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,30 +88,30 @@
     def detect_security_schemes(self, open_api: OpenapiParser) -> None:
 
         # detect scheme settings
         # TODO: make this a bit nicer
         for name, scheme in open_api.security_schemes.items():
 
             if scheme.type == "apiKey":
-                scheme.detected_secret_name = "api_key"
+                scheme.detected_secret_names = ["api_key"]
                 scheme.detected_auth_vars = f"""
             "type": "api_key",
             "api_key": api_key,
             "name": "{scheme.name}",
             "location": "{scheme.location}"
 """
             elif scheme.type == "http" and scheme.scheme == "basic":
-                scheme.detected_secret_name = "password"
+                scheme.detected_secret_names = ["username", "password"]
                 scheme.detected_auth_vars = """
             "type": "http_basic",
-            "username": "username",
+            "username": username,
             "password": password,
 """
             elif scheme.type == "http" and scheme.scheme == "bearer":
-                scheme.detected_secret_name = "token"
+                scheme.detected_secret_names = ["token"]
                 scheme.detected_auth_vars = """
             "type": "bearer",
             "token": token,
 """
 
         # find default scheme
         if open_api.global_security_name:
```

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/const.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/detector/default/const.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/primary_key.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/detector/default/primary_key.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/utils.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/detector/default/utils.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/detector/default/warnings.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/detector/default/warnings.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/context.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/context.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/endpoints.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/endpoints.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/errors.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/errors.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/info.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/info.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/models.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/models.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/openapi_parser.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/openapi_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -38,14 +38,36 @@
         logger.info("Validating spec structure")
         try:
             spec = osp.OpenAPI.parse_obj(self.spec_raw)
         except Exception as e:
             raise DltOpenAPIException("Could not Validate spec:\n" + str(e)) from e
         logger.success("Spec validation successful")
 
+        # check if this is openapi 3.0
+        convert_info = (
+            "you can convert it to an openapi 3.0 spec by going to https://editor.swagger.io/, "
+            + "pasting your spec and selecting 'Edit' -> 'Convert to OpenAPI 3.0' from the Menu "
+            + "and then retry with the converted file."
+        )
+        swagger_version = self.spec_raw.get("swagger")
+        if swagger_version:
+            logger.error(
+                "The spec you selected appears to be a Swagger/OpenAPI version 2 spec or older, " + convert_info
+            )
+            exit(0)
+
+        openapi_version = self.spec_raw.get("openapi")
+        if not openapi_version or not openapi_version.startswith("3"):
+            logger.error(
+                "The spec you selected does not appear to be an OpenAPI 3.0 spec. "
+                + "If this is a a Swagger/OpenAPI version 2 spec or older, "
+                + convert_info
+            )
+            exit(1)
+
         logger.info("Extracting openapi metadata")
         self.context = OpenapiContext(self.config, spec, self.spec_raw)
         self.info = OpenApiInfo.from_context(self.context)
         logger.success("Completed extracting openapi metadata and credentials.")
 
         logger.info("Extracting security schemes")
         if spec.security:
```

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/pagination.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/pagination.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/parameters.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/parameters.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/properties/converter.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/properties/converter.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/parser/types.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/parser/types.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/base_renderer.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/renderer/base_renderer.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/__init__.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/renderer/default/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,21 @@
         readme_template = self.env.get_template("README.md.j2")
         readme_path = self.config.project_dir / "README.md"
         readme_path.write_text(
             readme_template.render(endpoint_collection=self.openapi.endpoints, version=__version__),
             encoding=FILE_ENCODING,
         )
 
+        gitignore_template = self.env.get_template("gitignore.j2")
+        gitignore_path = self.config.project_dir / ".gitignore"
+        gitignore_path.write_text(
+            gitignore_template.render(),
+            encoding=FILE_ENCODING,
+        )
+
     def _create_package(self) -> None:
         self.config.project_dir.mkdir(exist_ok=True, parents=True)
         self.package_dir.mkdir(exist_ok=True)
 
     def _build_dlt_config(self) -> None:
         config_dir = self.config.project_dir / ".dlt"
         config_dir.mkdir(exist_ok=True)
```

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/README.md.j2` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/renderer/default/templates/README.md.j2`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 * https://dlthub.com
 * https://github.com/dlt-hub/dlt
 * https://github.com/dlt-hub/dlt-init-openapi
 
 {% if credentials %}
 ## Credentials
-This API uses {{ credentials.type }} authentication. Please fill in the required variable {{ credentials.detected_secret_name }} in your 
+This API uses {{ credentials.type }} authentication. Please fill in the required variables {{ credentials.detected_secret_names }} in your 
 secrets.toml.
 {% endif %}
 
 ## Available resources
 {% for endpoint in endpoint_collection.all_endpoints_to_render %}
 * {{ endpoint.detected_resource_name }}  
   _{{endpoint.method}} {{ endpoint.path }}_
```

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/dlt_config.toml.j2` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/renderer/default/templates/dlt_config.toml.j2`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/renderer/default/templates/source.py.j2` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/renderer/default/templates/source.py.j2`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from rest_api.typing import RESTAPIConfig
 from rest_api import rest_api_source
 
 
 @dlt.source(name="{{source_name}}", max_table_nesting=2)
 def {{ source_name }}(
         {% if credentials %}
-        {{ credentials.detected_secret_name }}: str = dlt.secrets.value,
+        {% for secret in credentials.detected_secret_names %}
+        {{ secret }}: str = dlt.secrets.value,
+        {% endfor %}
         {% endif %}
         base_url: str = dlt.config.value,
 ) -> List[DltResource]:
 
     # source configuration
     source_config: RESTAPIConfig = {
         "client": {
```

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/utils/misc.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/utils/paths.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/utils/paths.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.0.5a2/dlt_init_openapi/utils/update_rest_api.py` & `dlt_init_openapi-0.0.5a3/dlt_init_openapi/utils/update_rest_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,8 +28,8 @@
             with open(dst_path, "wb") as f:
                 for chunk in r.iter_content(chunk_size=8192):
                     f.write(chunk)
     logger.success("rest_api verified source synced")
 
 
 if __name__ == "__main__":
-    update_rest_api()
+    update_rest_api(False)
```

### Comparing `dlt_init_openapi-0.0.5a2/pyproject.toml` & `dlt_init_openapi-0.0.5a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt-init-openapi"
-version = "0.0.5a2"
+version = "0.0.5a3"
 description = "Generate dlt Python clients from OpenAPI"
 homepage = "https://dlthub.com"
 repository = "https://github.com/dlt-hub/dlt-init-openapi"
 license = "MIT"
 keywords=["OpenAPI", "Client", "Generator"]
 authors = ["David Scharf <david@dlthub.com>"]
 classifiers = [
```

### Comparing `dlt_init_openapi-0.0.5a2/PKG-INFO` & `dlt_init_openapi-0.0.5a3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt-init-openapi
-Version: 0.0.5a2
+Version: 0.0.5a3
 Summary: Generate dlt Python clients from OpenAPI
 Home-page: https://dlthub.com
 License: MIT
 Keywords: OpenAPI,Client,Generator
 Author: David Scharf
 Author-email: david@dlthub.com
 Requires-Python: >=3.9,<3.13
@@ -48,62 +48,70 @@
 version 3 first with one of many available converters.
 
 
 ## Prior work
 This project started as a fork of [openapi-python-client](https://github.com/openapi-generators/openapi-python-client). Pretty much all parts are heavily changed or completely replaced, but some lines of code still exist and we like to acknowledge the many good ideas we got from the original project :)
 
 
+## Support
+If you need support for this tool, [join our slack community](https://dlthub.com/community) and ask for help on the technical help channel. We're usually around to help you out or discuss features :)
+
+
 ## Features
 The dlt-init-openapi generates code from an OpenAPI spec that you can use to extract data from a `rest_api` into any [`destination`](https://dlthub.com/docs/dlt-ecosystem/destinations/) (e.g. Postgres, BigQuery, Redshift...) `dlt` supports.
 
 Features include
 
-* [Pagination](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#pagination) discovery
-* Primary key discovery
-* Endpoint relationship mapping into `dlt` [`transformers`](https://dlthub.com/docs/general-usage/resource#process-resources-with-dlttransformer) (e.g. /users/ -> /user/{id})
-* Payload JSON path [data selector](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#data-selection) discovery for nested results
-* [Authentication](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#authentication) discovery
+* **[Pagination](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#pagination) discovery** for each endpoint
+* **Primary key discovery** for each entity
+* **Endpoint relationship mapping** into `dlt` [`transformers`](https://dlthub.com/docs/general-usage/resource#process-resources-with-dlttransformer) (e.g. /users/ -> /user/{id})
+* **Payload JSON path [data selector](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#data-selection) discovery** for results nested in the returned json
+* **[Authentication](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#authentication)** discovery for an API
 
 ## Setup
 
-You will need Python 3.9 installed, as well as [`poetry`](https://python-poetry.org/docs/) to install dependencies.
+You will need Python 3.9 or higher installed, as well as pip.
 
 ```console
-# 1. Checkout this repository locally
-$ git clone git@github.com:dlt-hub/dlt-init-openapi.git
-
-# 2. Install required poetry dependencies
-$ poetry install
+# 1. install this tool locally
+$ pip install dlt-init-openapi
 
-# 3. Start the poetry shell
-$ poetry shell
+# 2. Show the version of the installed package to verify it worked
+$ dlt-init-openapi --version
 ```
 
 ## Basic Usage
 
 Let's create an example pipeline from the [PokeAPI spec](https://raw.githubusercontent.com/cliffano/pokeapi-clients/ec9a2707ef2a85f41b747d8df013e272ef650ec5/specification/pokeapi.yml). You can point to any other OpenAPI Spec instead if you like.
 
 ```console
-# 1. Run the generator with the dlt-init-openapi init command:
+# 1.a. Run the generator with the dlt-init-openapi init command:
 $ dlt-init-openapi init pokemon --url https://raw.githubusercontent.com/cliffano/pokeapi-clients/ec9a2707ef2a85f41b747d8df013e272ef650ec5/specification/pokeapi.yml
 
+# 1.b. If you have a local file, you can use the --path flag:
+$ dlt-init-openapi init pokemon --path ./my_specs/pokeapi.yml
+
 # 2. You can now pick the endpoints you need from the popup
 
 # 3. After selecting your pokemon endpoints and hitting Enter, your pipeline will be rendered
 
-# 4. Go to the created pipeline folder and run your pipeline
+# 4. If you have any kind of authentication on your pipeline (this example has not), open the `.dlt/secrets.toml` and provide the credentials. You can find further settings in the `.dlt/config.toml`.
+
+# 5. Go to the created pipeline folder and run your pipeline
 $ cd pokemon-pipeline
 $ PROGRESS=enlighten python pipeline.py # we use enlighten for a nice progress bar :)
 
-# 5. Print the pipeline info to console to see what got loaded
+# 6. Print the pipeline info to console to see what got loaded
 $ dlt pipeline pokemon_pipeline info
 
-# 6. You can now also install streamlit to see a preview of the data
+# 7. You can now also install streamlit to see a preview of the data
 $ pip install pandas streamlit
 $ dlt pipeline pokemon_pipeline show
+
+# 8. You can go to our docs at https://dlthub.com/docs to learn how modify the generated pipeline to load to many destinations, place schema contracts on your pipeline and many other things.
 ```
 
 ## What will be created?
 When you run the `init` command above, the following files will be generated:
 
 * `./pokemon-pipeline` - a folder containing the full project.
 * `./pokemon-pipeline/pipeline.py` - a file which you can execute to run your pipeline.
```

