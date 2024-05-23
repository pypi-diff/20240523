# Comparing `tmp/conviso-cli-2.1.5.dev9.tar.gz` & `tmp/conviso-cli-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conviso-cli-2.1.5.dev9.tar", last modified: Tue May 14 16:45:47 2024, max compression
+gzip compressed data, was "conviso-cli-2.1.6.tar", last modified: Thu May 23 12:53:34 2024, max compression
```

## Comparing `conviso-cli-2.1.5.dev9.tar` & `conviso-cli-2.1.6.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.022270 conviso-cli-2.1.5.dev9/
--rw-r--r--   0 root         (0) root         (0)      546 2024-05-14 16:45:47.022270 conviso-cli-2.1.5.dev9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      234 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.010270 conviso-cli-2.1.5.dev9/conviso_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      546 2024-05-14 16:45:46.000000 conviso-cli-2.1.5.dev9/conviso_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5691 2024-05-14 16:45:47.000000 conviso-cli-2.1.5.dev9/conviso_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 16:45:46.000000 conviso-cli-2.1.5.dev9/conviso_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-05-14 16:45:46.000000 conviso-cli-2.1.5.dev9/conviso_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      251 2024-05-14 16:45:46.000000 conviso-cli-2.1.5.dev9/conviso_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-14 16:45:46.000000 conviso-cli-2.1.5.dev9/conviso_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.010270 conviso-cli-2.1.5.dev9/convisoappsec/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.010270 conviso-cli-2.1.5.dev9/convisoappsec/common/
--rw-r--r--   0 root         (0) root         (0)      105 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7686 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/common/box.py
--rw-r--r--   0 root         (0) root         (0)    12525 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/common/docker.py
--rw-r--r--   0 root         (0) root         (0)      230 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/common/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2067 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/common/git_data_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.010270 conviso-cli-2.1.5.dev9/convisoappsec/common/graphql/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/common/graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2055 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/common/graphql/error_handlers.py
--rw-r--r--   0 root         (0) root         (0)      247 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/common/graphql/errors.py
--rw-r--r--   0 root         (0) root         (0)     1323 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/common/graphql/low_client.py
--rw-r--r--   0 root         (0) root         (0)      185 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/common/strings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.010270 conviso-cli-2.1.5.dev9/convisoappsec/flow/
--rw-r--r--   0 root         (0) root         (0)       81 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12044 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/__init__.py
--rw-r--r--   0 root         (0) root         (0)      502 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/models/issues/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/models/issues/__init__.py
--rw-r--r--   0 root         (0) root         (0)      310 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/models/issues/iac.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/models/issues/normalize.py
--rw-r--r--   0 root         (0) root         (0)     1673 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/models/issues/sast.py
--rw-r--r--   0 root         (0) root         (0)     1673 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/models/issues/sca.py
--rw-r--r--   0 root         (0) root         (0)     3614 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/resources_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/schemas/mutations/
--rw-r--r--   0 root         (0) root         (0)      607 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/schemas/resolvers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/schemas/resolvers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      790 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      345 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/models/asset.py
--rw-r--r--   0 root         (0) root         (0)      511 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/models/issues.py
--rw-r--r--   0 root         (0) root         (0)      972 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/models/project.py
--rw-r--r--   0 root         (0) root         (0)     6458 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/resources_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/schemas/mutations/
--rw-r--r--   0 root         (0) root         (0)     1254 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/schemas/resolvers/
--rw-r--r--   0 root         (0) root         (0)     2352 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/source_code_scanner/
--rw-r--r--   0 root         (0) root         (0)      227 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/source_code_scanner/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/source_code_scanner/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1655 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/source_code_scanner/scc.py
--rw-r--r--   0 root         (0) root         (0)     4726 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/source_code_scanner/source_code_scanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/util/
--rw-r--r--   0 root         (0) root         (0)      160 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2093 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/util/ci_provider.py
--rw-r--r--   0 root         (0) root         (0)      480 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/util/metrics.py
--rw-r--r--   0 root         (0) root         (0)      508 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/util/source_code_compressor.py
--rw-r--r--   0 root         (0) root         (0)    14635 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/version_control_system_adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/version_searchers/
--rw-r--r--   0 root         (0) root         (0)      294 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/version_searchers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py
--rw-r--r--   0 root         (0) root         (0)     1266 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/version_searchers/timebased_version_seacher.py
--rw-r--r--   0 root         (0) root         (0)      943 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/version_searchers/version_searcher_result.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.014270 conviso-cli-2.1.5.dev9/convisoappsec/flow/versioning_style/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/versioning_style/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1041 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flow/versioning_style/semantic_versioning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.018270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/
--rw-r--r--   0 root         (0) root         (0)       64 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/__init__.py
--rw-r--r--   0 root         (0) root         (0)       99 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.018270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/assets/
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2278 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/assets/create.py
--rw-r--r--   0 root         (0) root         (0)      310 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/assets/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     1484 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/assets/ls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.018270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/ast/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/ast/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9410 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/ast/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     5350 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.018270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/companies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/companies/__init__.py
--rw-r--r--   0 root         (0) root         (0)      892 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/companies/ls.py
--rw-r--r--   0 root         (0) root         (0)     1309 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.018270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.018270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/__init__.py
--rw-r--r--   0 root         (0) root         (0)      190 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/context.py
--rw-r--r--   0 root         (0) root         (0)      677 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.018270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/__init__.py
--rw-r--r--   0 root         (0) root         (0)      346 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.018270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/
--rw-r--r--   0 root         (0) root         (0)       64 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      194 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/context.py
--rw-r--r--   0 root         (0) root         (0)      675 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.018270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/
--rw-r--r--   0 root         (0) root         (0)       56 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/__init__.py
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     2815 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py
--rw-r--r--   0 root         (0) root         (0)     3500 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py
--rw-r--r--   0 root         (0) root         (0)     4681 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/values.py
--rw-r--r--   0 root         (0) root         (0)      353 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      763 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/ls.py
--rw-r--r--   0 root         (0) root         (0)      970 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/show.py
--rw-r--r--   0 root         (0) root         (0)     2878 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.018270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/findings/
--rw-r--r--   0 root         (0) root         (0)       58 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/findings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.018270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/findings/create/
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/findings/create/__init__.py
--rw-r--r--   0 root         (0) root         (0)      269 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/findings/create/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.022270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/findings/create/with_/
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/findings/create/with_/__init__.py
--rw-r--r--   0 root         (0) root         (0)      309 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/findings/create/with_/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/findings/create/with_/version_tracker.py
--rw-r--r--   0 root         (0) root         (0)      344 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/findings/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.022270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/findings/import_sarif/
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/findings/import_sarif/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7209 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/findings/import_sarif/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      331 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/help_option.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.022270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/iac/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/iac/__init__.py
--rw-r--r--   0 root         (0) root         (0)      241 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/iac/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    11269 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/iac/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.022270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/projects/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/projects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/projects/ls.py
--rw-r--r--   0 root         (0) root         (0)     9438 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/requirements_verifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.022270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/sast/
--rw-r--r--   0 root         (0) root         (0)       49 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/sast/__init__.py
--rw-r--r--   0 root         (0) root         (0)      245 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/sast/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    19208 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/sast/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.022270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/sca/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/sca/__init__.py
--rw-r--r--   0 root         (0) root         (0)      241 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/sca/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    10781 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/sca/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.022270 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/vulnerability/
--rw-r--r--   0 root         (0) root         (0)       67 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/vulnerability/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4937 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/vulnerability/assert_security_rules.py
--rw-r--r--   0 root         (0) root         (0)      386 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/vulnerability/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      948 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/vulnerability/rules_schema.json
--rw-r--r--   0 root         (0) root         (0)    16094 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/flowcli/vulnerability/run.py
--rw-r--r--   0 root         (0) root         (0)      231 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.022270 conviso-cli-2.1.5.dev9/convisoappsec/sast/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/sast/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/sast/decision.py
--rw-r--r--   0 root         (0) root         (0)     8982 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/sast/sastbox.py
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/convisoappsec/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.010270 conviso-cli-2.1.5.dev9/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:45:47.022270 conviso-cli-2.1.5.dev9/scripts/shell_completer/
--rw-r--r--   0 root         (0) root         (0)      624 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/scripts/shell_completer/flow_bash_completer.sh
--rw-r--r--   0 root         (0) root         (0)      147 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/scripts/shell_completer/flow_fish_completer.fish
--rw-r--r--   0 root         (0) root         (0)      844 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/scripts/shell_completer/flow_zsh_completer.sh
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 16:45:47.022270 conviso-cli-2.1.5.dev9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1882 2024-05-14 16:45:44.000000 conviso-cli-2.1.5.dev9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.925838 conviso-cli-2.1.6/
+-rw-r--r--   0 root         (0) root         (0)      541 2024-05-23 12:53:34.925838 conviso-cli-2.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      234 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.913838 conviso-cli-2.1.6/conviso_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      541 2024-05-23 12:53:34.000000 conviso-cli-2.1.6/conviso_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5691 2024-05-23 12:53:34.000000 conviso-cli-2.1.6/conviso_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 12:53:34.000000 conviso-cli-2.1.6/conviso_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-05-23 12:53:34.000000 conviso-cli-2.1.6/conviso_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      248 2024-05-23 12:53:34.000000 conviso-cli-2.1.6/conviso_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-23 12:53:34.000000 conviso-cli-2.1.6/conviso_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.913838 conviso-cli-2.1.6/convisoappsec/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.913838 conviso-cli-2.1.6/convisoappsec/common/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7686 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/common/box.py
+-rw-r--r--   0 root         (0) root         (0)    12525 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/common/docker.py
+-rw-r--r--   0 root         (0) root         (0)      230 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/common/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/common/git_data_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.913838 conviso-cli-2.1.6/convisoappsec/common/graphql/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/common/graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/common/graphql/error_handlers.py
+-rw-r--r--   0 root         (0) root         (0)      247 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/common/graphql/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/common/graphql/low_client.py
+-rw-r--r--   0 root         (0) root         (0)      185 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/common/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.913838 conviso-cli-2.1.6/convisoappsec/flow/
+-rw-r--r--   0 root         (0) root         (0)       81 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12044 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.913838 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.913838 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.917838 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.917838 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      310 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/iac.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/normalize.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/sast.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/sca.py
+-rw-r--r--   0 root         (0) root         (0)     3614 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/resources_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.917838 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.917838 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/schemas/mutations/
+-rw-r--r--   0 root         (0) root         (0)      607 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.917838 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/schemas/resolvers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/schemas/resolvers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.917838 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      790 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.917838 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      345 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/models/asset.py
+-rw-r--r--   0 root         (0) root         (0)      511 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/models/issues.py
+-rw-r--r--   0 root         (0) root         (0)      972 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/models/project.py
+-rw-r--r--   0 root         (0) root         (0)     6458 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/resources_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.917838 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.917838 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/schemas/mutations/
+-rw-r--r--   0 root         (0) root         (0)     1254 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.917838 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/schemas/resolvers/
+-rw-r--r--   0 root         (0) root         (0)     2352 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.917838 conviso-cli-2.1.6/convisoappsec/flow/source_code_scanner/
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/source_code_scanner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/source_code_scanner/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/source_code_scanner/scc.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/source_code_scanner/source_code_scanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.917838 conviso-cli-2.1.6/convisoappsec/flow/util/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/util/ci_provider.py
+-rw-r--r--   0 root         (0) root         (0)      480 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/util/metrics.py
+-rw-r--r--   0 root         (0) root         (0)      508 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/util/source_code_compressor.py
+-rw-r--r--   0 root         (0) root         (0)    14635 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/version_control_system_adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.917838 conviso-cli-2.1.6/convisoappsec/flow/version_searchers/
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/version_searchers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/version_searchers/timebased_version_seacher.py
+-rw-r--r--   0 root         (0) root         (0)      943 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/version_searchers/version_searcher_result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.917838 conviso-cli-2.1.6/convisoappsec/flow/versioning_style/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/versioning_style/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flow/versioning_style/semantic_versioning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.921838 conviso-cli-2.1.6/convisoappsec/flowcli/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       99 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.921838 conviso-cli-2.1.6/convisoappsec/flowcli/assets/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/assets/create.py
+-rw-r--r--   0 root         (0) root         (0)      310 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/assets/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/assets/ls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.921838 conviso-cli-2.1.6/convisoappsec/flowcli/ast/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/ast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8045 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/ast/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     5350 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.921838 conviso-cli-2.1.6/convisoappsec/flowcli/companies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/companies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      892 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/companies/ls.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.921838 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.921838 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      190 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/context.py
+-rw-r--r--   0 root         (0) root         (0)      677 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.921838 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      346 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.921838 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      194 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/context.py
+-rw-r--r--   0 root         (0) root         (0)      675 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.921838 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     2815 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py
+-rw-r--r--   0 root         (0) root         (0)     4681 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/values.py
+-rw-r--r--   0 root         (0) root         (0)      353 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)      763 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/ls.py
+-rw-r--r--   0 root         (0) root         (0)      970 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/deploy/show.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.921838 conviso-cli-2.1.6/convisoappsec/flowcli/findings/
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/findings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.921838 conviso-cli-2.1.6/convisoappsec/flowcli/findings/create/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/findings/create/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      269 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/findings/create/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.921838 conviso-cli-2.1.6/convisoappsec/flowcli/findings/create/with_/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/findings/create/with_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      309 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/findings/create/with_/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/findings/create/with_/version_tracker.py
+-rw-r--r--   0 root         (0) root         (0)      344 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/findings/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.925838 conviso-cli-2.1.6/convisoappsec/flowcli/findings/import_sarif/
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/findings/import_sarif/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7209 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/findings/import_sarif/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)      331 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/help_option.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.925838 conviso-cli-2.1.6/convisoappsec/flowcli/iac/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/iac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      241 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/iac/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    11269 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/iac/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.925838 conviso-cli-2.1.6/convisoappsec/flowcli/projects/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/projects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/projects/ls.py
+-rw-r--r--   0 root         (0) root         (0)     9438 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/requirements_verifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.925838 conviso-cli-2.1.6/convisoappsec/flowcli/sast/
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/sast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      245 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/sast/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    18807 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/sast/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.925838 conviso-cli-2.1.6/convisoappsec/flowcli/sca/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/sca/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      241 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/sca/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    10781 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/sca/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.925838 conviso-cli-2.1.6/convisoappsec/flowcli/vulnerability/
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/vulnerability/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4937 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/vulnerability/assert_security_rules.py
+-rw-r--r--   0 root         (0) root         (0)      386 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/vulnerability/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)      948 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/vulnerability/rules_schema.json
+-rw-r--r--   0 root         (0) root         (0)    16094 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/flowcli/vulnerability/run.py
+-rw-r--r--   0 root         (0) root         (0)      231 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.925838 conviso-cli-2.1.6/convisoappsec/sast/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/sast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/sast/decision.py
+-rw-r--r--   0 root         (0) root         (0)     8929 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/sast/sastbox.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/convisoappsec/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.913838 conviso-cli-2.1.6/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:53:34.925838 conviso-cli-2.1.6/scripts/shell_completer/
+-rw-r--r--   0 root         (0) root         (0)      624 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/scripts/shell_completer/flow_bash_completer.sh
+-rw-r--r--   0 root         (0) root         (0)      147 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/scripts/shell_completer/flow_fish_completer.fish
+-rw-r--r--   0 root         (0) root         (0)      844 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/scripts/shell_completer/flow_zsh_completer.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 12:53:34.925838 conviso-cli-2.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1879 2024-05-23 12:53:31.000000 conviso-cli-2.1.6/setup.py
```

### Comparing `conviso-cli-2.1.5.dev9/PKG-INFO` & `conviso-cli-2.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conviso-cli
-Version: 2.1.5.dev9
+Version: 2.1.6
 Summary: UNKNOWN
 Maintainer: Conviso
 Maintainer-email: development@convisoappsec.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/convisoappsec/convisocli/
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `conviso-cli-2.1.5.dev9/conviso_cli.egg-info/PKG-INFO` & `conviso-cli-2.1.6/conviso_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conviso-cli
-Version: 2.1.5.dev9
+Version: 2.1.6
 Summary: UNKNOWN
 Maintainer: Conviso
 Maintainer-email: development@convisoappsec.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/convisoappsec/convisocli/
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `conviso-cli-2.1.5.dev9/conviso_cli.egg-info/SOURCES.txt` & `conviso-cli-2.1.6/conviso_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/common/box.py` & `conviso-cli-2.1.6/convisoappsec/common/box.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/common/docker.py` & `conviso-cli-2.1.6/convisoappsec/common/docker.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/common/git_data_parser.py` & `conviso-cli-2.1.6/convisoappsec/common/git_data_parser.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/common/graphql/error_handlers.py` & `conviso-cli-2.1.6/convisoappsec/common/graphql/error_handlers.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/common/graphql/low_client.py` & `conviso-cli-2.1.6/convisoappsec/common/graphql/low_client.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/api.py` & `conviso-cli-2.1.6/convisoappsec/flow/api.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/models/issues/sast.py` & `conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/sast.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/models/issues/sca.py` & `conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/models/issues/sca.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/resources_api.py` & `conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/resources_api.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py` & `conviso-cli-2.1.6/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/client.py` & `conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/client.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/models/project.py` & `conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/models/project.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/resources_api.py` & `conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/resources_api.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py` & `conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py` & `conviso-cli-2.1.6/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/source_code_scanner/scc.py` & `conviso-cli-2.1.6/convisoappsec/flow/source_code_scanner/scc.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/source_code_scanner/source_code_scanner.py` & `conviso-cli-2.1.6/convisoappsec/flow/source_code_scanner/source_code_scanner.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/util/ci_provider.py` & `conviso-cli-2.1.6/convisoappsec/flow/util/ci_provider.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/version_control_system_adapter.py` & `conviso-cli-2.1.6/convisoappsec/flow/version_control_system_adapter.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py` & `conviso-cli-2.1.6/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/version_searchers/timebased_version_seacher.py` & `conviso-cli-2.1.6/convisoappsec/flow/version_searchers/timebased_version_seacher.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/version_searchers/version_searcher_result.py` & `conviso-cli-2.1.6/convisoappsec/flow/version_searchers/version_searcher_result.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flow/versioning_style/semantic_versioning.py` & `conviso-cli-2.1.6/convisoappsec/flow/versioning_style/semantic_versioning.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/assets/create.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/assets/create.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/assets/ls.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/assets/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/ast/entrypoint.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/ast/entrypoint.py`

 * *Files 11% similar despite different names*

```diff
@@ -128,57 +128,14 @@
     try:
         LOGGER.info("[*] Verifying if any vulnerability was fixed ...")
         auto_close_run.invoke(context)
     except Exception as err:
         raise click.ClickException(str(err)) from err
 
 
