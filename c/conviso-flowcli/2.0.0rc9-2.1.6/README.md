# Comparing `tmp/conviso-flowcli-2.0.0rc9.tar.gz` & `tmp/conviso-flowcli-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conviso-flowcli-2.0.0rc9.tar", last modified: Wed Jan 17 21:40:26 2024, max compression
+gzip compressed data, was "conviso-flowcli-2.1.6.tar", last modified: Thu May 23 13:03:50 2024, max compression
```

## Comparing `conviso-flowcli-2.0.0rc9.tar` & `conviso-flowcli-2.1.6.tar`

### file list

```diff
@@ -1,166 +1,169 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/
--rw-r--r--   0 root         (0) root         (0)      497 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      234 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.153240 conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      497 2024-01-17 21:40:26.000000 conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5567 2024-01-17 21:40:26.000000 conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-17 21:40:26.000000 conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-01-17 21:40:26.000000 conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      232 2024-01-17 21:40:26.000000 conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-01-17 21:40:26.000000 conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.153240 conviso-flowcli-2.0.0rc9/convisoappsec/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.153240 conviso-flowcli-2.0.0rc9/convisoappsec/common/
--rw-r--r--   0 root         (0) root         (0)      105 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7970 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/box.py
--rw-r--r--   0 root         (0) root         (0)    12525 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/docker.py
--rw-r--r--   0 root         (0) root         (0)      230 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2067 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/git_data_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.153240 conviso-flowcli-2.0.0rc9/convisoappsec/common/graphql/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2055 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/graphql/error_handlers.py
--rw-r--r--   0 root         (0) root         (0)      247 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/graphql/errors.py
--rw-r--r--   0 root         (0) root         (0)     1294 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/graphql/low_client.py
--rw-r--r--   0 root         (0) root         (0)      185 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/common/strings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/
--rw-r--r--   0 root         (0) root         (0)       81 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11584 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/__init__.py
--rw-r--r--   0 root         (0) root         (0)      502 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/__init__.py
--rw-r--r--   0 root         (0) root         (0)      311 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/iac.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/normalize.py
--rw-r--r--   0 root         (0) root         (0)     1488 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/sast.py
--rw-r--r--   0 root         (0) root         (0)     1349 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/sca.py
--rw-r--r--   0 root         (0) root         (0)     2113 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/resources_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/schemas/mutations/
--rw-r--r--   0 root         (0) root         (0)      327 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/schemas/resolvers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/schemas/resolvers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      790 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      345 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/models/asset.py
--rw-r--r--   0 root         (0) root         (0)      863 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/models/project.py
--rw-r--r--   0 root         (0) root         (0)     5835 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/resources_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/schemas/mutations/
--rw-r--r--   0 root         (0) root         (0)      970 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/schemas/resolvers/
--rw-r--r--   0 root         (0) root         (0)     1522 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/source_code_scanner/
--rw-r--r--   0 root         (0) root         (0)      227 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/source_code_scanner/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/source_code_scanner/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1655 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/source_code_scanner/scc.py
--rw-r--r--   0 root         (0) root         (0)     4726 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/source_code_scanner/source_code_scanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/util/
--rw-r--r--   0 root         (0) root         (0)      160 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2093 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/util/ci_provider.py
--rw-r--r--   0 root         (0) root         (0)      480 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/util/metrics.py
--rw-r--r--   0 root         (0) root         (0)      508 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/util/source_code_compressor.py
--rw-r--r--   0 root         (0) root         (0)    12087 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_control_system_adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/
--rw-r--r--   0 root         (0) root         (0)      294 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py
--rw-r--r--   0 root         (0) root         (0)     1266 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/timebased_version_seacher.py
--rw-r--r--   0 root         (0) root         (0)      943 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/version_searcher_result.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.157240 conviso-flowcli-2.0.0rc9/convisoappsec/flow/versioning_style/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/versioning_style/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1041 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flow/versioning_style/semantic_versioning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/
--rw-r--r--   0 root         (0) root         (0)       64 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/__init__.py
--rw-r--r--   0 root         (0) root         (0)       99 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/assets/
--rw-r--r--   0 root         (0) root         (0)       54 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2278 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/assets/create.py
--rw-r--r--   0 root         (0) root         (0)      310 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/assets/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     1484 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/assets/ls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/ast/
--rw-r--r--   0 root         (0) root         (0)       47 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/ast/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6207 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/ast/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     5350 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/companies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/companies/__init__.py
--rw-r--r--   0 root         (0) root         (0)      892 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/companies/ls.py
--rw-r--r--   0 root         (0) root         (0)     1309 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/
--rw-r--r--   0 root         (0) root         (0)       54 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/
--rw-r--r--   0 root         (0) root         (0)       54 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/__init__.py
--rw-r--r--   0 root         (0) root         (0)      190 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/context.py
--rw-r--r--   0 root         (0) root         (0)      677 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/
--rw-r--r--   0 root         (0) root         (0)       51 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/__init__.py
--rw-r--r--   0 root         (0) root         (0)      346 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/
--rw-r--r--   0 root         (0) root         (0)       64 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      194 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/context.py
--rw-r--r--   0 root         (0) root         (0)      675 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/
--rw-r--r--   0 root         (0) root         (0)       56 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/__init__.py
--rw-r--r--   0 root         (0) root         (0)      382 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     2815 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py
--rw-r--r--   0 root         (0) root         (0)     3500 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py
--rw-r--r--   0 root         (0) root         (0)     4580 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/values.py
--rw-r--r--   0 root         (0) root         (0)      353 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      763 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/ls.py
--rw-r--r--   0 root         (0) root         (0)      970 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/show.py
--rw-r--r--   0 root         (0) root         (0)     2878 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/
--rw-r--r--   0 root         (0) root         (0)       58 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/
--rw-r--r--   0 root         (0) root         (0)       54 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/__init__.py
--rw-r--r--   0 root         (0) root         (0)      269 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/with_/
--rw-r--r--   0 root         (0) root         (0)       51 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/with_/__init__.py
--rw-r--r--   0 root         (0) root         (0)      309 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/with_/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/with_/version_tracker.py
--rw-r--r--   0 root         (0) root         (0)      344 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.161240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/import_sarif/
--rw-r--r--   0 root         (0) root         (0)       66 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/import_sarif/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7209 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/import_sarif/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      331 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/help_option.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/iac/
--rw-r--r--   0 root         (0) root         (0)       47 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/iac/__init__.py
--rw-r--r--   0 root         (0) root         (0)      241 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/iac/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    11081 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/iac/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/projects/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/projects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/projects/ls.py
--rw-r--r--   0 root         (0) root         (0)     8055 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/requirements_verifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sast/
--rw-r--r--   0 root         (0) root         (0)       49 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sast/__init__.py
--rw-r--r--   0 root         (0) root         (0)      245 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sast/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    15835 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sast/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sca/
--rw-r--r--   0 root         (0) root         (0)       47 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sca/__init__.py
--rw-r--r--   0 root         (0) root         (0)      241 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sca/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    10508 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sca/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/vulnerability/
--rw-r--r--   0 root         (0) root         (0)       67 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/vulnerability/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4298 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/vulnerability/assert_security_rules.py
--rw-r--r--   0 root         (0) root         (0)      335 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/vulnerability/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      231 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/convisoappsec/sast/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/sast/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/sast/decision.py
--rw-r--r--   0 root         (0) root         (0)     6218 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/sast/sastbox.py
--rw-r--r--   0 root         (0) root         (0)       27 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/convisoappsec/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.153240 conviso-flowcli-2.0.0rc9/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/scripts/shell_completer/
--rw-r--r--   0 root         (0) root         (0)      624 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/scripts/shell_completer/flow_bash_completer.sh
--rw-r--r--   0 root         (0) root         (0)      147 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/scripts/shell_completer/flow_fish_completer.fish
--rw-r--r--   0 root         (0) root         (0)      844 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/scripts/shell_completer/flow_zsh_completer.sh
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-17 21:40:26.165240 conviso-flowcli-2.0.0rc9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1744 2024-01-17 21:40:22.000000 conviso-flowcli-2.0.0rc9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.462202 conviso-flowcli-2.1.6/
+-rw-r--r--   0 root         (0) root         (0)      545 2024-05-23 13:03:50.462202 conviso-flowcli-2.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      234 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.450202 conviso-flowcli-2.1.6/conviso_flowcli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      545 2024-05-23 13:03:50.000000 conviso-flowcli-2.1.6/conviso_flowcli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5715 2024-05-23 13:03:50.000000 conviso-flowcli-2.1.6/conviso_flowcli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 13:03:50.000000 conviso-flowcli-2.1.6/conviso_flowcli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-05-23 13:03:50.000000 conviso-flowcli-2.1.6/conviso_flowcli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      248 2024-05-23 13:03:50.000000 conviso-flowcli-2.1.6/conviso_flowcli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-23 13:03:50.000000 conviso-flowcli-2.1.6/conviso_flowcli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.450202 conviso-flowcli-2.1.6/convisoappsec/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.450202 conviso-flowcli-2.1.6/convisoappsec/common/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7686 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/common/box.py
+-rw-r--r--   0 root         (0) root         (0)    12525 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/common/docker.py
+-rw-r--r--   0 root         (0) root         (0)      230 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/common/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/common/git_data_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.450202 conviso-flowcli-2.1.6/convisoappsec/common/graphql/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/common/graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/common/graphql/error_handlers.py
+-rw-r--r--   0 root         (0) root         (0)      247 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/common/graphql/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/common/graphql/low_client.py
+-rw-r--r--   0 root         (0) root         (0)      185 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/common/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.450202 conviso-flowcli-2.1.6/convisoappsec/flow/
+-rw-r--r--   0 root         (0) root         (0)       81 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12044 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.450202 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.450202 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.450202 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.450202 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      310 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/iac.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/normalize.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/sast.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/sca.py
+-rw-r--r--   0 root         (0) root         (0)     3614 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/resources_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.450202 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.450202 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/schemas/mutations/
+-rw-r--r--   0 root         (0) root         (0)      607 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.450202 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/schemas/resolvers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/schemas/resolvers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.454202 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      790 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.454202 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      345 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/models/asset.py
+-rw-r--r--   0 root         (0) root         (0)      511 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/models/issues.py
+-rw-r--r--   0 root         (0) root         (0)      972 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/models/project.py
+-rw-r--r--   0 root         (0) root         (0)     6458 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/resources_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.454202 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.454202 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/schemas/mutations/
+-rw-r--r--   0 root         (0) root         (0)     1254 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.454202 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/schemas/resolvers/
+-rw-r--r--   0 root         (0) root         (0)     2352 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.454202 conviso-flowcli-2.1.6/convisoappsec/flow/source_code_scanner/
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/source_code_scanner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/source_code_scanner/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/source_code_scanner/scc.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/source_code_scanner/source_code_scanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.454202 conviso-flowcli-2.1.6/convisoappsec/flow/util/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/util/ci_provider.py
+-rw-r--r--   0 root         (0) root         (0)      480 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/util/metrics.py
+-rw-r--r--   0 root         (0) root         (0)      508 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/util/source_code_compressor.py
+-rw-r--r--   0 root         (0) root         (0)    14635 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/version_control_system_adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.454202 conviso-flowcli-2.1.6/convisoappsec/flow/version_searchers/
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/version_searchers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/version_searchers/timebased_version_seacher.py
+-rw-r--r--   0 root         (0) root         (0)      943 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/version_searchers/version_searcher_result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.454202 conviso-flowcli-2.1.6/convisoappsec/flow/versioning_style/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/versioning_style/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flow/versioning_style/semantic_versioning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.454202 conviso-flowcli-2.1.6/convisoappsec/flowcli/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       99 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.454202 conviso-flowcli-2.1.6/convisoappsec/flowcli/assets/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/assets/create.py
+-rw-r--r--   0 root         (0) root         (0)      310 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/assets/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/assets/ls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.454202 conviso-flowcli-2.1.6/convisoappsec/flowcli/ast/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/ast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8045 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/ast/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     5350 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.454202 conviso-flowcli-2.1.6/convisoappsec/flowcli/companies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/companies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      892 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/companies/ls.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.458202 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.458202 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      190 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/context.py
+-rw-r--r--   0 root         (0) root         (0)      677 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.458202 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      346 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.458202 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      194 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/context.py
+-rw-r--r--   0 root         (0) root         (0)      675 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.458202 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     2815 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py
+-rw-r--r--   0 root         (0) root         (0)     4681 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/values.py
+-rw-r--r--   0 root         (0) root         (0)      353 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)      763 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/ls.py
+-rw-r--r--   0 root         (0) root         (0)      970 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/show.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.458202 conviso-flowcli-2.1.6/convisoappsec/flowcli/findings/
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/findings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.458202 conviso-flowcli-2.1.6/convisoappsec/flowcli/findings/create/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/findings/create/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      269 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/findings/create/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.458202 conviso-flowcli-2.1.6/convisoappsec/flowcli/findings/create/with_/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/findings/create/with_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      309 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/findings/create/with_/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/findings/create/with_/version_tracker.py
+-rw-r--r--   0 root         (0) root         (0)      344 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/findings/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.458202 conviso-flowcli-2.1.6/convisoappsec/flowcli/findings/import_sarif/
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/findings/import_sarif/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7209 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/findings/import_sarif/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)      331 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/help_option.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.458202 conviso-flowcli-2.1.6/convisoappsec/flowcli/iac/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/iac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      241 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/iac/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    11269 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/iac/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.458202 conviso-flowcli-2.1.6/convisoappsec/flowcli/projects/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/projects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/projects/ls.py
+-rw-r--r--   0 root         (0) root         (0)     9438 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/requirements_verifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.458202 conviso-flowcli-2.1.6/convisoappsec/flowcli/sast/
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/sast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      245 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/sast/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    18807 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/sast/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.462202 conviso-flowcli-2.1.6/convisoappsec/flowcli/sca/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/sca/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      241 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/sca/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    10781 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/sca/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.462202 conviso-flowcli-2.1.6/convisoappsec/flowcli/vulnerability/
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/vulnerability/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4937 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/vulnerability/assert_security_rules.py
+-rw-r--r--   0 root         (0) root         (0)      386 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/vulnerability/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)      948 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/vulnerability/rules_schema.json
+-rw-r--r--   0 root         (0) root         (0)    16094 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/flowcli/vulnerability/run.py
+-rw-r--r--   0 root         (0) root         (0)      231 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.462202 conviso-flowcli-2.1.6/convisoappsec/sast/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/sast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/sast/decision.py
+-rw-r--r--   0 root         (0) root         (0)     8929 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/sast/sastbox.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/convisoappsec/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.446201 conviso-flowcli-2.1.6/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:03:50.462202 conviso-flowcli-2.1.6/scripts/shell_completer/
+-rw-r--r--   0 root         (0) root         (0)      624 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/scripts/shell_completer/flow_bash_completer.sh
+-rw-r--r--   0 root         (0) root         (0)      147 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/scripts/shell_completer/flow_fish_completer.fish
+-rw-r--r--   0 root         (0) root         (0)      844 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/scripts/shell_completer/flow_zsh_completer.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 13:03:50.462202 conviso-flowcli-2.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1883 2024-05-23 13:03:46.000000 conviso-flowcli-2.1.6/setup.py
```

### Comparing `conviso-flowcli-2.0.0rc9/conviso_flowcli.egg-info/SOURCES.txt` & `conviso-flowcli-2.1.6/conviso_flowcli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py
 convisoappsec/flow/graphql_api/beta/schemas/resolvers/__init__.py
 convisoappsec/flow/graphql_api/v1/__init__.py
 convisoappsec/flow/graphql_api/v1/client.py
 convisoappsec/flow/graphql_api/v1/resources_api.py
 convisoappsec/flow/graphql_api/v1/models/__init__.py
 convisoappsec/flow/graphql_api/v1/models/asset.py
