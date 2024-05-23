# Comparing `tmp/dm-cli-1.7.0.tar.gz` & `tmp/dm-cli-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm-cli-1.7.0.tar", last modified: Wed Mar 20 14:54:40 2024, max compression
+gzip compressed data, was "dm-cli-1.7.1.tar", last modified: Thu May 23 11:32:24 2024, max compression
```

## Comparing `dm-cli-1.7.0.tar` & `dm-cli-1.7.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:54:40.043530 dm-cli-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-20 14:54:32.000000 dm-cli-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-03-20 14:54:40.043530 dm-cli-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-03-20 14:54:32.000000 dm-cli-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:54:40.035530 dm-cli-1.7.0/dm_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:54:40.035530 dm-cli-1.7.0/dm_cli/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/bin/dm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:54:40.035530 dm-cli-1.7.0/dm_cli/command_group/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/command_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7561 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/command_group/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/command_group/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:54:40.035530 dm-cli-1.7.0/dm_cli/dmss_api/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:54:40.039530 dm-cli-1.7.0/dm_cli/dmss_api/api/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13451 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/access_control_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/attribute_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/blob_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/blueprint_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/datasource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   182276 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    37828 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/document_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/entity_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/export_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/file_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/health_check_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/lookup_table_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/meta_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16745 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/personal_access_token_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/reference_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api/whoami_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    39037 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17323 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:54:40.043530 dm-cli-1.7.0/dm_cli/dmss_api/model/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/access_control_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/access_level.py
--rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/data_source_information.py
--rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/data_source_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)    11602 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/export_meta_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/get_blueprint_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/pat_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/recipe_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    13879 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/repository_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/storage_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/storage_data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    13218 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model/storage_recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)    82475 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:54:40.043530 dm-cli-1.7.0/dm_cli/dmss_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/dmss_api/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/import_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/import_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/package_tree_from_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:54:40.043530 dm-cli-1.7.0/dm_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/utils/file_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/utils/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/utils/resolve_local_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-03-20 14:54:32.000000 dm-cli-1.7.0/dm_cli/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:54:40.035530 dm-cli-1.7.0/dm_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-03-20 14:54:39.000000 dm-cli-1.7.0/dm_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-03-20 14:54:40.000000 dm-cli-1.7.0/dm_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 14:54:39.000000 dm-cli-1.7.0/dm_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-20 14:54:39.000000 dm-cli-1.7.0/dm_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-20 14:54:39.000000 dm-cli-1.7.0/dm_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-20 14:54:32.000000 dm-cli-1.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 14:54:40.043530 dm-cli-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-20 14:54:32.000000 dm-cli-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:32:24.928588 dm-cli-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-23 11:32:17.000000 dm-cli-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-05-23 11:32:24.928588 dm-cli-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-05-23 11:32:17.000000 dm-cli-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:32:24.920588 dm-cli-1.7.1/dm_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:32:24.920588 dm-cli-1.7.1/dm_cli/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/bin/dm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:32:24.920588 dm-cli-1.7.1/dm_cli/command_group/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/command_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7649 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/command_group/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/command_group/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:32:24.924588 dm-cli-1.7.1/dm_cli/dmss_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:32:24.924588 dm-cli-1.7.1/dm_cli/dmss_api/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13451 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/access_control_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/attribute_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/blob_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/blueprint_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/datasource_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   182276 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37828 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/document_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/entity_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/export_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/file_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/health_check_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/lookup_table_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/meta_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16745 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/personal_access_token_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/reference_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api/whoami_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39037 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17323 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:32:24.928588 dm-cli-1.7.1/dm_cli/dmss_api/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/access_control_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/access_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/data_source_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/data_source_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11602 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/export_meta_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/get_blueprint_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/pat_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/recipe_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13879 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/repository_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/storage_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/storage_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13218 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model/storage_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82475 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:32:24.928588 dm-cli-1.7.1/dm_cli/dmss_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/dmss_api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/import_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/import_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/package_tree_from_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:32:24.928588 dm-cli-1.7.1/dm_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/utils/file_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/utils/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/utils/resolve_local_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-23 11:32:17.000000 dm-cli-1.7.1/dm_cli/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:32:24.920588 dm-cli-1.7.1/dm_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-05-23 11:32:24.000000 dm-cli-1.7.1/dm_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-23 11:32:24.000000 dm-cli-1.7.1/dm_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:32:24.000000 dm-cli-1.7.1/dm_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-23 11:32:24.000000 dm-cli-1.7.1/dm_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-23 11:32:24.000000 dm-cli-1.7.1/dm_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-23 11:32:17.000000 dm-cli-1.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:32:24.928588 dm-cli-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-23 11:32:17.000000 dm-cli-1.7.1/setup.py
```

### Comparing `dm-cli-1.7.0/dm_cli/bin/dm` & `dm-cli-1.7.1/dm_cli/bin/dm`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 def version_callback(print_version: bool):
     if print_version:
         print(VERSION)
         raise typer.Exit()
 
 @app.callback()
 def main(
-        force: bool = typer.Option(False,"--force", "-f", help="Force the operation. Overwriting and potentially deleting data."),
+        force: bool = typer.Option(False, "--force", "-f", help="Force the operation. Overwriting and potentially deleting data."),
         dmss_url: str = typer.Option("http://localhost:5000", "--url", "-u", help="URL to the Data Modelling Storage Service (DMSS)."),
-        token: str = typer.Option("no-token","--token","-t", help="Token for authentication against DMSS."),
-        debug: bool = typer.Option(False, "--debug","-d",help="Print stack trace of suppressed exceptions"),
-        version: Optional[bool] = typer.Option(None, "--version", "-v", callback=version_callback, is_eager=True)
+        token: str = typer.Option("no-token", "--token", "-t", help="Token for authentication against DMSS."),
+        debug: bool = typer.Option(False, "--debug", "-d", help="Print stack trace of suppressed exceptions"),
+        version: Optional[bool] = typer.Option(None, "--version", "-v", callback=version_callback, is_eager=True, help="Print version and exit")
 ):
     """
     Command Line Interface (CLI) tool for working with the Data Modelling Framework.
     This tool is mainly used to upload data source definitions, models and entities, and creating RecipeLink-tables.
     """
     state.force = force
     state.dmss_url = dmss_url
```