-def validate_git_repo(context):
-    """
-    Validates the repository to ensure that it will not lose the git history reference.
-
-    Args:
-        context (<class 'click.core.Context'>)
-
-    Returns:
-        context object
-    """
-    repository_dir = context.params['repository_dir']
-    previous_commit = context.params['previous_commit']
-
-    repo = git.Repo(repository_dir)
-    commits = list(repo.iter_commits())
-
-    if not commits:
-        # No commits in the repository, just return
-        click.echo("No commits found in the repository.")
-        return
-
-    previous_commit_is_in_commits = any(commit.hexsha == previous_commit for commit in commits)
-
-    if previous_commit_is_in_commits:
-        return
-
-    merge_commits = [commit for commit in commits if len(commit.parents) > 1]
-
-    if merge_commits:
-        last_merge_commit = merge_commits[-1]
-        first_parent_commit = last_merge_commit.parents[0]
-        context.params['previous_commit'] = first_parent_commit.hexsha
-    else:
-        if len(commits) > 1:
-            second_latest_commit = commits[1]
-            context.params['previous_commit'] = second_latest_commit.hexsha
-        else:
-            # Only one commit in the repository, use that as the previous commit.
-            context.params['previous_commit'] = commits[0].hexsha
-
-    return
-
-
 def perform_deploy(context):
     """Setup and runs the "deploy create with values" command.
 
     Args:
         context (<class 'click.core.Context'>): clonned context
 
     Returns:
@@ -193,15 +150,14 @@
     """
     context.obj.output_formatter = DeployFormatter(
         format=DeployFormatter.DEFAULT
     )
     context.params = parse_params(context.params, values.params)
     try:
         LOGGER.info("Creating new deploy ...")