+convisoappsec/flow/graphql_api/v1/models/issues.py
 convisoappsec/flow/graphql_api/v1/models/project.py
 convisoappsec/flow/graphql_api/v1/schemas/__init__.py
 convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py
 convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py
 convisoappsec/flow/source_code_scanner/__init__.py
 convisoappsec/flow/source_code_scanner/exceptions.py
 convisoappsec/flow/source_code_scanner/scc.py
@@ -109,13 +110,15 @@
 convisoappsec/flowcli/sast/run.py
 convisoappsec/flowcli/sca/__init__.py
 convisoappsec/flowcli/sca/entrypoint.py
 convisoappsec/flowcli/sca/run.py
 convisoappsec/flowcli/vulnerability/__init__.py
 convisoappsec/flowcli/vulnerability/assert_security_rules.py
 convisoappsec/flowcli/vulnerability/entrypoint.py
+convisoappsec/flowcli/vulnerability/rules_schema.json
+convisoappsec/flowcli/vulnerability/run.py
 convisoappsec/sast/__init__.py
 convisoappsec/sast/decision.py
 convisoappsec/sast/sastbox.py
 scripts/shell_completer/flow_bash_completer.sh
 scripts/shell_completer/flow_fish_completer.fish
 scripts/shell_completer/flow_zsh_completer.sh
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/common/box.py` & `conviso-flowcli-2.1.6/convisoappsec/common/box.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,15 +103,14 @@
             self.name, self.state
         ))
 
     def _on_pulling(self):
         self.logger.debug(RAW_STATE_MSG.format(
             self.name, self.state
         ))
-        self.logger.info('   Pulling {} image'.format(self.name))
         image = self.scanner.pull()
         if image:
             self.logger.debug('Image: {}'.format(image))
             self.next_state()
         else:
             raise RuntimeError("Image not found.")
 
@@ -121,20 +120,14 @@
         ))
         self.scanner.run()
         self.end_time = time.time()
         self.logger.debug('Total execution time for {} was {:2f}'.format(
             self.scanner.repository_name,
             self.end_time - self.start_time
         ))
-        status_code = self.scanner.wait()
-        self.logger.info('   Scanner {}@{} returned status code {}'.format(
-            self.scanner.repository_name,
-            self.name,
-            status_code
-        ))
         self.next_state()
 
     def _on_sending(self):
         self.logger.debug(RAW_STATE_MSG.format(
             self.name, self.state
         ))
         self.results = self.scanner.get_container_reports()
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/common/docker.py` & `conviso-flowcli-2.1.6/convisoappsec/common/docker.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/common/git_data_parser.py` & `conviso-flowcli-2.1.6/convisoappsec/common/git_data_parser.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/common/graphql/error_handlers.py` & `conviso-flowcli-2.1.6/convisoappsec/common/graphql/error_handlers.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/common/graphql/low_client.py` & `conviso-flowcli-2.1.6/convisoappsec/common/graphql/low_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from convisoappsec.common.graphql.error_handlers import GraphQlErrorHandler, RequestErrorHandler
 
 
 class GraphQLClient:
     DEFAULT_HEADERS = {
         'Accept': 'application/json',
         'Content-Type': 'application/json',
+        "User-Agent": "AST",
     }
 
     def __init__(self, url, headers={}):
         self.url = url
         self.__session = requests.Session()
         self.__session.headers.update(
             **self.DEFAULT_HEADERS,
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/api.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,26 +40,29 @@
 
 
 class Deploys(object):
     DIFF_CONTENT_FILE_NAME = 'diff_content.txt'
     DIFF_CONTENT_MIME_TYPE = 'text/plain'
     COMMIT_AUTHORS_FILE_NAME = 'commit_authors.yaml'
     COMMIT_AUTHORS_MIME_TYPE = 'text/yaml'
+    COMMIT_HISTORY_FILE_NAME = 'commit_history.yaml'
+    COMMIT_HISTORY_MIME_TYPE = 'text/yaml'
     ENDPOINT = '/api/v3/deploys'
     LIST_BY_PROJECT_ENPOINT = "api/v2/deploys/deploys_by_project_api_code"
 
     def __init__(self, client):
         self.client = client
 
     def create(self, project_code, **kargs):
         current_version = kargs.get('current_version')
         previous_version = kargs.get('previous_version')
         diff_content = kargs.get('diff_content')
         project_metrics = kargs.get('project_metrics')
         commit_authors = kargs.get('commit_authors')
+        commit_history = kargs.get('commit_history')
 
         files = {
             'api_code': (None, project_code),
 
             'deploy[current_version][commit]': (None, current_version.get('commit')),  # noqa: E501
             'deploy[current_version][tag]': (None, current_version.get('tag')),
 
@@ -101,18 +104,30 @@
                 self.COMMIT_AUTHORS_MIME_TYPE,
             )
 
             files.update({
                 'deploy[authors]': commit_authors_args,
             })
 
+        if commit_history:
+            commit_history_args = (
+                self.COMMIT_HISTORY_FILE_NAME,
+                commit_history,
+                self.COMMIT_HISTORY_MIME_TYPE,
+            )
+
+            files.update({
+                'deploy[commit_history]': commit_history_args,
+            })
+
         session = self.client.requests_session
         response = session.post(self.ENDPOINT, files=files)
 
         response.raise_for_status()
+
         return response.json()
 
     def list(self, project_code, current_tag=None):
         data = {
             'api_code': project_code,
         }
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/sast.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/sast.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,24 +10,26 @@
         first_line,
         title,
         description,
         severity,
         commit_ref,
         deploy_id,
         reference,
+        original_issue_id_from_tool,
     ):
         self.asset_id = asset_id
         self.severity = Normalize.normalize_severity(severity)
         self.title = title
         self.description = description
         self.code_snippet = code_snippet
         self.file_name = file_name
         self.vulnerable_line = int(vulnerable_line)
         self.first_line = int(first_line)
         self.reference = reference
+        self.original_issue_id_from_tool = original_issue_id_from_tool
 
         self.commit_ref = commit_ref
         self.deploy_id = str(deploy_id)
 
     def to_graphql_dict(self):
         """
         This function returns a dictionary containing various attributes of an
@@ -41,8 +43,9 @@
             "codeSnippet": self.code_snippet,
             "fileName": self.file_name,
             "vulnerableLine": int(self.vulnerable_line),
             "firstLine": int(self.first_line),
             "reference": self.reference,
             "commitRef": self.commit_ref,
             "deployId": str(self.deploy_id),
+            "originalIssueIdFromTool": str(self.original_issue_id_from_tool)
         }
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/models/issues/sca.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/sca.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 from convisoappsec.flow.graphql_api.beta.models.issues.normalize import Normalize
 
+
 class CreateScaFindingInput:
     def __init__(
-        self,
-        asset_id,
-        title,
-        description,
-        severity,
-        solution,
-        reference,
-        file_name,
-        affected_version,
-        package,
-        cve,
+            self,
+            asset_id,
+            title,
+            description,
+            severity,
+            solution,
+            reference,
+            file_name,
+            affected_version,
+            package,
+            cve,
+            original_issue_id_from_tool
     ):
         self.asset_id = asset_id
         self.title = title
         self.description = description
         self.severity = Normalize.normalize_severity(severity)
         self.solution = solution
         self.reference = reference
         self.file_name = file_name
         self.affected_version = affected_version
         self.package = package
+        self.original_issue_id_from_tool = original_issue_id_from_tool
 
         if type(cve) is list:
             self.cve = ' , '.join(cve)
         elif type(cve) is str:
             self.cve = cve
         else:
             self.cve = ""
 
     def to_graphql_dict(self):
         """
         This function returns a dictionary containing various attributes of an
         asset in a GraphQL format.
         """
         return {
-			"assetId": int(self.asset_id),
-			"title": self.title,
-			"description": self.description,
-			"severity": self.severity,
-			"solution": self.solution,
-			"reference": self.reference,
-			"fileName": self.file_name,
-			"affectedVersion": self.affected_version,
-			"package": self.package,
-			"cve": self.cve,
-		}
+            "assetId": int(self.asset_id),
+            "title": self.title,
+            "description": self.description,
+            "severity": self.severity,
+            "solution": self.solution,
+            "reference": self.reference,
+            "fileName": self.file_name,
+            "affectedVersion": self.affected_version,
+            "package": self.package,
+            "cve": self.cve,
+            "originalIssueIdFromTool": self.original_issue_id_from_tool
+        }
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/beta/resources_api.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/beta/resources_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,121 @@
-
 import jmespath
 from convisoappsec.flow.graphql_api.beta.models.issues.iac import CreateIacFindingInput
-
 from convisoappsec.flow.graphql_api.beta.models.issues.sast import CreateSastFindingInput
 from convisoappsec.flow.graphql_api.beta.models.issues.sca import CreateScaFindingInput
 from convisoappsec.flow.graphql_api.beta.schemas import mutations
+from convisoappsec.flow.graphql_api.v1.schemas import resolvers
+
 
 class IssuesAPI(object):
     """ To operations on Issues's (aka, findings and vulnerabilities)) in Conviso Platform. """
 
     def __init__(self, conviso_graphql_client):
         self.__conviso_graphql_client = conviso_graphql_client
 
     def create_sast(self, sast_issue_model: CreateSastFindingInput):
         graphql_variables = {
             "input": sast_issue_model.to_graphql_dict()
         }