### Comparing `dm-cli-1.7.0/dm_cli/command_group/data_source.py` & `dm-cli-1.7.1/dm_cli/command_group/data_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,44 +2,45 @@
 from pathlib import Path
 
 import emoji
 import typer
 from rich import print
 from tenacity import (
     retry,
-    retry_if_not_exception_type,
+    retry_if_exception_type,
     stop_after_attempt,
     wait_random_exponential,
 )
 from typing_extensions import Annotated
 
 from dm_cli.dmss import ApplicationException, dmss_api, dmss_exception_wrapper
+from dm_cli.dmss_api.exceptions import ServiceException
 from dm_cli.import_entity import import_folder_entity, remove_by_path_ignore_404
 from dm_cli.utils.file_structure import get_app_dir_structure, get_json_files_in_dir
 from dm_cli.utils.utils import (
     get_root_packages_in_data_sources,
     validate_entities_in_data_sources,
 )
 
-data_source_app = typer.Typer()
+data_source_app = typer.Typer(help="Import and reset data sources")
 
 
-@data_source_app.command("import", help="Subcommand for working with data sources")
+@data_source_app.command("import", help="Import a single data source definition")
 def import_data_source(
     path: Annotated[Path, typer.Argument(help="Path on local filesystem to a data source JSON file.")]
 ):
     """
     Import a single data source definition to DMSS.
     """
 
     @retry(
         wait=wait_random_exponential(multiplier=1, max=60),
         stop=stop_after_attempt(5),
         reraise=True,
-        retry=retry_if_not_exception_type(ApplicationException),
+        retry=retry_if_exception_type(ServiceException),
     )
     def retry_wrapper():
         data_source_path = Path(path)
         if not data_source_path.is_file():
             raise FileNotFoundError(f"The path '{path}' is not a file.")
 
         print(f"IMPORTING DATA SOURCE '{data_source_path.name}'")