-        validate_git_repo(context)
         created_deploy = values.invoke(context)
 
         if created_deploy:
             return created_deploy
 
         raise CreateDeployException("Deploy not created.")
```

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/common.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/common.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/companies/ls.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/companies/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/context.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/context.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/entrypoint.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/create/with_/values.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/deploy/create/with_/values.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/ls.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/deploy/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/deploy/show.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/deploy/show.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/entrypoint.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/findings/create/with_/version_tracker.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/findings/create/with_/version_tracker.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/findings/import_sarif/entrypoint.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/findings/import_sarif/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/iac/run.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/iac/run.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/projects/ls.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/projects/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/requirements_verifier.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/requirements_verifier.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/sast/run.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/sast/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import sys
 import click
 import traceback
-from copy import deepcopy as clone
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
@@ -77,33 +75,33 @@
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
 
     results_filepaths = []
     for r in reports:
         try:
             file_path = str(r)
             results_filepaths.append(file_path)
         except Exception as e:
@@ -112,15 +110,15 @@
     return results_filepaths
 
 
 def deploy_results_to_conviso(
         conviso_api, results_filepaths, project_code, deploy_id=None, commit_refs=None
 ):
     results_context = click.progressbar(
-        results_filepaths, label="Sending SASTBox reports to Conviso Platform"
+        results_filepaths, label="Sending SAST reports to Conviso Platform"
     )
 
     with results_context as reports:
         for report_name in reports:
             report_file = open(report_name)
 
             default_report_type = "sast"
@@ -191,20 +189,17 @@
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
@@ -561,15 +556,15 @@
                     results_filepaths,
                     asset_id,
                     commit_ref=end_commit,
                     deploy_id=deploy_id
                 )
 
             else:
-                commit_refs = git_adapater.show_commit_refs(end_commit)
+                commit_refs = git_adapter.show_commit_refs(end_commit)
 
                 deploy_results_to_conviso(
                     conviso_rest_api,
                     results_filepaths,
                     project_code,
                     deploy_id,
                     commit_refs,
```

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/sca/run.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/sca/run.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/vulnerability/assert_security_rules.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/vulnerability/assert_security_rules.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/vulnerability/rules_schema.json` & `conviso-cli-2.1.6/convisoappsec/flowcli/vulnerability/rules_schema.json`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/flowcli/vulnerability/run.py` & `conviso-cli-2.1.6/convisoappsec/flowcli/vulnerability/run.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/sast/decision.py` & `conviso-cli-2.1.6/convisoappsec/sast/decision.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/convisoappsec/sast/sastbox.py` & `conviso-cli-2.1.6/convisoappsec/sast/sastbox.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 bitbucket = os.getenv('BITBUCKET_CLONE_DIR')
 
 
 class SASTBox(object):
     REGISTRY = 'docker.convisoappsec.com'
     REPOSITORY_NAME = 'sastbox_v2'
-    DEFAULT_TAG = 'unstable'
+    DEFAULT_TAG = 'latest'
     CONTAINER_CODE_DIR = bitbucket or '/code'
-    CONTAINER_REPORTS_DIR = CONTAINER_CODE_DIR
-    WORKSPACE_REPORT_PATH = [CONTAINER_CODE_DIR]
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
@@ -91,29 +91,27 @@
 
         environment = {
             'PREVIOUS_COMMIT': previous_commit,
             'CURRENT_COMMIT': current_commit,
             'SASTBOX_REPORTS_DIR': self.CONTAINER_REPORTS_DIR,
             'SASTBOX_REPORT_PATTERN': self.JSON_REPORT_PATTERN,
             'SASTBOX_CODE_DIR': self.CONTAINER_CODE_DIR,
-            'REGISTRY_PASSWORD': token,
-            'REGISTRY_URL': self.REGISTRY,
-            'REGISTRY_USERNAME': 'AWS'
         }
 
         command = (
-            ''' -c {code_dir} -a -o {report} --diff={previous_commit},{current_commit}'''.format(
+            ''' ruby manager/sastbox_cli.rb -c {code_dir} -a -o {report} --diff={previous_commit},{current_commit} && \
+            cp $(find $SASTBOX_REPORT_PATTERN) $SASTBOX_REPORTS_DIR'''.format(
                 code_dir=self.CONTAINER_CODE_DIR, previous_commit=previous_commit, current_commit=current_commit,
-                report='output.sarif')
+                report='/tmp/output.sarif')
         )
 
         create_args = {
             'image': self.image,
-            'entrypoint': ['ruby', 'manager/sastbox_cli.rb'],
-            'command': command,
+            'entrypoint': ['sh', '-c'],
+            'command': [command],
             'tty': True,
             'detach': True,
             'environment': environment,
         }
 
         # clean all containers not running
         for container in self.docker.containers.list(filters={'status': 'exited'}):
```

### Comparing `conviso-cli-2.1.5.dev9/scripts/shell_completer/flow_bash_completer.sh` & `conviso-cli-2.1.6/scripts/shell_completer/flow_bash_completer.sh`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/scripts/shell_completer/flow_zsh_completer.sh` & `conviso-cli-2.1.6/scripts/shell_completer/flow_zsh_completer.sh`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev9/setup.py` & `conviso-cli-2.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     package_data={'convisoappsec': ['flowcli/vulnerability/rules_schema.json']},
     packages=find_packages(
         exclude=["test*"],
     ),
     install_requires=[
         "GitPython>=3.1.2,<4",
         "click>=7.1.2,<8",
-        "requests>=2.23.0,<3",
+        "requests==2.31.0",
         "urllib3==2.2.0",
         "semantic-version>=2.8.5,<3",
         "docker<=6.1.3",
         "PyYAML==6.0.1",
         "click-log>=0.3.2,<1",
         "transitions>=0.8.7,<1",
         "jsonschema>=2.5.1,<3",
```