-        
+
         graphql_body_response = self.__conviso_graphql_client.execute(
             mutations.CREATE_SAST_FINDING_INPUT,
             graphql_variables
         )
 
         expected_path = 'createSastFinding.issue'
 
         issue = jmespath.search(
             expected_path,
             graphql_body_response,
         )
 
         return issue
-    
+
     def create_sca(self, sca_issue_model: CreateScaFindingInput):
         graphql_variables = {
             "input": sca_issue_model.to_graphql_dict()
         }
-        
+
         graphql_body_response = self.__conviso_graphql_client.execute(
             mutations.CREATE_SCA_FINDING_INPUT,
             graphql_variables
         )
 
         expected_path = 'createScaFinding.issue'
 
         issue = jmespath.search(
             expected_path,
             graphql_body_response,
         )
 
         return issue
 
-
     def create_iac(self, issue_model: CreateIacFindingInput):
         graphql_variables = {
             "input": issue_model.to_graphql_dict()
         }
-        
+
         graphql_body_response = self.__conviso_graphql_client.execute(
             mutations.CREATE_SAST_FINDING_INPUT,
             graphql_variables
         )
 
         expected_path = 'createSastFinding.issue'
 
         issue = jmespath.search(
             expected_path,
             graphql_body_response,
         )
 
         return issue
+
+    def auto_close_vulnerabilities(self, company_id, asset_id, statuses, page=1, vulnerability_type=None):
+        """ entry point for auto closing vulnerabilities on conviso platform """
+        if vulnerability_type is None:
+            vulnerability_type = ['SAST_FINDING', 'SCA_FINDING']
+
+        graphql_variables = {
+            'company_id': company_id,
+            'asset_id': asset_id,
+            'page': page,
+            'per_page': 100,
+            'statuses': statuses,
+            'failure_types': vulnerability_type
+        }
+
+        graphql_body_response = self.__conviso_graphql_client.execute(
+            resolvers.GET_ISSUES_FINGERPRINT,
+            graphql_variables
+        )
+
+        expected_path = 'issues'
+
+        issues = jmespath.search(
+            expected_path,
+            graphql_body_response
+        )
+
+        return issues
+
+    def update_issue_status(self, issue_id, status):
+        """ Update issue status on conviso platform """
+
+        graphql_variables = {
+            'issueId': issue_id,
+            'status': status,
+            'reason': 'Status changed by Conviso AST.'
+        }
+
+        graphql_body_response = self.__conviso_graphql_client.execute(
+            mutations.UPDATE_ISSUE_STATUS,
+            graphql_variables
+        )
+
+        expected_path = 'changeIssueStatus.issue'
+
+        issue = jmespath.search(
+            expected_path,
+            graphql_body_response,
+        )
+
+        return issue
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/client.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/client.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/models/project.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/models/project.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-from datetime import datetime
+from datetime import datetime, timezone
+
 
 class CreateProjectInput:
     def __init__(self, company_id, asset_id, label):
         self.company_id = company_id
         self.asset_id = asset_id
         self.label = label
 
     def to_graphql_dict(self):
+        current_datetime = datetime.now(timezone.utc)
+        formatted_date = current_datetime.isoformat()
+
         return {
             "companyId": int(self.company_id),
             "assetsIds": int(self.asset_id),
             "label": self.label,
-            "startDate": str(datetime.now().isoformat()),
+            "startDate": str(formatted_date),
             "typeId": 33,
             "playbooksIds": 1,
             "goal": '',
             "scope": self.company_id
         }
 
+
 class UpdateProjectInput:
     def __init__(self, project_id, asset_id):
         self.project_id = project_id
         self.asset_id = asset_id
 
     def to_graphql_dict(self):
         return {
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/resources_api.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/resources_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,36 @@
         asset = jmespath.search(
             expected_path,
             graphql_body_response,
         )
 
         return asset
 
+    def update_asset(self, company_id, asset_id, asset_name, technologies):
+        graphql_variables = {
+            "id": asset_id,
+            "companyId": company_id,
+            "name": asset_name,
+            "tecnologyList": technologies
+        }
+
+        graphql_body_response = self.__conviso_graphql_client.execute(
+            mutations.UPDATE_ASSET,
+            graphql_variables
+        )
+
+        expected_path = 'updateAsset.asset'
+
+        asset = jmespath.search(
+            expected_path,
+            graphql_body_response,
+        )
+
+        return asset
+
     def get_by_company_id_or_name(self, company_id, asset_name, page, limit):
         graphql_variables = {
             "id": company_id,
             'name': asset_name,
             "page": page,
             "limit": limit
         }
@@ -82,14 +104,15 @@
         assets = jmespath.search(
             expected_path,
             graphql_body_response,
         )
 
         return assets
 
+
 class ProjectsApi(object):
     """ To operations on Project's resources in Conviso Platform. """
 
     def __init__(self, conviso_graphql_client):
         self.__conviso_graphql_client = conviso_graphql_client
 
     def create_project(self, project_input: CreateProjectInput):
@@ -136,14 +159,15 @@
         projects = jmespath.search(
             expected_path,
             graphql_body_response,
         )
 
         return projects
 
+
 class CompaniesApi(object):
     """ To operations on Companies resources in Conviso Platform. """
 
     def __init__(self, conviso_graphql_client):
         self.__conviso_graphql_client = conviso_graphql_client
 
     def get_company_by_id(self, company_id):
@@ -159,15 +183,14 @@
         expected_path = 'company'
         company = jmespath.search(
             expected_path,
             graphql_body_response,
         )
         return company
 
-
     def get_companies(self, page=1, limit=10):
         graphql_variables = {
             "page": page,
             "limit": limit
         }
 
         graphql_body_response = self.__conviso_graphql_client.execute(
@@ -180,26 +203,28 @@
         companies = jmespath.search(
             expected_path,
             graphql_body_response,
         )
 
         return companies
 
+
 class IssuesApi(object):
     """ To operations on Issue's resources in Conviso Platform. """
 
     def __init__(self, conviso_graphql_client):
         self.__conviso_graphql_client = conviso_graphql_client
 
-    def get_issues_stats(self, asset_id, company_id):
+    def get_issues_stats(self, asset_id, company_id, statuses):
         """ Return issue stats filter by asset and company """
 
         graphql_variables = {
             'asset_id': asset_id,
-            'company_id': company_id
+            'company_id': company_id,
+            'statuses': statuses
         }
 
         graphql_body_response = self.__conviso_graphql_client.execute(
             resolvers.GET_ISSUES_STATS,
             graphql_variables
         )
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,19 +32,21 @@
 }
 """
 
 GET_ISSUES_STATS = """
 query (
   $asset_id: [ID!],
   $company_id: ID!,
+  $statuses: [IssueStatusLabel!]
 ) {
   issuesStats(
     companyId: $company_id
     filters: {
       assetIds: $asset_id
+      statuses: $statuses
     }
   ) {
     severities {
       value
       count
     }
   }
@@ -112,7 +114,45 @@
       id
       label
       customFeatures
     }
   }
 }
 """
+
+GET_ISSUES_FINGERPRINT = """
+query GetIssuesFingerprint(
+    $company_id: ID!,
+    $page: Int,
+    $per_page: Int,
+    $asset_id: [ID!],
+    $statuses: [IssueStatusLabel!]
+    $failure_types: [Issue!]
+) {
+    issues(
+        companyId: $company_id,
+        pagination: {
+            page: $page,
+            perPage: $per_page
+        },
+        filters: {
+            assetIds: $asset_id,
+            statuses: $statuses,
+            failureTypes: $failure_types
+        }
+    ) {
+        collection {
+            id
+            type
+            ... on FindingInterface {
+                originalIssueIdFromTool
+                scanSource
+            }
+            status
+        }
+        metadata {
+            totalCount
+            totalPages
+        }
+    }
+}
+"""
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/source_code_scanner/scc.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/source_code_scanner/scc.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/source_code_scanner/source_code_scanner.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/source_code_scanner/source_code_scanner.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/util/ci_provider.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/util/ci_provider.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_control_system_adapter.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/version_control_system_adapter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import json
 import tempfile
 import re
 import yaml
+import git
 from contextlib import suppress
-
 from convisoappsec.logger import LOGGER
+from git.exc import GitCommandError
 
 
 class GitAdapter(object):
     LIST_OPTION = '--list'
     SORT_OPTION = '--sort'
     FORMAT_OPTION = '--format'
     ANCESTRY_PATH_OPTION = '--ancestry-path'
@@ -15,24 +17,91 @@
     OPTION_WITH_ARG_FMT = '{option}={value}'
     EMPTY_REPOSITORY_HASH = '4b825dc642cb6eb9a060e54bf8d69288fbee4904'
 
     def __init__(self, repository_dir='.', load_remote_repositories_heads=True, unshallow_repository=True):
         LOGGER.debug('Unshallow: {}'.format(unshallow_repository))
         LOGGER.debug('Load remote: {}'.format(load_remote_repositories_heads))
 
-        import git
         self._git_client = git.cmd.Git(repository_dir)
         self._first_commit = None
+        self._repo = git.Repo(repository_dir)
 
         if load_remote_repositories_heads:
             self.__load_remote_repositories_heads()
 
         if unshallow_repository:
             self.__unshallow_repository()
 
+    def get_commit_history(self):
+        """
+        Retrieves the commit history (including stashes) of the repository and saves it to a temporary JSON file.
+
+        Returns:
+            str: The path to the temporary JSON file.
+        """
+        commits = self._repo.iter_commits()
+
+        commit_info_list = [
+            {
+                'commit': commit.hexsha,
+                'author': "{author_name} <{author_email}>".format(
+                    author_name=commit.author.name, author_email=commit.author.email
+                ),
+                'date': commit.authored_datetime.strftime("%Y-%m-%d %H:%M:%S"),
+                'message': commit.message
+            }
+            for commit in commits
+        ]
+
+        # Include information about stashes
+        stashes = self._repo.git.stash("list", "--format=%H|%gd|%ci|%P|%gs", "--date=iso").splitlines()
+        stash_info_list = [
+            {
+                'commit': stash_info.split('|')[0],
+                'stash_ref': stash_info.split('|')[1],
+                'date': stash_info.split('|')[2],
+                'parent_commits': stash_info.split('|')[3].split(),
+                'message': stash_info.split('|')[4],
+                'contributors': self.get_contributors_for_stash_merge(stash_info.split('|')[0])
+            }
+            for stash_info in stashes
+        ]
+
+        commit_info_list.extend(stash_info_list)
+
+        temp_file = tempfile.NamedTemporaryFile(mode='w+', delete=False)
+        json.dump(commit_info_list, temp_file, indent=2)
+        temp_file.seek(0)
+
+        return temp_file
+
+    def get_contributors_for_stash_merge(self, stash_commit):
+        """
+        Get contributors involved in a stash merge.
+
+        Args:
+            stash_commit (str): The commit hash of the stash.
+
+        Returns:
+            list: List of contributors involved in the stash merge.
+        """
+        contributors = set()
+        stash_diff = self._repo.git.diff(stash_commit + "^", stash_commit, "--name-only").splitlines()
+
+        for file_path in stash_diff:
+            blame_output = self._repo.git.blame(stash_commit, "--", file_path).splitlines()
+            for line in blame_output:
+                commit_hash = line.split()[0]
+                contributor_name = (self._repo.git.show("-s", "--format=%aN|%ae", commit_hash)).split('|')[0]
+                contributor_email = (self._repo.git.show("-s", "--format=%aN|%ae", commit_hash)).split('|')[1]
+                contributor = "{name} {email}".format(name=contributor_name, email=contributor_email)
+                contributors.add(contributor)
+
+        return list(contributors)
+
     def tags(self, sort='-committerdate'):
         sort_option = self.OPTION_WITH_ARG_FMT.format(
             option=self.SORT_OPTION,
             value=sort,
         )
 
         args = (self.LIST_OPTION, sort_option)
@@ -44,37 +113,27 @@
         version = version or self.EMPTY_REPOSITORY_HASH
 
         if version == self.EMPTY_REPOSITORY_HASH:
             msg_fmt = """Creating diff comparing revision[{0}] and the repository beginning"""
             LOGGER.warning(msg_fmt.format(another_version))
 
         diff_file = tempfile.TemporaryFile()
-        self._git_client.diff(
-            version,
-            another_version,
-            output_stream=diff_file
-        )
+        self._git_client.diff(version, another_version, output_stream=diff_file)
 
         return diff_file
 
     def diff_stats(self, version, another_version):
         version = version or self.EMPTY_REPOSITORY_HASH
 
         if version == self.EMPTY_REPOSITORY_HASH:
             msg_fmt = """Creating diff stats comparing revision[{0}] and the repository beginning"""
             LOGGER.warning(msg_fmt.format(another_version))
 
         stats_output = tempfile.TemporaryFile()
-
-        self._git_client.diff(
-            version,
-            another_version,
-            '--numstat',
-            output_stream=stats_output
-        )
+        self._git_client.diff(version, another_version, '--numstat', output_stream=stats_output)
 
         stats_summary = GitDiffNumStatSummary.load(stats_output)
         stats_output.close()
 
         return stats_summary
 
     @property
@@ -189,17 +248,15 @@
 
         return author_data
 
     def get_commits_by_range(self, start_commit, end_commit):
         tmp_commits = tempfile.TemporaryFile()
 
         self._git_client.rev_list(
-            self.ANCESTRY_PATH_OPTION,
-            start_commit + '..' + end_commit,
-            output_stream=tmp_commits
+            self.ANCESTRY_PATH_OPTION, start_commit + '..' + end_commit, output_stream=tmp_commits
         )
 
         return _read_file_lines_generator(tmp_commits)
 
     def get_commit_authors_by_range(self, start_commit, end_commit):
         start_commit_range = start_commit
         author_file = CommitAuthorFile()
@@ -223,16 +280,14 @@
     def remote_repositories_name(self):
         args = ("show")
         client_output = self._git_client.remote(args)
         repositories = client_output.splitlines()
         return repositories
 
     def __load_remote_repositories_heads(self):
-        from git.exc import GitCommandError
-
         heads_refspec_format = "refs/heads/*:refs/remotes/{remote_repository_name}/*"
 
         for remote_repository_name in self.remote_repositories_name:
             try:
                 heads_refspec = heads_refspec_format.format(
                     remote_repository_name=remote_repository_name
                 )
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/timebased_version_seacher.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/version_searchers/timebased_version_seacher.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/version_searchers/version_searcher_result.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/version_searchers/version_searcher_result.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flow/versioning_style/semantic_versioning.py` & `conviso-flowcli-2.1.6/convisoappsec/flow/versioning_style/semantic_versioning.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/assets/create.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/assets/create.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/assets/ls.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/assets/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/ast/entrypoint.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/ast/entrypoint.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-from copy import deepcopy as clone
-
 import click
+import git
 from convisoappsec.flowcli import help_option
-from convisoappsec.flowcli.common import CreateDeployException, DeployFormatter, PerformDeployException, project_code_option, asset_id_option
+from convisoappsec.flowcli.common import CreateDeployException, DeployFormatter, PerformDeployException, \
+    project_code_option, asset_id_option
 from convisoappsec.flowcli.deploy.create.context import pass_create_context
 from convisoappsec.flowcli.deploy.create.with_.values import values
 from convisoappsec.flowcli.requirements_verifier import RequirementsVerifier
 from convisoappsec.flowcli.sast import sast
 from convisoappsec.flowcli.sca import sca
+from convisoappsec.flowcli.iac import iac
+from convisoappsec.flowcli.vulnerability import vulnerability
 from convisoappsec.logger import LOGGER
+from copy import deepcopy as clone
+
 
 def get_default_params_values(cmd_params):
     """ Further information in https://click.palletsprojects.com/en/8.1.x/api/?highlight=params#click.Command.params
 
     Args:
         cmd_params (List[click.core.Parameter]):
 
