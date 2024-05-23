# Comparing `tmp/pulp_gem-client-0.5.0.tar.gz` & `tmp/pulp_gem-client-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp_gem-client-0.5.0.tar", last modified: Mon Feb 12 17:43:52 2024, max compression
+gzip compressed data, was "pulp_gem-client-0.5.1.tar", last modified: Thu May 23 15:10:40 2024, max compression
```

## Comparing `pulp_gem-client-0.5.0.tar` & `pulp_gem-client-0.5.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:52.132483 pulp_gem-client-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-12 17:43:52.132483 pulp_gem-client-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:52.120483 pulp_gem-client-0.5.0/pulp_gem_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-12 17:43:52.000000 pulp_gem-client-0.5.0/pulp_gem_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-02-12 17:43:52.000000 pulp_gem-client-0.5.0/pulp_gem_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 17:43:52.000000 pulp_gem-client-0.5.0/pulp_gem_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-12 17:43:52.000000 pulp_gem-client-0.5.0/pulp_gem_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 17:43:52.000000 pulp_gem-client-0.5.0/pulp_gem_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:52.120483 pulp_gem-client-0.5.0/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:52.120483 pulp_gem-client-0.5.0/pulpcore/client/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:52.120483 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:52.120483 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25540 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api/content_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    83549 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api/distributions_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    54912 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api/publications_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    84765 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api/remotes_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    98540 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api/repositories_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    33743 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api/repositories_gem_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26274 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13958 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:52.128483 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_content.py
--rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_content_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_publication.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_publication_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    28909 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    26296 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_remote_response_hidden_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/my_permissions_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/nested_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/nested_role_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/object_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_content_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_publication_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/patchedgem_gem_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    29302 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/patchedgem_gem_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     7724 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/patchedgem_gem_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/repair.py
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/set_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/set_label_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/unset_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/unset_label_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12311 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-12 17:43:52.132483 pulp_gem-client-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:52.132483 pulp_gem-client-0.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_content_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_distributions_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_gem_gem_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_gem_gem_content_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_gem_gem_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_gem_gem_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_gem_gem_publication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_gem_gem_publication_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_gem_gem_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_gem_gem_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_gem_gem_remote_response_hidden_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_gem_gem_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_gem_gem_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_my_permissions_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_nested_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_nested_role_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_object_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_paginatedgem_gem_content_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_paginatedgem_gem_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_paginatedgem_gem_publication_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_paginatedgem_gem_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_paginatedgem_gem_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_patchedgem_gem_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_patchedgem_gem_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_patchedgem_gem_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_publications_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_remotes_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_repair.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_repositories_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_repositories_gem_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_set_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_set_label_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_unset_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-02-12 17:43:51.000000 pulp_gem-client-0.5.0/test/test_unset_label_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:10:40.348628 pulp_gem-client-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-23 15:10:40.348628 pulp_gem-client-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:10:40.336628 pulp_gem-client-0.5.1/pulp_gem_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-23 15:10:40.000000 pulp_gem-client-0.5.1/pulp_gem_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-23 15:10:40.000000 pulp_gem-client-0.5.1/pulp_gem_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:10:40.000000 pulp_gem-client-0.5.1/pulp_gem_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-23 15:10:40.000000 pulp_gem-client-0.5.1/pulp_gem_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 15:10:40.000000 pulp_gem-client-0.5.1/pulp_gem_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:10:40.336628 pulp_gem-client-0.5.1/pulpcore/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-23 15:10:40.000000 pulp_gem-client-0.5.1/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:10:40.336628 pulp_gem-client-0.5.1/pulpcore/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-23 15:10:40.000000 pulp_gem-client-0.5.1/pulpcore/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:10:40.336628 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:10:40.340628 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25540 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api/content_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83549 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api/distributions_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54912 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api/publications_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84765 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api/remotes_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98540 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api/repositories_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33743 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api/repositories_gem_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26274 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13958 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:10:40.344628 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_content_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_publication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_publication_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28909 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26296 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_remote_response_hidden_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/my_permissions_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/nested_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/nested_role_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/object_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_content_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_publication_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/patchedgem_gem_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29302 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/patchedgem_gem_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7724 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/patchedgem_gem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/set_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/set_label_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/unset_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/unset_label_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12311 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-23 15:10:40.348628 pulp_gem-client-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:10:40.348628 pulp_gem-client-0.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_content_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_distributions_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_gem_gem_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_gem_gem_content_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_gem_gem_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_gem_gem_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_gem_gem_publication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_gem_gem_publication_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_gem_gem_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_gem_gem_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_gem_gem_remote_response_hidden_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_gem_gem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_gem_gem_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_my_permissions_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_nested_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_nested_role_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_object_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_paginatedgem_gem_content_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_paginatedgem_gem_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_paginatedgem_gem_publication_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_paginatedgem_gem_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_paginatedgem_gem_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_patchedgem_gem_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_patchedgem_gem_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_patchedgem_gem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_publications_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_remotes_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_repositories_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_repositories_gem_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_set_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_set_label_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_unset_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-23 15:10:39.000000 pulp_gem-client-0.5.1/test/test_unset_label_response.py
```

### Comparing `pulp_gem-client-0.5.0/README.md` & `pulp_gem-client-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pulp_gem-client
 Fetch, Upload, Organize, and Distribute Software Packages
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v3
-- Package version: 0.5.0
+- Package version: 0.5.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pulpproject.org](https://pulpproject.org)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `pulp_gem-client-0.5.0/pulp_gem_client.egg-info/SOURCES.txt` & `pulp_gem-client-0.5.1/pulp_gem_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/__init__.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: pulp-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 # import apis into sdk package
 from pulpcore.client.pulp_gem.api.content_gem_api import ContentGemApi
 from pulpcore.client.pulp_gem.api.distributions_gem_api import DistributionsGemApi
 from pulpcore.client.pulp_gem.api.publications_gem_api import PublicationsGemApi
 from pulpcore.client.pulp_gem.api.remotes_gem_api import RemotesGemApi
 from pulpcore.client.pulp_gem.api.repositories_gem_api import RepositoriesGemApi
```

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api/__init__.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api/content_gem_api.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api/content_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api/distributions_gem_api.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api/distributions_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api/publications_gem_api.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api/publications_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api/remotes_gem_api.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api/remotes_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api/repositories_gem_api.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api/repositories_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api/repositories_gem_versions_api.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api/repositories_gem_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/api_client.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.5.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/configuration.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3\n"\
-               "SDK Package Version: 0.5.0".\
+               "SDK Package Version: 0.5.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/exceptions.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/__init__.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/async_operation_response.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/content_summary_response.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_content.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_content.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_content_response.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_content_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_distribution.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_distribution_response.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_publication.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_publication.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_publication_response.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_publication_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_remote.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_remote_response.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_remote_response_hidden_fields.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_remote_response_hidden_fields.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_repository.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/gem_gem_repository_response.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/gem_gem_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/my_permissions_response.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/my_permissions_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/nested_role.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/nested_role.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/nested_role_response.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/nested_role_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/object_roles_response.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/object_roles_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/paginated_repository_version_response_list.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_content_response_list.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_content_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_distribution_response_list.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_publication_response_list.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_publication_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_remote_response_list.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_repository_response_list.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/patchedgem_gem_distribution.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/patchedgem_gem_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/patchedgem_gem_remote.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/patchedgem_gem_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/patchedgem_gem_repository.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/patchedgem_gem_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/policy_enum.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/repair.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/repair.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/repository_add_remove_content.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/repository_sync_url.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/repository_version_response.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/set_label.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/set_label.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/set_label_response.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/set_label_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/unset_label.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/unset_label.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/models/unset_label_response.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/models/unset_label_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/pulpcore/client/pulp_gem/rest.py` & `pulp_gem-client-0.5.1/pulpcore/client/pulp_gem/rest.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/setup.py` & `pulp_gem-client-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pulp_gem-client"
-VERSION = "0.5.0"
+VERSION = "0.5.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pulp_gem-client-0.5.0/test/test_async_operation_response.py` & `pulp_gem-client-0.5.1/test/test_async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_content_gem_api.py` & `pulp_gem-client-0.5.1/test/test_content_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_content_summary_response.py` & `pulp_gem-client-0.5.1/test/test_content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_distributions_gem_api.py` & `pulp_gem-client-0.5.1/test/test_distributions_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_gem_gem_content.py` & `pulp_gem-client-0.5.1/test/test_gem_gem_content.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_gem_gem_content_response.py` & `pulp_gem-client-0.5.1/test/test_gem_gem_content_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_gem_gem_distribution.py` & `pulp_gem-client-0.5.1/test/test_gem_gem_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_gem_gem_distribution_response.py` & `pulp_gem-client-0.5.1/test/test_gem_gem_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_gem_gem_publication.py` & `pulp_gem-client-0.5.1/test/test_gem_gem_publication.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_gem_gem_publication_response.py` & `pulp_gem-client-0.5.1/test/test_gem_gem_publication_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_gem_gem_remote.py` & `pulp_gem-client-0.5.1/test/test_gem_gem_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_gem_gem_remote_response.py` & `pulp_gem-client-0.5.1/test/test_gem_gem_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_gem_gem_remote_response_hidden_fields.py` & `pulp_gem-client-0.5.1/test/test_gem_gem_remote_response_hidden_fields.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_gem_gem_repository.py` & `pulp_gem-client-0.5.1/test/test_gem_gem_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_gem_gem_repository_response.py` & `pulp_gem-client-0.5.1/test/test_gem_gem_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_my_permissions_response.py` & `pulp_gem-client-0.5.1/test/test_my_permissions_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_nested_role.py` & `pulp_gem-client-0.5.1/test/test_nested_role.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_nested_role_response.py` & `pulp_gem-client-0.5.1/test/test_nested_role_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_object_roles_response.py` & `pulp_gem-client-0.5.1/test/test_object_roles_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_paginated_repository_version_response_list.py` & `pulp_gem-client-0.5.1/test/test_paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_paginatedgem_gem_content_response_list.py` & `pulp_gem-client-0.5.1/test/test_paginatedgem_gem_content_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_paginatedgem_gem_distribution_response_list.py` & `pulp_gem-client-0.5.1/test/test_paginatedgem_gem_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_paginatedgem_gem_publication_response_list.py` & `pulp_gem-client-0.5.1/test/test_paginatedgem_gem_publication_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_paginatedgem_gem_remote_response_list.py` & `pulp_gem-client-0.5.1/test/test_paginatedgem_gem_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_paginatedgem_gem_repository_response_list.py` & `pulp_gem-client-0.5.1/test/test_paginatedgem_gem_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_patchedgem_gem_distribution.py` & `pulp_gem-client-0.5.1/test/test_patchedgem_gem_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_patchedgem_gem_remote.py` & `pulp_gem-client-0.5.1/test/test_patchedgem_gem_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_patchedgem_gem_repository.py` & `pulp_gem-client-0.5.1/test/test_patchedgem_gem_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_policy_enum.py` & `pulp_gem-client-0.5.1/test/test_policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_publications_gem_api.py` & `pulp_gem-client-0.5.1/test/test_publications_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_remotes_gem_api.py` & `pulp_gem-client-0.5.1/test/test_remotes_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_repair.py` & `pulp_gem-client-0.5.1/test/test_repair.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_repositories_gem_api.py` & `pulp_gem-client-0.5.1/test/test_repositories_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_repositories_gem_versions_api.py` & `pulp_gem-client-0.5.1/test/test_repositories_gem_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_repository_add_remove_content.py` & `pulp_gem-client-0.5.1/test/test_repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_repository_sync_url.py` & `pulp_gem-client-0.5.1/test/test_repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_repository_version_response.py` & `pulp_gem-client-0.5.1/test/test_repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_set_label.py` & `pulp_gem-client-0.5.1/test/test_set_label.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_set_label_response.py` & `pulp_gem-client-0.5.1/test/test_set_label_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_unset_label.py` & `pulp_gem-client-0.5.1/test/test_unset_label.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.5.0/test/test_unset_label_response.py` & `pulp_gem-client-0.5.1/test/test_unset_label_response.py`

 * *Files identical despite different names*

