# Comparing `tmp/pulp-gem-0.5.0.tar.gz` & `tmp/pulp-gem-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-gem-0.5.0.tar", last modified: Mon Feb 12 17:40:48 2024, max compression
+gzip compressed data, was "pulp-gem-0.5.1.tar", last modified: Thu May 23 15:07:37 2024, max compression
```

## Comparing `pulp-gem-0.5.0.tar` & `pulp-gem-0.5.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:40:48.913387 pulp-gem-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/COMMITMENT
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-02-12 17:40:48.913387 pulp-gem-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/functest_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:40:48.909387 pulp-gem-0.5.0/pulp_gem/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:40:48.909387 pulp-gem-0.5.0/pulp_gem/app/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:40:48.913387 pulp-gem-0.5.0/pulp_gem/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/migrations/0002_gemrepository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/migrations/0003_move_data_to_new_master_distribution_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/migrations/0004_alter_gemcontent_content_ptr_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/migrations/0005_rename_gemcontent_shallowgemcontent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/migrations/0006_gemremote_excludes_gemremote_includes_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/migrations/0007_DATA_fix_prerelease.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/migrations/0008_gemcontent_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/migrations/0009_check_datarepair.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/migrations/0010_delete_shallowgemcontent.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/migrations/0011_alter_gemcontent_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/migrations/0012_alter_gemdistribution_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/replica.py
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:40:48.913387 pulp-gem-0.5.0/pulp_gem/app/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/tasks/publishing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/tasks/synchronizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/app/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13139 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:40:48.913387 pulp-gem-0.5.0/pulp_gem/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:40:48.913387 pulp-gem-0.5.0/pulp_gem/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:40:48.913387 pulp-gem-0.5.0/pulp_gem/tests/functional/api/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/functional/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_crud_content_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_crud_remotes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_download_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_pull_through.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/functional/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:40:48.913387 pulp-gem-0.5.0/pulp_gem/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/unit/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pulp_gem/tests/unit/test_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:40:48.909387 pulp-gem-0.5.0/pulp_gem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-02-12 17:40:48.000000 pulp-gem-0.5.0/pulp_gem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-02-12 17:40:48.000000 pulp-gem-0.5.0/pulp_gem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 17:40:48.000000 pulp-gem-0.5.0/pulp_gem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-12 17:40:48.000000 pulp-gem-0.5.0/pulp_gem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-12 17:40:48.000000 pulp-gem-0.5.0/pulp_gem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 17:40:48.000000 pulp-gem-0.5.0/pulp_gem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 17:40:48.913387 pulp-gem-0.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1378 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 17:40:42.000000 pulp-gem-0.5.0/unittest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:07:37.347803 pulp-gem-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/COMMITMENT
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-23 15:07:37.347803 pulp-gem-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/functest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:07:37.339803 pulp-gem-0.5.1/pulp_gem/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:07:37.339803 pulp-gem-0.5.1/pulp_gem/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:07:37.343803 pulp-gem-0.5.1/pulp_gem/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/migrations/0002_gemrepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/migrations/0003_move_data_to_new_master_distribution_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/migrations/0004_alter_gemcontent_content_ptr_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/migrations/0005_rename_gemcontent_shallowgemcontent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/migrations/0006_gemremote_excludes_gemremote_includes_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/migrations/0007_DATA_fix_prerelease.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/migrations/0008_gemcontent_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/migrations/0009_check_datarepair.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/migrations/0010_delete_shallowgemcontent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/migrations/0011_alter_gemcontent_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/migrations/0012_alter_gemdistribution_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/replica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:07:37.343803 pulp-gem-0.5.1/pulp_gem/app/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/tasks/publishing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/tasks/synchronizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/app/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13139 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:07:37.343803 pulp-gem-0.5.1/pulp_gem/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:07:37.343803 pulp-gem-0.5.1/pulp_gem/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:07:37.343803 pulp-gem-0.5.1/pulp_gem/tests/functional/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/functional/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_crud_content_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_crud_remotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_download_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_pull_through.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/functional/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:07:37.343803 pulp-gem-0.5.1/pulp_gem/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/unit/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pulp_gem/tests/unit/test_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:07:37.339803 pulp-gem-0.5.1/pulp_gem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-23 15:07:37.000000 pulp-gem-0.5.1/pulp_gem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-23 15:07:37.000000 pulp-gem-0.5.1/pulp_gem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:07:37.000000 pulp-gem-0.5.1/pulp_gem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 15:07:37.000000 pulp-gem-0.5.1/pulp_gem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-23 15:07:37.000000 pulp-gem-0.5.1/pulp_gem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 15:07:37.000000 pulp-gem-0.5.1/pulp_gem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:07:37.347803 pulp-gem-0.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1378 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 15:07:24.000000 pulp-gem-0.5.1/unittest_requirements.txt
```

### Comparing `pulp-gem-0.5.0/CHANGES.rst` & `pulp-gem-0.5.1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,27 @@
     To add a new change log entry, please see
     https://docs.pulpproject.org/en/3.0/nightly/contributing/git.html#changelog-update
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+0.5.1 (2024-05-23)
+==================
+
+Bugfixes
+--------
+
+- Fixed the wrong upper bound for pulpcore version requirement.
+  `#265 <https://github.com/pulp/pulp_gem/issues/265>`__
+
+
+----
+
+
 0.5.0 (2024-02-12)
 ==================
 
 Features
 --------
 
 - Added replica definitions.