@@ -44,15 +48,15 @@
     return parsed_params
 
 
 def perform_sast(context) -> None:
     """Setup and runs the "sast run" command.
 
     Args:
-        context (<class 'click.core.Context'>): clonned context
+        context (<class 'click.core.Context'>): cloned context
     """
     sast_run = sast.commands.get('run')
 
     specific_params = {
         "deploy_id": context.obj.deploy['id'],
         "start_commit": context.obj.deploy['previous_commit'],
         "end_commit": context.obj.deploy['current_commit'],
@@ -70,15 +74,15 @@
         raise click.ClickException(str(err)) from err
 
 
 def perform_sca(context) -> None:
     """Setup and runs the "sca run" command.
 
     Args:
-        context (<class 'click.core.Context'>): clonned context
+        context (<class 'click.core.Context'>): cloned context
     """
     sca_run = sca.commands.get('run')
     context.params.update({"deploy_id": context.obj.deploy['id']})
     context.params = parse_params(context.params, sca_run.params)
     try:
         LOGGER.info(
             'Running SCA on deploy ID "{deploy_id}"'
@@ -86,14 +90,52 @@
         )
         sca_run.invoke(context)
 
     except Exception as err:
         raise click.ClickException(str(err)) from err
 
 
+def perform_iac(context) -> None:
+    """Setup and runs the "iac run" command.
+
+    Args:
+        context (<class 'click.core.Context'>): clonned context
+    """
+    iac_run = iac.commands.get('run')
+    context.params.update({"deploy_id": context.obj.deploy['id']})
+    context.params = parse_params(context.params, iac_run.params)
+
+    try:
+        LOGGER.info(
+            'Running IAC on deploy ID "{deploy_id}"'
+            .format(deploy_id=context.params["deploy_id"])
+        )
+        iac_run.invoke(context)
+    except Exception as err:
+        raise click.ClickException(str(err)) from err
+
+
+def perform_vulnerabilities_service(context) -> None:
+    auto_close_run = vulnerability.commands.get('run')
+
+    specific_params = {
+        "deploy_id": context.obj.deploy['id'],
+        "start_commit": context.obj.deploy['previous_commit'],
+        "end_commit": context.obj.deploy['current_commit'],
+    }
+    context.params.update(specific_params)
+    context.params = parse_params(context.params, auto_close_run.params)
+
+    try:
+        LOGGER.info("[*] Verifying if any vulnerability was fixed ...")
+        auto_close_run.invoke(context)
+    except Exception as err:
+        raise click.ClickException(str(err)) from err
+
+
 def perform_deploy(context):
     """Setup and runs the "deploy create with values" command.
 
     Args:
         context (<class 'click.core.Context'>): clonned context
 
     Returns:
@@ -121,14 +163,15 @@
 
     except CreateDeployException as err:
         raise PerformDeployException(err)
 
     except Exception as err:
         raise click.ClickException(str(err)) from err
 
+
 @click.command(
     context_settings=dict(
         allow_extra_args=True,
         ignore_unknown_options=True
     )
 )
 @asset_id_option(
@@ -172,24 +215,41 @@
 )
 @click.option(
     "--company-id",
     required=False,
     envvar=("CONVISO_COMPANY_ID", "FLOW_COMPANY_ID"),
     help="Company ID on Conviso Platform",
 )
+@click.option(
+    '--asset-name',
+    required=False,
+    envvar=("CONVISO_ASSET_NAME", "FLOW_ASSET_NAME"),
+    help="Provides a asset name.",
+)
+@click.option(
+    '--vulnerability-auto-close',
+    default=False,
+    is_flag=True,
+    hidden=True,
+    help="Enable auto fixing vulnerabilities on cp.",
+)
 @help_option
 @pass_create_context
 @click.pass_context
 def run(context, create_context, **kwargs):
     """ AST - Application Security Testing. Unifies deploy issue, SAST and SCA analyses.  """
     try:
         prepared_context = RequirementsVerifier.prepare_context(clone(context), from_ast=True)
         prepared_context.obj.deploy = perform_deploy(clone(prepared_context))
         perform_sast(clone(prepared_context))
         perform_sca(clone(prepared_context))
+        perform_iac(clone(prepared_context))
+
+        if context.params['vulnerability_auto_close'] is True:
+            perform_vulnerabilities_service(clone(prepared_context))
 
     except PerformDeployException as err:
         LOGGER.warning(err)
 
     except Exception as err:
         raise click.ClickException(str(err)) from err
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/common.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/common.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/companies/ls.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/companies/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/context.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/context.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/entrypoint.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/create/with_/values.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/create/with_/values.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,15 +74,14 @@
         project_code = prepared_context.params['project_code']
 
     try:
         flow = flow_context.create_conviso_rest_api_client()
         git_adapter = GitAdapter(repository_dir)
 
         current_commit = current_commit or git_adapter.head_commit
-
         if not previous_commit:
             try:
                 latest_deploy = flow.deploys.get_latest(project_code)
                 previous_commit = latest_deploy.get('current_commit')
 
                 if not previous_commit:
                     previous_tag = latest_deploy.get('current_tag')
@@ -120,22 +119,25 @@
         LOGGER.debug(deploy_metrics_msg_fmt.format(
             previous_commit, current_commit))
         LOGGER.debug('Deploy metrics: {}'.format(deploy_metrics))
 
         project_metrics_data = project_metrics(repository_dir)
         LOGGER.debug('Project metrics: {}'.format(project_metrics_data))
 
+        commit_history = git_adapter.get_commit_history()
+
         deploy = flow.deploys.create(
             project_code,
             current_version={'commit': current_commit},
             previous_version={'commit': previous_commit},
             diff_content=diff_content,
             metrics=deploy_metrics,
             project_metrics=project_metrics_data,
-            commit_authors=authors_data
+            commit_authors=authors_data,
+            commit_history=commit_history
         )
 
         click.echo(
             create_context.output_formatter.format(deploy)
         )
         return deploy
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/ls.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/deploy/show.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/deploy/show.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/entrypoint.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/create/with_/version_tracker.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/findings/create/with_/version_tracker.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/findings/import_sarif/entrypoint.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/findings/import_sarif/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/iac/run.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/iac/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,37 +83,31 @@
 @click.option(
     "--company-id",
     required=False,
     envvar=("CONVISO_COMPANY_ID", "FLOW_COMPANY_ID"),
     help="Company ID on Conviso Platform",
 )
 @click.option(
+    '--asset-name',
+    required=False,
+    envvar=("CONVISO_ASSET_NAME", "FLOW_ASSET_NAME"),
+    help="Provides a asset name.",
+)
+@click.option(
     '--from-ast',
     default=False,
     is_flag=True,
     hidden=True,
     help="Internal use only.",
 )
 @help_option
 @pass_flow_context
 @click.pass_context
-def run(
-        context,
-        flow_context,
-        project_code,
-        asset_id,
-        company_id,
-        repository_dir,
-        send_to_flow,
-        scanner_timeout,
-        parallel_workers,
-        deploy_id,
-        experimental,
-        from_ast
-):
+def run(context, flow_context, project_code, asset_id, company_id, repository_dir, send_to_flow, scanner_timeout,
+        parallel_workers, deploy_id, experimental, asset_name, from_ast):
     """
       This command will perform IAC analysis at the source code. The analysis
       results can be reported or not to flow application.
     """
     context.params['company_id'] = company_id if company_id is not None else None
 
     if not from_ast:
@@ -138,16 +132,15 @@
         context.params['scanner_timeout'],
         context.params['parallel_workers'],
         context.params['deploy_id'],
         context.params['experimental'],
     )
 
 
-def deploy_results_to_conviso(
-        conviso_api, results_filepaths, project_code, deploy_id, repository_dir, token, scanner_timeout):
+def deploy_results_to_conviso(conviso_api, results_filepaths, project_code, deploy_id, repository_dir, token, scanner_timeout):
     results_context = click.progressbar(
         results_filepaths, label="Sending SASTBox reports to Conviso Platform"
     )
 
     with results_context as reports:
         for report_name in reports:
             compatible_report_filepath = convert_sarif_to_sastbox1(
@@ -182,26 +175,28 @@
             )
 
             with open(compatible_report_filepath) as report_file:
                 report_content = json.load(report_file)
 
                 issues = report_content.get("issues", [])
                 for issue in issues:
+                    hash_issue = issue.get('hash_issue_v2', [])
                     issue_model = CreateIacFindingInput(
                         asset_id=asset_id,
                         file_name=issue.get("filename"),
                         vulnerable_line=issue.get("line"),
                         title=issue.get("title"),
                         description=issue.get("description"),
                         severity=issue.get("severity"),
                         deploy_id=deploy_id,
                         code_snippet=parse_code_snippet(issue.get("evidence")),
                         reference=parse_conviso_references(issue.get("references")),
                         first_line=parse_first_line_number(issue.get("evidence")),
-                        commit_ref=commit_ref
+                        commit_ref=commit_ref,
+                        original_issue_id_from_tool=hash_issue,
                     )
 
                     try:
                         conviso_api.issues.create_iac(issue_model)
                     except ReponseError as error:
                         if error.code == 'RECORD_NOT_UNIQUE':
                             duplicated_issues += 1
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/projects/ls.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/projects/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/requirements_verifier.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/requirements_verifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,33 +67,54 @@
         """ assignment asset when is a sarif import """
         context.params['asset_id'] = asset['id']
         context.params['experimental'] = True
 
         return context
 
     @staticmethod
-    def find_or_create_asset(company_id, old_name, new_name):
+    def find_or_create_asset(context, company_id, old_name, new_name):
         """ Method to find or create asset on conviso platform """
         try:
             existing_assets = RequirementsVerifier.list_assets(company_id, new_name, 'SAST')
             if not existing_assets:
                 existing_assets = RequirementsVerifier.list_assets(company_id, old_name, 'SAST')
-            if existing_assets:
-                LOGGER.info('Asset found ...')
-                return existing_assets
-            else:
-                LOGGER.info('Asset not found creating ...')
-                new_asset = RequirementsVerifier.create_asset(company_id, new_name, 'SAST')
-                return [new_asset]
+            for asset in existing_assets:
+                if asset['name'] == old_name or asset['name'] == new_name:
+                    LOGGER.info('Asset found ...')
+                    context.params['asset_name'] = asset['name']
+                    return [asset]
+            LOGGER.info('Asset not found creating ...')
+            new_asset = RequirementsVerifier.create_asset(company_id, new_name, 'SAST')
+            context.params['asset_name'] = new_name
+            return [new_asset]
         except Exception as e:
-            raise "Error: {}".format(e)
+            raise Exception("Error: {}".format(e))
+
+    @staticmethod
+    def create_asset_with_custom_name(context, company_id, asset_name):
+        """ Create an asset with custom name pass with a custom name """
+
+        # we need to verify if already has an asset with the name provided.
+        # because graphql will return an error if already has.
+        existing_asset = RequirementsVerifier.list_assets(company_id, asset_name, 'SAST')
+
+        if not existing_asset:
+            LOGGER.info("Asset not found creating with name {} ...".format(asset_name))
+            asset = RequirementsVerifier.create_asset(company_id, asset_name, 'SAST')
+        else:
+            LOGGER.info('Asset found ...')
+            asset = existing_asset[0]
+
+        context.params['asset_name'] = asset_name
+
+        return asset
 
     @staticmethod
     def find_or_create_project(context, project_label, company_id, asset_id):
-        """ find or create a project to perform a deploy """
+        """ find or create a project to perform a deployment """
         projects = Projects()
         existing_project = projects.ls(flow_context=context, project_label=project_label, company_id=company_id)
 
         if not existing_project:
             project = RequirementsVerifier.create_project(company_id, asset_id, project_label)
             return [project]
         elif len(existing_project) > 1:
@@ -176,20 +197,25 @@
             company = companies_filtered[0]
             company_id = company['id']
 
             if new_management_flag not in company['customFeatures']:
                 error_msg = "Deploy not created. The company '{}' does not have access to the new vulnerability management".format(company['label'])
                 raise CreateDeployException(error_msg)
 
-            pattern = r"\([^)]*\)"  # eliminating what is in parentheses
-            old_asset_name = GitDataParser(context.params['repository_dir']).parse_name()
-            new_asset_name = re.sub(pattern, '', old_asset_name).strip()
+            if context.params['asset_name'] is not None:
+                # if user use --asset-name param or envvar CONVISO_ASSET_NAME, FLOW_ASSET_NAME
+                asset_name = context.params['asset_name']
+                asset = RequirementsVerifier.create_asset_with_custom_name(context, company_id, asset_name)
+            else:
+                pattern = r"\([^)]*\)"  # eliminating what is in parentheses
+                old_asset_name = GitDataParser(context.params['repository_dir']).parse_name()
+                new_asset_name = re.sub(pattern, '', old_asset_name).strip()
 
-            assets = RequirementsVerifier.find_or_create_asset(company_id, old_asset_name, new_asset_name)
-            asset = assets[0]
+                assets = RequirementsVerifier.find_or_create_asset(context, company_id, old_asset_name, new_asset_name)
+                asset = assets[0]
 
             if 'input_file' in context.params:
                 # sarif only uses assets, not requiring the creation of a project.
                 RequirementsVerifier.sarif_asset_assignment(context, asset)
 
                 return context
 
@@ -203,9 +229,10 @@
                 project_code = project['apiCode']
             else:
                 project_code = asset['projects'][0]['apiCode']
 
             context.params['project_code'] = project_code
             context.params['asset_id'] = asset['id']
             context.params['experimental'] = True
+            context.params['company_id'] = company_id
 
             return context
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sast/run.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/sast/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import sys
 import click
+import traceback
 from json import load as json_load
 from copy import deepcopy as clone
 from base64 import b64decode
 from re import search as regex_search
 from convisoappsec.flow import GitAdapter
 from convisoappsec.flow.graphql_api.beta.models.issues.sast import (CreateSastFindingInput)
 from convisoappsec.flowcli import help_option
 from convisoappsec.flowcli.common import (asset_id_option, on_http_error, project_code_option)
 from convisoappsec.flowcli.context import pass_flow_context
 from convisoappsec.sast.decision import Decision, Severity
 from convisoappsec.sast.sastbox import SASTBox
 from convisoappsec.common.graphql.errors import ReponseError
 from convisoappsec.flowcli.requirements_verifier import RequirementsVerifier
-from convisoappsec.flowcli.findings import import_sarif
 
 
 def log_func(msg, new_line=True, clear=False):
     click.echo(msg, nl=new_line, err=True)
 
 
 def find_blocked_issues(
-    results_filepaths, overall_threshold, severity_threshold, severity
+        results_filepaths, overall_threshold, severity_threshold, severity
 ):
     blocked_issues = []
 
     for result_path in results_filepaths:
         report_decision = Decision(result_path)
 
         overall_policy = report_decision.block_from_findings(overall_threshold)
@@ -56,63 +56,69 @@
                     line_index=issue["line"],
                 )
             )
     pass
 
 
 def perform_sastbox_scan(
-    conviso_rest_api,
-    sastbox_registry,
-    sastbox_repository_name,
-    sastbox_tag,
-    sastbox_skip_login,
-    repository_dir,
-    end_commit,
-    start_commit,
-    logger,
+        conviso_rest_api,
+        sastbox_registry,
+        sastbox_repository_name,
+        sastbox_tag,
+        sastbox_skip_login,
+        repository_dir,
+        end_commit,
+        start_commit,
+        logger,
 ):
     sastbox = SASTBox(
         registry=sastbox_registry,
         repository_name=sastbox_repository_name,
         tag=sastbox_tag,
     )
 
     token = conviso_rest_api.docker_registry.get_sast_token()
 
     if not sastbox_skip_login:
-        logger("Checking SASTBox authorization...")
+        logger("Checking SAST authorization...")
         sastbox.login(token)
 
     pull_progress_bar = click.progressbar(
         length=sastbox.size,
-        label="Performing SASTBox download...",
+        label="Performing SAST download...",
     )
 
     with pull_progress_bar as progressbar:
         for downloaded_chunk in sastbox.pull():
             progressbar.update(downloaded_chunk)
 
-    logger("Starting SASTBox scandiff...")
+    logger("Starting SAST scandiff...")
 
     reports = sastbox.run_scan_diff(
         repository_dir, end_commit, start_commit, log=logger, token=token
     )
 
-    logger("SASTBox scandiff done")
+    logger("SAST scandiff done")
 
-    results_filepaths = [str(r) for r in reports]
+    results_filepaths = []
+    for r in reports:
+        try:
+            file_path = str(r)
+            results_filepaths.append(file_path)
+        except Exception as e:
+            click.echo(f"Error decoding file path: {r} with error {e}", file=sys.stderr)
 
     return results_filepaths
 
 
 def deploy_results_to_conviso(
-    conviso_api, results_filepaths, project_code, deploy_id=None, commit_refs=None
+        conviso_api, results_filepaths, project_code, deploy_id=None, commit_refs=None
 ):
     results_context = click.progressbar(
-        results_filepaths, label="Sending SASTBox reports to Conviso Platform"
+        results_filepaths, label="Sending SAST reports to Conviso Platform"
     )
 
     with results_context as reports:
         for report_name in reports:
             report_file = open(report_name)
 
             default_report_type = "sast"
@@ -138,30 +144,44 @@
         if reference:
             references_to_join.append(reference)
 
     return divider.join(references_to_join)
 
 
 def parse_code_snippet(encoded_base64):
-    decoded_text = b64decode(encoded_base64).decode("utf-8")
+    try:
+        decoded_text = b64decode(encoded_base64).decode("utf-8")
+    except UnicodeDecodeError:
+        try:
+            decoded_text = b64decode(encoded_base64, validate=False).decode("latin-1")
+        except Exception as e:
+            print("Error handling decoding error:", e, file=sys.stderr)
+            decoded_text = ''
 
     lines = decoded_text.split("\n")
 
     cleaned_lines = []
     for line in lines:
         cleaned_line = line.split(": ", 1)[-1]
         cleaned_lines.append(cleaned_line)
 
     code_snippet = "\n".join(cleaned_lines)
 
     return code_snippet
 
 
 def parse_first_line_number(encoded_base64):
-    decoded_text = b64decode(encoded_base64).decode("utf-8")
+    try:
+        decoded_text = b64decode(encoded_base64).decode("utf-8")
+    except UnicodeDecodeError:
+        try:
+            decoded_text = b64decode(encoded_base64, validate=False).decode("latin-1")
+        except Exception as e:
+            print("Error handling decoding error:", e, file=sys.stderr)
+            decoded_text = ''
 
     regex = r"^(\d+):"
 
     result = regex_search(regex, decoded_text)
 
     if result and result.group(1):
         return result.group(1)
@@ -169,57 +189,105 @@
     line_number_when_not_found = 1
     return line_number_when_not_found
 
 
 def deploy_results_to_conviso_beta(
     flow_context, conviso_api, results_filepaths, asset_id, commit_ref=None, deploy_id=None
 ):
-    file_path = results_filepaths[0]  # sastbox v2 unify all results in one file
-    # the way it was decided to import perform_command was to make it more explicit where it comes from
-    converted_results = [import_sarif.entrypoint.perform_command(flow_context, file_path, internal=True)]
 
     results_context = click.progressbar(
-        converted_results, label="Sending SASTBox reports to Conviso Platform"
+        results_filepaths, label="Sending SAST reports to Conviso Platform"
     )
 
     duplicated_issues = 0
 
     with results_context as reports:
         for report_path in reports:
             report_file = open(report_path)
             report_content = json_load(report_file)
             issues = report_content.get("issues", [])
+            issues_not_in_cp = hash_issues_from_cp(conviso_api, issues)
+
+            for issue in issues_not_in_cp:
+                hash_issue = issue.get("hash_issue")
+
+                if hash_issue == '':
+                    hash_issue = issue.get("hash_issue_v2")
 
-            for issue in issues:
                 issue_model = CreateSastFindingInput(
                     asset_id=asset_id,
                     file_name=issue.get("filename"),
                     vulnerable_line=issue.get("line"),
                     title=issue.get("title"),
                     description=issue.get("description"),
                     severity=issue.get("severity"),
                     commit_ref=commit_ref,
                     deploy_id=deploy_id,
                     code_snippet=parse_code_snippet(issue.get("evidence")),
                     reference=parse_conviso_references(issue.get("references")),
                     first_line=parse_first_line_number(issue.get("evidence")),
+                    original_issue_id_from_tool=hash_issue,
                 )
 
                 try:
                     conviso_api.issues.create_sast(issue_model)
                 except ReponseError as error:
                     if error.code == 'RECORD_NOT_UNIQUE':
                         duplicated_issues += 1
                     else:
                         raise error
 
-    msg = "\U0001F4AC %s Issue/Issues ignored during duplication" % duplicated_issues
+    msg = "\U0001F4AC %s Issue/Issues already on conviso platform due internal validation." % duplicated_issues
     log_func(msg)
 
 
+@click.pass_context
+def hash_issues_from_cp(context, conviso_api, issues):
+    """ Get hash issues from issues on conviso platform """
+    company_id = context.params['company_id']
+    asset_id = context.params['asset_id']
+
+    page = 1
+    original_issue_ids = []
+    try:
+        while True:
+            issues_from_cp = conviso_api.issues.auto_close_vulnerabilities(
+                company_id=company_id, asset_id=asset_id, statuses=None, vulnerability_type='SAST_FINDING'
+            )
+            total_pages = issues_from_cp['metadata']['totalPages']
+            issues_collection = issues_from_cp['collection']
+            issues_collection = [item for item in issues_collection if item['scanSource'] == 'conviso_scanner']
+
+            original_issue_ids.extend([item['originalIssueIdFromTool'] for item in issues_collection])
+
+            if total_pages == page:
+                break
+            else:
+                page += 1
+
+        log_func(
+            "\U0001F4AC %s vulnerability/vulnerabilities already on conviso platform." % len(original_issue_ids)
+        )
+
+        data = []
+        for item in issues:
+            if item['hash_issue'] != '' and item['hash_issue'] not in original_issue_ids:
+                data.append(item)
+            elif item['hash_issue'] == '' and item['hash_issue_v2'] not in original_issue_ids:
+                data.append(item)
+
+        log_func(
+            "\U0001F4AC %s New vulnerability/vulnerabilities founded." % len(data)
+        )
+
+        return data
+    except Exception as error:
+        raise error
+
+
 @click.command()
 @project_code_option(required=False)
 @asset_id_option(required=False)
 @click.option(
     "-s",
     "--start-commit",
     required=False,
@@ -277,15 +345,15 @@
     envvar=("CONVISO_DEPLOY_ID", "FLOW_DEPLOY_ID")
 )
 @click.option(
     "--sastbox-registry",
     default="",
     required=False,
     hidden=True,
-    envvar=("CONVISO_SASTBOX_REGISTRY","FLOW_SASTBOX_REGISTRY"),
+    envvar=("CONVISO_SASTBOX_REGISTRY", "FLOW_SASTBOX_REGISTRY"),
 )
 @click.option(
     "--sastbox-repository-name",
     default="",
     required=False,
     hidden=True,
     envvar=("CONVISO_SASTBOX_REPOSITORY_NAME", "FLOW_SASTBOX_REPOSITORY_NAME"),
@@ -314,42 +382,57 @@
 @click.option(
     "--company-id",
     required=False,
     envvar=("CONVISO_COMPANY_ID", "FLOW_COMPANY_ID"),
     help="Company ID on Conviso Platform",
 )
 @click.option(
+    '--asset-name',
+    required=False,
+    envvar=("CONVISO_ASSET_NAME", "FLOW_ASSET_NAME"),
+    help="Provides a asset name.",
+)
+@click.option(
+    '--vulnerability-auto-close',
+    default=False,
+    is_flag=True,
+    hidden=True,
+    help="Enable auto fixing vulnerabilities on cp.",
+)
+@click.option(
     '--from-ast',
     default=False,
     is_flag=True,
     hidden=True,
     help="Internal use only.",
 )
 @help_option
 @pass_flow_context
 @click.pass_context
 def run(
-    context,
-    flow_context,
-    project_code,
-    asset_id,
-    company_id,
-    end_commit,
-    start_commit,
-    repository_dir,
-    send_to_flow,
-    deploy_id,
-    sastbox_registry,
-    sastbox_repository_name,
-    sastbox_tag,
-    sastbox_skip_login,
-    fail_on_threshold,
-    fail_on_severity_threshold,
-    experimental,
-    from_ast
+        context,
+        flow_context,
+        project_code,
+        asset_id,
+        company_id,
+        end_commit,
+        start_commit,
+        repository_dir,
+        send_to_flow,
+        deploy_id,
+        sastbox_registry,
+        sastbox_repository_name,
+        sastbox_tag,
+        sastbox_skip_login,
+        fail_on_threshold,
+        fail_on_severity_threshold,
+        experimental,
+        asset_name,
+        vulnerability_auto_close,
+        from_ast
 ):
     """
     This command will perform SAST analysis at the source code. The analysis
     results can be reported or not to flow application. The analysis can be
     applied to specific commit range.
 
     This command will write the analysis reports files paths to stdout.
@@ -357,23 +440,23 @@
     context.params['company_id'] = company_id if company_id is not None else None
 
     if not from_ast:
         prepared_context = RequirementsVerifier.prepare_context(clone(context))
 
         params_to_copy = [
             'project_code', 'asset_id', 'start_commit', 'end_commit',
-            'repository_dir', 'send_to_flow', 'deploy_id',
-            'sastbox_registry', 'sastbox_repository_name', 'sastbox_tag',
-            'sastbox_skip_login', 'experimental'
+            'repository_dir', 'send_to_flow', 'deploy_id', 'sastbox_registry',
+            'sastbox_repository_name', 'sastbox_tag', 'sastbox_skip_login',
+            'experimental', 'asset_name', 'vulnerability_auto_close', 'company_id'
         ]
 
         for param_name in params_to_copy:
             context.params[param_name] = (
-                locals()[param_name] or prepared_context.params[param_name]
-                )
+                    locals()[param_name] or prepared_context.params[param_name]
+            )
 
     perform_command(
         flow_context,
         context.params['project_code'],
         context.params['asset_id'],
         context.params['end_commit'],
         context.params['start_commit'],
@@ -382,36 +465,37 @@
         context.params['deploy_id'],
         context.params['sastbox_registry'],
         context.params['sastbox_repository_name'],
         context.params['sastbox_tag'],
         context.params['sastbox_skip_login'],
         context.params['fail_on_threshold'],
         context.params['fail_on_severity_threshold'],
-        context.params['experimental']
+        context.params['experimental'],
+        context.params['company_id']
     )
 
 
 def perform_command(
-    flow_context,
-    project_code,
-    asset_id,
-    end_commit,
-    start_commit,
-    repository_dir,
-    send_to_flow,
-    deploy_id,
-    sastbox_registry,
-    sastbox_repository_name,
-    sastbox_tag,
-    sastbox_skip_login,
-    fail_on_threshold,
-    fail_on_severity_threshold,
-    experimental
+        flow_context,
+        project_code,
+        asset_id,
+        end_commit,
+        start_commit,
+        repository_dir,
+        send_to_flow,
+        deploy_id,
+        sastbox_registry,
+        sastbox_repository_name,
+        sastbox_tag,
+        sastbox_skip_login,
+        fail_on_threshold,
+        fail_on_severity_threshold,
+        experimental,
+        company_id
 ):