@@ -88,15 +89,15 @@
     path: Annotated[Path, typer.Argument(help="Path on local filesystem to data source folder.")],
     validate_entities: Annotated[
         bool, typer.Option(help="If True, all entities uploaded to DMSS will be validated.")
     ] = True,
 ):
     """
     Initialize the data sources and import all packages.
-    The packages in a data sources will be deleted before data sources are imported.
+    The remote packages in a data source will be deleted before new data sources are imported.
     """
     # Check for presence of expected directories, 'data_sources' and 'data'
     data_sources_dir, data_dir = get_app_dir_structure(Path(path))
 
     data_source_definitions = get_json_files_in_dir(data_sources_dir)
     if not data_source_definitions:
         print(emoji.emojize(f"\t:warning: No data source definitions were found in '{data_sources_dir}'."))
```

### Comparing `dm-cli-1.7.0/dm_cli/command_group/entities.py` & `dm-cli-1.7.1/dm_cli/command_group/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from typing_extensions import Annotated
 
 from dm_cli.dmss import ApplicationException, console, dmss_api, dmss_exception_wrapper
 from dm_cli.dmss_api import ApiException
 from dm_cli.import_entity import import_folder_entity, import_single_entity
 from dm_cli.utils.utils import destination_is_root
 
-entities_app = typer.Typer()
+entities_app = typer.Typer(help="Import, delete, or validate entities and/or blueprints")
 
 
 @entities_app.command("import")
 def import_entity(
     source: Annotated[
         str,
         typer.Argument(
@@ -46,32 +46,29 @@
     def inner_import():
         if source_path.is_dir():
             # If source path ends with "/" or windows "\", import content instead of the package itself
             if source[-1] in ("/", "\\"):
                 print(f"Importing all content from '{source}*' --> '{destination}'")
                 for file in source_path.iterdir():
                     if file.is_file():
-                        import_single_entity(file, destination)
+                        import_single_entity(file, destination, validate)
                         continue
                     import_folder_entity(file, destination, fast)
                     if validate:
                         print(f"Validating entities in: {destination}/{file.name}")
                         dmss_api.validate_existing_entity(f"{destination}/{file.name}")
                 return True
             print(f"Importing PACKAGE '{source}' --> '{destination}'")
             import_folder_entity(source_path, destination, fast)
             if validate:
                 print(f"Validating entities in: {destination}/{source_path.name}")
                 dmss_api.validate_existing_entity(f"{destination}/{source_path.name}")
             return True
         else:
-            import_single_entity(source_path, destination)
-            if validate:
-                print(f"Validating entities in: {destination}/{source_path.name}")
-                dmss_api.validate_existing_entity(f"{destination}/{source_path.name}")
+            import_single_entity(source_path, destination, validate)
             return True
 
     return dmss_exception_wrapper(inner_import)
 
 
 @entities_app.command("validate")
 def validate_entity(
```

### Comparing `dm-cli-1.7.0/dm_cli/dmss.py` & `dm-cli-1.7.1/dm_cli/dmss.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 import requests
 import typer
 from rich.console import Console
 from rich.text import Text
 from tenacity import (
     retry,
-    retry_if_not_exception_type,
+    retry_if_exception_type,
     stop_after_attempt,
     wait_random_exponential,
 )
 
 from dm_cli.dmss_api import ApiException
 from dm_cli.dmss_api.api.default_api import DefaultApi
-from dm_cli.dmss_api.exceptions import NotFoundException
+from dm_cli.dmss_api.exceptions import NotFoundException, ServiceException
 from dm_cli.state import state
 
 console = Console()
 
 dmss_api = DefaultApi()
 
 
@@ -31,15 +31,17 @@
 
     def __init__(
         self,
         message: str = "The requested operation failed",
         debug: str = "An unknown and unhandled exception occurred in the API",
         data: dict = None,
         status: int = 500,
+        type: str = "ApplicationException",
     ):
+        self.type = type
         self.status = status
         self.type = self.__class__.__name__
         self.message = message
         self.debug = debug
         self.data = data
 
     def dict(self):
@@ -52,15 +54,15 @@
         }
 
 
 @retry(
     wait=wait_random_exponential(multiplier=1, max=60),
     stop=stop_after_attempt(5),
     reraise=True,
-    retry=retry_if_not_exception_type(ApplicationException),
+    retry=retry_if_exception_type(ServiceException),
 )
 def export(absolute_document_ref: str):
     """Call export endpoint from DMSS to download document(s) as zip.
 
     The reason dmss_api cannot be used directly is that there were some issues with interpreting the JSON schema,
     which caused the export function in the generated DMSS api to not work properly.
     """
```

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/__init__.py` & `dm-cli-1.7.1/dm_cli/dmss_api/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/access_control_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/access_control_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/attribute_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/attribute_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/blob_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/blob_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/blueprint_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/blueprint_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/datasource_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/datasource_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/default_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/default_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/document_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/document_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/entity_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/entity_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/export_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/export_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/file_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/file_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/health_check_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/health_check_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/lookup_table_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/lookup_table_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/meta_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/meta_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/personal_access_token_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/personal_access_token_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/reference_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/reference_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/search_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/search_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api/whoami_api.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api/whoami_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/api_client.py` & `dm-cli-1.7.1/dm_cli/dmss_api/api_client.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/configuration.py` & `dm-cli-1.7.1/dm_cli/dmss_api/configuration.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/exceptions.py` & `dm-cli-1.7.1/dm_cli/dmss_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/access_control_list.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/access_control_list.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/access_level.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/access_level.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/acl.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/acl.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/data_source_information.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/data_source_information.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/data_source_request.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/data_source_request.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/dependency.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/dependency.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/entity.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/entity.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/error_response.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/error_response.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/export_meta_response.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/export_meta_response.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/get_blueprint_response.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/get_blueprint_response.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/lookup.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/lookup.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/pat_data.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/pat_data.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/recipe.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/recipe.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/recipe_attribute.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/recipe_attribute.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/reference.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/reference.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/reference_entity.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/reference_entity.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/repository.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/repository.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/repository_type.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/repository_type.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/storage_attribute.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/storage_attribute.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/storage_data_types.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/storage_data_types.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model/storage_recipe.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model/storage_recipe.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/model_utils.py` & `dm-cli-1.7.1/dm_cli/dmss_api/model_utils.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/models/__init__.py` & `dm-cli-1.7.1/dm_cli/dmss_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/dmss_api/rest.py` & `dm-cli-1.7.1/dm_cli/dmss_api/rest.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/domain.py` & `dm-cli-1.7.1/dm_cli/domain.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/enums.py` & `dm-cli-1.7.1/dm_cli/enums.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/import_entity.py` & `dm-cli-1.7.1/dm_cli/import_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import io
 import json
 from json import JSONDecodeError
 from pathlib import Path
 from zipfile import ZipFile
 
+from requests import Response
 from rich import print
 from tenacity import (
     retry,
+    retry_if_exception_type,
     retry_if_not_exception_type,
+    retry_if_not_result,
     stop_after_attempt,
     wait_random_exponential,
 )
 
 from .dmss import ApplicationException, dmss_api
-from .dmss_api.exceptions import NotFoundException
+from .dmss_api.exceptions import ApiException, NotFoundException, ServiceException
 from .import_package import import_package_tree
 from .package_tree_from_zip import package_tree_from_zip
 from .state import state
 from .utils.reference import replace_relative_references
 from .utils.utils import (
     concat_dependencies,
     console,
@@ -27,15 +30,15 @@
 from .utils.zip import zip_all
 
 
 @retry(
     wait=wait_random_exponential(multiplier=1, max=60),
     stop=stop_after_attempt(5),
     reraise=True,
-    retry=retry_if_not_exception_type(ApplicationException),
+    retry=retry_if_exception_type(ServiceException),
 )
 def import_document(source_path: Path, destination: str, document: dict):
     remote_dependencies = dmss_api.export_meta(destination)
     old_dependencies = {dependency["alias"]: dependency for dependency in remote_dependencies.get("dependencies", [])}
 
     dependencies = concat_dependencies(
         new_dependencies=document.get("_meta_", {}).get("dependencies", []),
@@ -50,22 +53,27 @@
     dmss_api.document_add(
         destination,
         document_json_str,
         files=[],
     )
 
 
-def import_single_entity(source_path: Path, destination: str):
+def import_single_entity(source_path: Path, destination: str, validate: bool = False):
     ensure_package_structure(Path(destination))
     print(f"Importing ENTITY '{source_path.name}' --> '{destination}'")
 
     try:  # Load the JSON document
         with open(source_path, "r") as fh:
             if Path(source_path).suffix == ".json":
-                import_document(source_path, destination, json.load(fh))
+                content = json.load(fh)
+                if validate:
+                    print(f"Validating {source_path}", end="")
+                    dmss_api.validate_entity(content)
+                    print(" [green]✓[/green]")
+                import_document(source_path, destination, content)
             else:
                 print(f"Unsupported file type {source_path}")
     except JSONDecodeError:
         raise Exception(f"Failed to load the file '{source_path.name}' as a JSON document")
 
 
 def remove_by_path_ignore_404(target: str):
@@ -75,15 +83,15 @@
         pass
 
 
 @retry(
     wait=wait_random_exponential(multiplier=1, max=60),
     stop=stop_after_attempt(5),
     reraise=True,
-    retry=retry_if_not_exception_type(ApplicationException),
+    retry=retry_if_exception_type(ServiceException),
 )
 def import_folder_entity(
     source_path: Path,
     destination: str,
     raw_package_import: bool = False,
     resolve_local_ids: bool = False,
 ) -> dict:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dm-cli-1.7.0/dm_cli/import_package.py` & `dm-cli-1.7.1/dm_cli/import_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from pathlib import Path
 from typing import Dict, List
 from uuid import uuid4
 
 from rich.console import Console
 from tenacity import (
     retry,
+    retry_if_exception_type,
     retry_if_not_exception_type,
     stop_after_attempt,
     wait_random_exponential,
 )
 from tqdm import tqdm
 
 from .dmss import ApplicationException, dmss_api
+from .dmss_api.exceptions import ServiceException
 from .domain import Dependency, File, Package
 from .utils.reference import replace_relative_references
 from .utils.resolve_local_ids import resolve_local_ids_in_document
 from .utils.utils import concat_dependencies, replace_global_addresses
 
 console = Console()
 
@@ -92,15 +94,15 @@
     import_package_content(package, data_source, destination, resolve_local_ids)
 
 
 @retry(
     wait=wait_random_exponential(multiplier=1, max=60),
     stop=stop_after_attempt(5),
     reraise=True,
-    retry=retry_if_not_exception_type(ApplicationException),
+    retry=retry_if_exception_type(ServiceException),
 )
 def import_package_content(package: Package, data_source: str, destination: str, resolve_local_ids: bool) -> None:
     files: List[File] = []
     entities: List[dict] = []
     package.traverse_documents(
         lambda document, **kwargs: files.append(document) if isinstance(document, File) else entities.append(document)
     )
```

### Comparing `dm-cli-1.7.0/dm_cli/package_tree_from_zip.py` & `dm-cli-1.7.1/dm_cli/package_tree_from_zip.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/utils/file_structure.py` & `dm-cli-1.7.1/dm_cli/utils/file_structure.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/utils/reference.py` & `dm-cli-1.7.1/dm_cli/utils/reference.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/utils/resolve_local_ids.py` & `dm-cli-1.7.1/dm_cli/utils/resolve_local_ids.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/utils/utils.py` & `dm-cli-1.7.1/dm_cli/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli/utils/zip.py` & `dm-cli-1.7.1/dm_cli/utils/zip.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/dm_cli.egg-info/SOURCES.txt` & `dm-cli-1.7.1/dm_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dm-cli-1.7.0/setup.py` & `dm-cli-1.7.1/setup.py`

 * *Files identical despite different names*