```

### Comparing `pulp-gem-0.5.0/COMMITMENT` & `pulp-gem-0.5.1/COMMITMENT`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/COPYRIGHT` & `pulp-gem-0.5.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/LICENSE` & `pulp-gem-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/PKG-INFO` & `pulp-gem-0.5.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pulp-gem
-Version: 0.5.0
+Version: 0.5.1
 Summary: Gemfile plugin for the Pulp Project
 Home-page: https://pulpproject.org/
 Author: Pulp Project Developers
 Author-email: pulp-dev@redhat.com
 License: GPLv2+
 Project-URL: Documentation, https://docs.pulpproject.org/pulp_gem/
 Project-URL: Source, https://github.com/pulp/pulp_gem
 Project-URL: Tracker, https://github.com/pulp/pulp_gem/issues
-Description: # pulp-gem
-        
-        A Pulp plugin to support hosting your own gem.
-        
-        For more information, please see the [documentation](docs/index.rst) or the [Pulp project page](https://pulpproject.org/).
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.8
+License-File: LICENSE
+
+# pulp-gem
+
+A Pulp plugin to support hosting your own gem.
+
+For more information, please see the [documentation](docs/index.rst) or the [Pulp project page](https://pulpproject.org/).
```

### Comparing `pulp-gem-0.5.0/pulp_gem/app/migrations/0001_initial.py` & `pulp-gem-0.5.1/pulp_gem/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/app/migrations/0002_gemrepository.py` & `pulp-gem-0.5.1/pulp_gem/app/migrations/0002_gemrepository.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/app/migrations/0003_move_data_to_new_master_distribution_model.py` & `pulp-gem-0.5.1/pulp_gem/app/migrations/0003_move_data_to_new_master_distribution_model.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/app/migrations/0004_alter_gemcontent_content_ptr_and_more.py` & `pulp-gem-0.5.1/pulp_gem/app/migrations/0004_alter_gemcontent_content_ptr_and_more.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/app/migrations/0005_rename_gemcontent_shallowgemcontent.py` & `pulp-gem-0.5.1/pulp_gem/app/migrations/0005_rename_gemcontent_shallowgemcontent.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/app/migrations/0006_gemremote_excludes_gemremote_includes_and_more.py` & `pulp-gem-0.5.1/pulp_gem/app/migrations/0006_gemremote_excludes_gemremote_includes_and_more.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/app/migrations/0007_DATA_fix_prerelease.py` & `pulp-gem-0.5.1/pulp_gem/app/migrations/0007_DATA_fix_prerelease.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/app/migrations/0009_check_datarepair.py` & `pulp-gem-0.5.1/pulp_gem/app/migrations/0009_check_datarepair.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/app/migrations/0012_alter_gemdistribution_options_and_more.py` & `pulp-gem-0.5.1/pulp_gem/app/migrations/0012_alter_gemdistribution_options_and_more.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/app/models.py` & `pulp-gem-0.5.1/pulp_gem/app/models.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/app/replica.py` & `pulp-gem-0.5.1/pulp_gem/app/replica.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/app/serializers.py` & `pulp-gem-0.5.1/pulp_gem/app/serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/app/tasks/publishing.py` & `pulp-gem-0.5.1/pulp_gem/app/tasks/publishing.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/app/tasks/synchronizing.py` & `pulp-gem-0.5.1/pulp_gem/app/tasks/synchronizing.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/app/viewsets.py` & `pulp-gem-0.5.1/pulp_gem/app/viewsets.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/specs.py` & `pulp-gem-0.5.1/pulp_gem/specs.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_crud_content_unit.py` & `pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_crud_content_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests that perform actions over content unit."""
+
 import pytest
 
 
 def test_upload_content_unit(
     gem_content_api_client,
     gem_content_artifact,
     monitor_task,
```

### Comparing `pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_crud_remotes.py` & `pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_crud_remotes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests that CRUD gem remotes."""
+
 import pytest
 import uuid
 from random import choice
 
 
 from pulpcore.client.pulp_gem import ApiException
 from pulp_gem.tests.functional.constants import DOWNLOAD_POLICIES, GEM_FIXTURE_URL
```

### Comparing `pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_domain.py` & `pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_domain.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_download_content.py` & `pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_download_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests that verify download of content served by Pulp."""
+
 import pytest
 import hashlib
 from random import choice
 from urllib.parse import urljoin
 
 from pulp_gem.tests.functional.constants import DOWNLOAD_POLICIES, GEM_FIXTURE_URL
```

### Comparing `pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_publish.py` & `pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_publish.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests that publish gem plugin repositories."""
+
 import pytest
 from random import choice
 
 
 @pytest.mark.parallel
 def test_publish(
     gem_repository_api_client,
```

### Comparing `pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_pull_through.py` & `pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_pull_through.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_replicate.py` & `pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_replicate.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/tests/functional/api/test_sync.py` & `pulp-gem-0.5.1/pulp_gem/tests/functional/api/test_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests that sync gem plugin repositories."""
+
 import pytest
 
 from pulp_gem.tests.functional.constants import (
     DOWNLOAD_POLICIES,
     GEM_FIXTURE_SUMMARY,
     GEM_INVALID_FIXTURE_URL,
     GEM_FIXTURE_URL,
```

### Comparing `pulp-gem-0.5.0/pulp_gem/tests/functional/conftest.py` & `pulp-gem-0.5.1/pulp_gem/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/tests/functional/constants.py` & `pulp-gem-0.5.1/pulp_gem/tests/functional/constants.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/tests/unit/test_serializers.py` & `pulp-gem-0.5.1/pulp_gem/tests/unit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem/tests/unit/test_spec.py` & `pulp-gem-0.5.1/pulp_gem/tests/unit/test_spec.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pulp_gem.egg-info/PKG-INFO` & `pulp-gem-0.5.1/pulp_gem.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pulp-gem
-Version: 0.5.0
+Version: 0.5.1
 Summary: Gemfile plugin for the Pulp Project
 Home-page: https://pulpproject.org/
 Author: Pulp Project Developers
 Author-email: pulp-dev@redhat.com
 License: GPLv2+
 Project-URL: Documentation, https://docs.pulpproject.org/pulp_gem/
 Project-URL: Source, https://github.com/pulp/pulp_gem
 Project-URL: Tracker, https://github.com/pulp/pulp_gem/issues
-Description: # pulp-gem
-        
-        A Pulp plugin to support hosting your own gem.
-        
-        For more information, please see the [documentation](docs/index.rst) or the [Pulp project page](https://pulpproject.org/).
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.8
+License-File: LICENSE
+
+# pulp-gem
+
+A Pulp plugin to support hosting your own gem.
+
+For more information, please see the [documentation](docs/index.rst) or the [Pulp project page](https://pulpproject.org/).
```

### Comparing `pulp-gem-0.5.0/pulp_gem.egg-info/SOURCES.txt` & `pulp-gem-0.5.1/pulp_gem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/pyproject.toml` & `pulp-gem-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.5.0/setup.py` & `pulp-gem-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = requirements.readlines()
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="pulp-gem",
-    version="0.5.0",
+    version="0.5.1",
     description="Gemfile plugin for the Pulp Project",
     long_description=long_description,
     license="GPLv2+",
     author="Pulp Project Developers",
     author_email="pulp-dev@redhat.com",
     url="https://pulpproject.org/",
     python_requires=">=3.8",
```