-
     if send_to_flow and not experimental and not project_code:
         raise click.MissingParameter(
             "It is required when sending reports to Conviso Platform API.",
             param_type="option",
             param_hint="--project-code",
         )
 
@@ -430,59 +514,58 @@
             "{} is not a valid Severity. Use a valid Severity value:\n{}".format(
                 severity, [severity.name for severity in Severity]
             ),
             param_hint="--fail-on-severity-threshold",
         )
 
     try:
-        git_adapater = GitAdapter(repository_dir)
+        git_adapter = GitAdapter(repository_dir)
 
-        end_commit = end_commit or git_adapater.head_commit
+        end_commit = end_commit or git_adapter.head_commit
 
-        start_commit = start_commit or git_adapater.empty_repository_tree_commit
+        start_commit = start_commit or git_adapter.empty_repository_tree_commit
 
         if start_commit == end_commit:
             click.echo(
                 "Previous commit ({0}) and Current commit ({1}) are the same, nothing to do.".format(
                     start_commit, end_commit
                 ),
                 file=sys.stderr,
             )
             return
 
         conviso_rest_api = flow_context.create_conviso_rest_api_client()
+        conviso_beta_api = flow_context.create_conviso_api_client_beta()
 
         results_filepaths = perform_sastbox_scan(
             conviso_rest_api,
             sastbox_registry,
             sastbox_repository_name,
             sastbox_tag,
             sastbox_skip_login,
             repository_dir,
             end_commit,
             start_commit,
             log_func,
         )
 
         if send_to_flow:
-            commit_refs = git_adapater.show_commit_refs(end_commit)
-
             if experimental:
-                conviso_beta_api = flow_context.create_conviso_api_client_beta()
-
                 deploy_results_to_conviso_beta(
                     flow_context,
                     conviso_beta_api,
                     results_filepaths,
                     asset_id,
                     commit_ref=end_commit,
-                    deploy_id=deploy_id,
+                    deploy_id=deploy_id
                 )
 
             else:
+                commit_refs = git_adapter.show_commit_refs(end_commit)
+
                 deploy_results_to_conviso(
                     conviso_rest_api,
                     results_filepaths,
                     project_code,
                     deploy_id,
                     commit_refs,
                 )
@@ -492,14 +575,15 @@
         )
 
         if blocked_issues:
             print_blocked_issues(blocked_issues)
             sys.exit(1)
 
     except Exception as e:
+        traceback.print_exc()
         on_http_error(e)
         raise click.ClickException(str(e)) from e
 
 
 EPILOG = """
 Examples:
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/sca/run.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/sca/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 )
 from convisoappsec.flowcli.context import pass_flow_context
 from convisoappsec.logger import LOGGER
 from convisoappsec.common.graphql.errors import ReponseError
 from convisoappsec.flowcli.requirements_verifier import RequirementsVerifier
 from copy import deepcopy as clone
 
-
 click_log.basic_config(LOGGER)
 
 
 @click.command()
 @click_log.simple_verbosity_option(LOGGER)
 @project_code_option(
     help="Not required when --no-send-to-flow option is set",
@@ -90,51 +89,66 @@
 @click.option(
     "--company-id",
     required=False,
     envvar=("CONVISO_COMPANY_ID", "FLOW_COMPANY_ID"),
     help="Company ID on Conviso Platform",
 )
 @click.option(
+    '--asset-name',
+    required=False,
+    envvar=("CONVISO_ASSET_NAME", "FLOW_ASSET_NAME"),
+    help="Provides a asset name.",
+)
+@click.option(
+    '--vulnerability-auto-close',
+    default=False,
+    is_flag=True,
+    hidden=True,
+    help="Enable auto fixing vulnerabilities on cp.",
+)
+@click.option(
     '--from-ast',
     default=False,
     is_flag=True,
     hidden=True,
     help="Internal use only.",
 )
 @help_option
 @pass_flow_context
 @click.pass_context
 def run(
-    context,
-    flow_context,
-    project_code,
-    asset_id,
-    company_id,
-    repository_dir,
-    send_to_flow,
-    custom_sca_tags,
-    scanner_timeout,
-    parallel_workers,
-    deploy_id,
-    experimental,
-    from_ast
+        context,
+        flow_context,
+        project_code,
+        asset_id,
+        company_id,
+        repository_dir,
+        send_to_flow,
+        custom_sca_tags,
+        scanner_timeout,
+        parallel_workers,
+        deploy_id,
+        experimental,
+        asset_name,
+        vulnerability_auto_close,
+        from_ast
 ):
-    '''
+    """
       This command will perform SCA analysis at the source code. The analysis
       results can be reported or not to flow application.
-    '''
+    """
     context.params['company_id'] = company_id if company_id is not None else None
 
     if not from_ast:
         prepared_context = RequirementsVerifier.prepare_context(clone(context))
 
         params_to_copy = [
             'project_code', 'asset_id', 'repository_dir', 'send_to_flow',
-            'deploy_id', 'custom_sca_tags', 'scanner_timeout',
-            'parallel_workers', 'experimental'
+            'deploy_id', 'custom_sca_tags', 'scanner_timeout', 'parallel_workers',
+            'experimental', 'asset_name', 'vulnerability_auto_close'
         ]
 
         for param_name in params_to_copy:
             context.params[param_name] = (
                 locals()[param_name] or prepared_context.params[param_name]
             )
 
@@ -144,20 +158,21 @@
         context.params['asset_id'],
         context.params['repository_dir'],
         context.params['send_to_flow'],
         context.params['custom_sca_tags'],
         context.params['scanner_timeout'],
         context.params['parallel_workers'],
         context.params['deploy_id'],
-        context.params['experimental']
+        context.params['experimental'],
+        context.params['company_id']
     )
 
 
 def deploy_results_to_conviso(
-    conviso_api, results_filepaths, project_code, deploy_id=None
+        conviso_api, results_filepaths, project_code, deploy_id=None
 ):
     results_context = click.progressbar(
         results_filepaths, label="Sending SCA reports to Conviso Platform"
     )
     default_report_type = "sca"
 
     with results_context as reports:
@@ -170,108 +185,100 @@
                 default_report_type=default_report_type,
                 deploy_id=deploy_id,
             )
             report_file.close()
     pass
 
 
-def deploy_results_to_conviso_beta(
-    conviso_api, results_filepaths, asset_id
-):
+def deploy_results_to_conviso_beta(conviso_api, results_filepaths, asset_id):
+    """ Send vulnerabilities to conviso platform via graphql endpoint """
+
     results_context = click.progressbar(
         results_filepaths, label="Sending SCA reports to Conviso Platform"
     )
 
     duplicated_issues = 0
 
     with results_context as reports:
         for report_path in reports:
             report_file = open(report_path)
             report_content = json.load(report_file)
             issues = report_content.get("issues", [])
 
             for issue in issues:
                 description = issue.get("description")
+                hash_issue = issue.get('hash_issue', [])
 
                 if not description:
                     description = ""
 
                 sanitezed_description = strings.parse_to_ascii(description)
 
                 issue_model = CreateScaFindingInput(
-                    asset_id = asset_id,
-                    title = issue.get("title"),
-                    description = sanitezed_description,
-                    severity = issue.get("severity"),
-                    solution = issue.get("solution"),
-                    reference = parse_conviso_references(issue.get("references")),
-                    file_name = issue.get("path"),
-                    affected_version = issue.get("version"),
-                    package = issue.get("component"),
-                    cve = issue.get("cve", []),
+                    asset_id=asset_id,
+                    title=issue.get("title"),
+                    description=sanitezed_description,
+                    severity=issue.get("severity"),
+                    solution=issue.get("solution"),
+                    reference=parse_conviso_references(issue.get("references")),
+                    file_name=issue.get("path"),
+                    affected_version=issue.get("version"),
+                    package=issue.get("component"),
+                    cve=issue.get("cve", []),
+                    original_issue_id_from_tool=hash_issue
                 )
 
                 try:
                     conviso_api.issues.create_sca(issue_model)
                 except ReponseError as error:
                     if error.code == 'RECORD_NOT_UNIQUE':
                         duplicated_issues += 1
                     else:
-                        raise(error)
+                        raise error
 
     msg = "\U0001F4AC %s Issue/Issues ignored during duplication" % duplicated_issues
     LOGGER.info(msg)
 
 
 def parse_conviso_references(references=[]):
     DIVIDER = "\n"
+    urls = [ref['url'] for ref in references]
+    return DIVIDER.join(urls)
 
-    return DIVIDER.join(references)
 
 def perform_command(
-    flow_context, project_code, asset_id, repository_dir, send_to_flow, custom_sca_tags, scanner_timeout, parallel_workers, deploy_id, experimental
+        flow_context, project_code, asset_id, repository_dir, send_to_flow, custom_sca_tags, scanner_timeout,
+        parallel_workers, deploy_id, experimental, company_id
 ):
-
     if send_to_flow and not experimental and not project_code:
         raise click.MissingParameter(
             "It is required when sending reports to Conviso Platform API.",
             param_type="option",
             param_hint="--project-code",
         )
-    
+
     if send_to_flow and experimental and not asset_id:
         raise click.MissingParameter(
             "It is required when sending reports to Conviso Platform using experimental API.",
             param_type="option",
             param_hint="--asset-id",
         )
 
     try:
         REQUIRED_CODEBASE_PATH = '/code'
-        DANDELION_IMAGE_NAME = 'scabox-dandelion'
-        RAMPHASTOS_IMAGE_NAME = 'scabox-ramphastos'
+        OSV_SCANNER_IMAGE_NAME = 'osv_scanner'
 
         scanners = {
-            DANDELION_IMAGE_NAME: {
-                'repository_name': DANDELION_IMAGE_NAME,
-                'tag': 'latest',
-                'command': [
-                    '-c', REQUIRED_CODEBASE_PATH,
-                    '-f', 'json',
-                    '-o', '/{}.json'.format(DANDELION_IMAGE_NAME)
-                ],
-                'repository_dir': repository_dir
-            },
-            RAMPHASTOS_IMAGE_NAME: {
-                'repository_name': RAMPHASTOS_IMAGE_NAME,
+            OSV_SCANNER_IMAGE_NAME: {
+                'repository_name': OSV_SCANNER_IMAGE_NAME,
                 'tag': 'latest',
                 'command': [
                     '-c', REQUIRED_CODEBASE_PATH,
                     '-f', 'json',
-                    '-o', '/{}.json'.format(RAMPHASTOS_IMAGE_NAME)
+                    '-o', '/{}.json'.format(OSV_SCANNER_IMAGE_NAME)
                 ],
                 'repository_dir': repository_dir
             },
         }
 
         if custom_sca_tags:
             for custom_tag in custom_sca_tags:
@@ -302,16 +309,16 @@
         for unit in scabox.scanners:
             file_path = unit.results
             if file_path:
                 results_filepaths.append(file_path)
 
         if send_to_flow:
             LOGGER.info("   Sending data to Conviso Platform...")
+            conviso_beta_api = flow_context.create_conviso_api_client_beta()
             if experimental:
-                conviso_beta_api = flow_context.create_conviso_api_client_beta()
                 deploy_results_to_conviso_beta(
                     conviso_beta_api,
                     results_filepaths,
                     asset_id,
                 )
             else:
                 deploy_results_to_conviso(
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/flowcli/vulnerability/assert_security_rules.py` & `conviso-flowcli-2.1.6/convisoappsec/flowcli/vulnerability/assert_security_rules.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import click
 import click_log
 import logging
 import yaml
 import json
 import jsonschema
-
+from pkg_resources import resource_filename
 from convisoappsec.flowcli import help_option
 from convisoappsec.flowcli.context import pass_flow_context
 from convisoappsec.flowcli.common import project_code_option, asset_id_option
 from convisoappsec.flowcli.requirements_verifier import RequirementsVerifier
-
+from convisoappsec.flowcli.companies.ls import Companies
 
 logger = logging.getLogger(__name__)
 click_log.basic_config(logger)
 
 
 @click.command('assert-security-rules')
 @click_log.simple_verbosity_option(logger)
@@ -43,24 +43,38 @@
 )
 @click.option(
     '--rules-file',
     'rules_file',
     type=click.File('r'),
     required=True
 )
+@click.option(
+    '--asset-name',
+    required=False,
+    envvar=("CONVISO_ASSET_NAME", "FLOW_ASSET_NAME"),
+    help="Provides a asset name.",
+)
 @help_option
 @pass_flow_context
 @click.pass_context
-def assert_security_rules(context, flow_context, project_code, asset_id, company_id, repository_dir, rules_file):
+def assert_security_rules(
+        context, flow_context, project_code, asset_id, company_id, repository_dir, rules_file, asset_name
+):
+    new_vulnerability_management = False
 
     if project_code is None:
         prepared_context = RequirementsVerifier.prepare_context(context)
         asset_id = prepared_context.params['asset_id']
         new_vulnerability_management = prepared_context.params['experimental']
 
+    if company_id is None:
+        companies = Companies()
+        company = companies.ls(flow_context, company_id=company_id)
+        company_id = company[0]['id']
+
     try:
         rules = yaml.load(
             rules_file,
             Loader=yaml.Loader
         )
 
         click.secho(
@@ -71,16 +85,17 @@
         click.secho(
             "\U0001F4AC Applying the given rules at security gate:\n{0}".format(yaml.dump(rules)),
             bold=True
         )
 
         if new_vulnerability_management:
             conviso_api = flow_context.create_conviso_graphql_client()
+            statuses = ['IDENTIFIED', 'IN_PROGRESS', 'AWAITING_VALIDATION']
 
-            issues = conviso_api.issues.get_issues_stats(asset_id, company_id)
+            issues = conviso_api.issues.get_issues_stats(asset_id, company_id, statuses)
 
             if validate_json(rules)[0] is False:
                 msg = click.secho(
                     '\U0001F4AC Error: Validation of security gate yaml file, failed in validation step!',
                     bold=True
                 )
 
@@ -110,39 +125,42 @@
             json.dumps(response['summary'], indent=4)
         )
 
         raise click.ClickException(
             'Vulnerabilities quantity offending security rules'
         )
 
+
 def validate_rules(issues, rules):
     """ function to validate security gate rules """
     response = {"locked": False, "summary": [{"from": "any", "severity": {}}]}
-    parsed_issues = { issue['value']: issue['count'] for issue in issues }
+    parsed_issues = {issue['value']: issue['count'] for issue in issues}
 
     for i, rule in enumerate(rules['rules']):
         for criticity, rule_max in rule['severity'].items():
             if parsed_issues[criticity.upper()] > rule_max['maximum']:
                 response['locked'] = True
             response["summary"][i]["severity"].update({criticity: {"quantity": parsed_issues[criticity.upper()]}})
 
     return response
 
+
 def validate_json(rules):
     """ Validate a JSON document against a JSON schema. """
+    schema_path = resource_filename('convisoappsec', 'flowcli/vulnerability/rules_schema.json')
 
-    with open('examples/rules_schema.json', 'r') as json_file:
+    with open(schema_path, 'r') as json_file:
         schema = json.load(json_file)
-
     try:
         jsonschema.validate(rules, schema)
         return True, "Validation successful"
     except jsonschema.exceptions.ValidationError as e:
         return False, str(e)
 
+
 EPILOG = '''
 '''
 
 SHORT_HELP = ''
 
 command = 'conviso vulnerability assert-security-rules'
 assert_security_rules.short_help = SHORT_HELP
```

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/sast/decision.py` & `conviso-flowcli-2.1.6/convisoappsec/sast/decision.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/convisoappsec/sast/sastbox.py` & `conviso-flowcli-2.1.6/convisoappsec/sast/sastbox.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import tempfile
 import tarfile
 import docker
 import os
+import click
+import json
+from io import BytesIO
 from contextlib import suppress
 from pathlib import Path
+from convisoappsec.flowcli.context import pass_flow_context
 
 bitbucket = os.getenv('BITBUCKET_CLONE_DIR')
 
 
 class SASTBox(object):
     REGISTRY = 'docker.convisoappsec.com'
     REPOSITORY_NAME = 'sastbox_v2'
-    DEFAULT_TAG = 'unstable'
-    CONTAINER_REPORTS_DIR = '/tmp'
+    DEFAULT_TAG = 'latest'
     CONTAINER_CODE_DIR = bitbucket or '/code'
-    WORKSPACE_REPORT_PATH = ["tmp"]
-    JSON_REPORT_PATTERN = 'output.sarif'
+    CONTAINER_REPORTS_DIR = '/tmp'
+    WORKSPACE_REPORT_PATH = CONTAINER_CODE_DIR
+    JSON_REPORT_PATTERN = 'output.json'
     SUCCESS_EXIT_CODE = 1
     USER_ENV_VAR = "USER"
 
     def __init__(self, registry=None, repository_name=None, tag=None):
         self.docker = docker.from_env(
             version="auto"
         )
@@ -36,15 +40,15 @@
             'reauth': True,
         }
 
         login_result = self.docker.login(**login_args)
         return login_result
 
     def run_scan_diff(
-        self, code_dir, current_commit, previous_commit, log=None, token=None
+            self, code_dir, current_commit, previous_commit, log=None, token=None
     ):
         return self._scan_diff(
             code_dir, current_commit, previous_commit, log, token
         )
 
     @property
     def size(self):
@@ -54,25 +58,18 @@
             )
             descriptor = registry_data.attrs.get('Descriptor', {})
             return descriptor.get('size') * 1024 * 1024
         except docker.errors.APIError:
             return 6300 * 1024 * 1024
 
     def pull(self):
-        """
-        {
-            'status': 'Downloading',
-            'progressDetail': {'current': int, 'total': int},
-            'id': 'string'
-        }
-        """
         size = self.size
         layers = {}
         for line in self.docker.api.pull(
-            self.repository, tag=self.tag, stream=True, decode=True
+                self.repository, tag=self.tag, stream=True, decode=True
         ):
             status = line.get('status', '')
             detail = line.get('progressDetail', {})
 
             if status == 'Downloading':
                 with suppress(Exception):
                     layer_id = line.get('id')
@@ -80,95 +77,99 @@
                     layer.update(detail)
                     layers[layer_id] = layer
 
                     for layer in layers.values():
                         current = layer.get('current')
                         total = layer.get('total')
 
-                        if (current/total) > 0.98 and not layer.get('done'):
+                        if (current / total) > 0.98 and not layer.get('done'):
                             yield current
                             layer.update({'done': True})
 
         yield size
 
     def _scan_diff(self, code_dir, current_commit, previous_commit, log, token):
-        report_dir = '/tmp/output.sarif'
 
         environment = {
             'PREVIOUS_COMMIT': previous_commit,
             'CURRENT_COMMIT': current_commit,
             'SASTBOX_REPORTS_DIR': self.CONTAINER_REPORTS_DIR,
-            'SASTBOX_REPORT_PATTERN': report_dir,
+            'SASTBOX_REPORT_PATTERN': self.JSON_REPORT_PATTERN,
             'SASTBOX_CODE_DIR': self.CONTAINER_CODE_DIR,
-            'REGISTRY_PASSWORD': token,
-            'REGISTRY_URL': self.REGISTRY,
-            'REGISTRY_USERNAME': 'AWS'
         }
 
         command = (
-            ''' -c {code_dir} --diff={previous_commit},{current_commit} -a -o {report_dir} -v --dedup'''.format(
-                code_dir=code_dir, previous_commit=previous_commit, current_commit=current_commit, report_dir=report_dir)
-        )  # noqa: E501
-
-        volumes = {
-            '/var/run/docker.sock': {'bind': '/var/run/docker.sock', 'mode': 'rw'},
-            '/tmp': {'bind': '/tmp', 'mode': 'rw'}
-        }
+            ''' ruby manager/sastbox_cli.rb -c {code_dir} -a -o {report} --diff={previous_commit},{current_commit} && \
+            cp $(find $SASTBOX_REPORT_PATTERN) $SASTBOX_REPORTS_DIR'''.format(
+                code_dir=self.CONTAINER_CODE_DIR, previous_commit=previous_commit, current_commit=current_commit,
+                report='/tmp/output.sarif')
+        )
 
         create_args = {
             'image': self.image,
-            'entrypoint': ['ruby', '/sastbox2-manager/sastbox_cli.rb'],
-            'command': command,
+            'entrypoint': ['sh', '-c'],
+            'command': [command],
             'tty': True,
             'detach': True,
             'environment': environment,
-            'volumes': volumes,
         }
 
+        # clean all containers not running
+        for container in self.docker.containers.list(filters={'status': 'exited'}):
+            container.remove(force=True)
+
         self.container = self.docker.containers.create(**create_args)
         # previously create source code tar ball
         source_code_tarball_file = tempfile.TemporaryFile()
         source_code_tarball = tarfile.open(
             mode="w|gz", fileobj=source_code_tarball_file
         )
 
-        source_code_tarball.add(name=code_dir, arcname=self.CONTAINER_CODE_DIR)
+        source_code_tarball.add(
+            name=code_dir,
+            arcname=self.CONTAINER_CODE_DIR,
+        )
 
         source_code_tarball.close()
 
         source_code_tarball_file.seek(0)
         self.container.put_archive("/", source_code_tarball_file)
         source_code_tarball_file.close()
         self.container.start()
 
         for line in self.container.logs(stream=True):
             if log:
                 log(line, new_line=False)
 
+        # self.recovery_technologies_file()
+
         wait_result = self.container.wait()
         status_code = wait_result.get('StatusCode')
 
         if not status_code == self.SUCCESS_EXIT_CODE:
             raise RuntimeError(
                 'SASTBox exiting with error status code'
             )
 
-        result, _ = self.container.get_archive(report_dir)
+        chunks, _ = self.container.get_archive(
+            self.CONTAINER_REPORTS_DIR
+        )
 
         reports_tarball_file = tempfile.TemporaryFile()
 
-        for chunk in result:
+        for chunk in chunks:
             reports_tarball_file.write(chunk)
 
         tempdir = tempfile.mkdtemp()
         reports_tarball_file.seek(0)
         reports_tarball = tarfile.open(mode="r|", fileobj=reports_tarball_file)
         reports_tarball.extractall(path=tempdir)
         reports_tarball.close()
         reports_tarball_file.close()
+        self.container.remove(force=True)
 
         return self._list_reports_paths(tempdir)
 
     @property
     def repository(self):
         return "{registry}/{repository_name}".format(
             registry=self.registry,
@@ -184,11 +185,76 @@
 
     def __del__(self):
         with suppress(Exception):
             self.container.remove(v=True, force=True)
 
     @classmethod
     def _list_reports_paths(cls, root_dir):
+        root_dir = root_dir + cls.CONTAINER_REPORTS_DIR
         sastbox_reports_dir = Path(root_dir)
 
         for report in sastbox_reports_dir.glob(cls.JSON_REPORT_PATTERN):
             yield report
+
+    def recovery_technologies_file(self):
+        """ Method to recovery a fingerprint file inside the container with founded technology """
+        try:
+            generator_object, file_info = self.container.get_archive('/tmp/fingerprint.json')
+            file_content = b"".join(generator_object)
+            file_content_stream = BytesIO(file_content)
+            tar = tarfile.open(fileobj=file_content_stream)
+            file_data = tar.extractfile(file_info['name'])
+            content = json.loads(file_data.read())
+            technologies = content['result']['technologies']
+        except Exception as error:
+            msg = "\U0001F4AC Something goes wrong when try to recovery the technologies, continuing ..."
+            log_func(msg)
+
+            technologies = []
+
+        if technologies is None:
+            return
+
+        self.update_asset_technologies(technologies=technologies)
+
+    @staticmethod
+    @pass_flow_context
+    @click.pass_context
+    def update_asset_technologies(flow_context, context, technologies):
+        """
+        Update technologies on asset.
+        Args:
+            flow_context (dict): Flow context containing parameters.
+            context (object): Object containing necessary methods (e.g., create_conviso_graphql_client).
+            technologies (list): List of technologies to be updated.
+        Returns:
+            dict: Response from the API call.
+        """
+
+        # this prevents a broken execution when something goes wrong.
+        try:
+            company_id = flow_context.params.get('company_id')
+            asset_id = flow_context.params.get('asset_id')
+            asset_name = flow_context.params.get('asset_name')
+            unwanted_technologies = {
+                'unknown', 'json', 'text', 'ini', 'diff', 'xml', 'markdown', 'csv', 'gemfile.lock', 'html+erb',
+                'javascript+erb', 'robots.txt', 'yaml'
+            }
+            updated_technologies = [tech for tech in technologies if tech not in unwanted_technologies]
+            conviso_api = context.create_conviso_graphql_client()
+
+            response = conviso_api.assets.update_asset(
+                company_id=int(company_id),
+                asset_id=asset_id,
+                asset_name=asset_name,
+                technologies=updated_technologies
+            )
+        except Exception as error:
+            msg = "\U0001F4AC Something goes wrong when try to send technologies to the cp, continuing ..."
+            log_func(msg)
+
+            response = None
+
+        return response
+
+def log_func(msg, new_line=True, clear=False):
+    click.echo(msg, nl=new_line, err=True)
```

### Comparing `conviso-flowcli-2.0.0rc9/scripts/shell_completer/flow_bash_completer.sh` & `conviso-flowcli-2.1.6/scripts/shell_completer/flow_bash_completer.sh`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/scripts/shell_completer/flow_zsh_completer.sh` & `conviso-flowcli-2.1.6/scripts/shell_completer/flow_zsh_completer.sh`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-2.0.0rc9/setup.py` & `conviso-flowcli-2.1.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,48 +14,51 @@
 
 with open(VERSION_MODULE) as fp:
     exec(fp.read(), version_module_context)
 
 with open(README_PATH, "r") as fh:
     long_description = fh.read()
 
-
 version = version_module_context.get('__version__')
 
-
 setup(
     name='conviso-flowcli',
     version=version,
     long_description=long_description,
     long_description_content_type='text/markdown',
-    maintainer='Jean Carlos Sales Pantoja',
-    maintainer_email='jpantoja@convisoappsec.com',
+    maintainer='Conviso',
+    maintainer_email='development@convisoappsec.com',
+    package_data={'convisoappsec': ['flowcli/vulnerability/rules_schema.json']},
     packages=find_packages(
         exclude=["test*"],
     ),
     install_requires=[
         "GitPython>=3.1.2,<4",
         "click>=7.1.2,<8",
-        "requests>=2.23.0,<3",
-        "urllib3<=2.0.6",
+        "requests==2.31.0",
+        "urllib3==2.2.0",
         "semantic-version>=2.8.5,<3",
         "docker<=6.1.3",
-        "PyYAML==5.3.1", # https://github.com/yaml/pyyaml/issues/724
+        "PyYAML==6.0.1",
         "click-log>=0.3.2,<1",
         "transitions>=0.8.7,<1",
         "jsonschema>=2.5.1,<3",
         "giturlparse<=0.12.0",
-        "jmespath>=0.9.0,<1.0.1"
+        "jmespath>=0.9.0,<1.0.1",
+        "setuptools==69.2.0"
     ],
     entry_points={
         'console_scripts': [
             'flow=convisoappsec.flowcli.entrypoint:cli',
             'conviso=convisoappsec.flowcli.entrypoint:cli',
         ]
     },
     scripts=[
         path.join(SCRIPTS_SHELL_COMPLETER_DIR, 'flow_bash_completer.sh'),
         path.join(SCRIPTS_SHELL_COMPLETER_DIR, 'flow_zsh_completer.sh'),
         path.join(SCRIPTS_SHELL_COMPLETER_DIR, 'flow_fish_completer.fish'),
     ],
-    python_requires='>=3.5',
+    project_urls={
+        'Source': 'https://github.com/convisoappsec/convisocli/',
+    },
+    python_requires='>=3.8',
 )
```

