# Comparing `tmp/fastr-3.3.1.tar.gz` & `tmp/fastr-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastr-3.3.1.tar", last modified: Thu Oct 13 07:48:43 2022, max compression
+gzip compressed data, was "dist/fastr-3.4.0.tar", last modified: Thu May 23 10:39:24 2024, max compression
```

## Comparing `fastr-3.3.1.tar` & `fastr-3.4.0.tar`

### file list

```diff
@@ -1,1007 +1,987 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/
--rw-rw-rw-   0 root         (0) root         (0)    10174 2022-10-13 07:48:29.000000 fastr-3.3.1/APACHE-LICENSE-2.0
--rw-rw-rw-   0 root         (0) root         (0)      684 2022-10-13 07:48:29.000000 fastr-3.3.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      565 2022-10-13 07:48:29.000000 fastr-3.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2025 2022-10-13 07:48:43.000000 fastr-3.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      821 2022-10-13 07:48:29.000000 fastr-3.3.1/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/
--rw-rw-rw-   0 root         (0) root         (0)     2632 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/abc/
--rw-rw-rw-   0 root         (0) root         (0)    12110 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/abc/basemanager.py
--rw-rw-rw-   0 root         (0) root         (0)     6410 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/abc/baseplugin.py
--rw-rw-rw-   0 root         (0) root         (0)     8792 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/abc/basepluginmanager.py
--rw-rw-rw-   0 root         (0) root         (0)    11370 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/abc/serializable.py
--rw-rw-rw-   0 root         (0) root         (0)    10372 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/abc/updateable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/api/
--rw-rw-rw-   0 root         (0) root         (0)    27859 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/core/
--rw-rw-rw-   0 root         (0) root         (0)      891 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20756 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/cardinality.py
--rw-rw-rw-   0 root         (0) root         (0)     5826 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/dimension.py
--rw-rw-rw-   0 root         (0) root         (0)     6732 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/interface.py
--rw-rw-rw-   0 root         (0) root         (0)    14694 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/ioplugin.py
--rw-rw-rw-   0 root         (0) root         (0)     7499 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/provenance.py
--rw-rw-rw-   0 root         (0) root         (0)     6075 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/resourcelimit.py
--rw-rw-rw-   0 root         (0) root         (0)    39605 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/samples.py
--rw-rw-rw-   0 root         (0) root         (0)    10351 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/core/test/
--rw-rw-rw-   0 root         (0) root         (0)      696 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/test/test_datatypemanager.py
--rw-rw-rw-   0 root         (0) root         (0)     5357 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/test/test_dimension.py
--rw-rw-rw-   0 root         (0) root         (0)    13348 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/test/test_samples.py
--rw-rw-rw-   0 root         (0) root         (0)     3230 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/test/test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     4587 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/test/test_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4292 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/test/test_vfs.py
--rwxrwxrwx   0 root         (0) root         (0)    36127 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/tool.py
--rwxrwxrwx   0 root         (0) root         (0)     7152 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/version.py
--rw-rw-rw-   0 root         (0) root         (0)    12813 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/core/vfs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/data/
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6389 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/data/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/datatypes/
--rw-rw-rw-   0 root         (0) root         (0)    45610 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/datatypes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/doc/
--rw-rw-rw-   0 root         (0) root         (0)     4602 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     9637 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/conf.py
--rwxrwxrwx   0 root         (0) root         (0)     1203 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/doc_clean.py
--rwxrwxrwx   0 root         (0) root         (0)     1268 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/doc_generate.py
--rw-rw-rw-   0 root         (0) root         (0)     1709 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/generate_cmd.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/generate_config.py
--rwxrwxrwx   0 root         (0) root         (0)    10748 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/generate_modules.py
--rwxrwxrwx   0 root         (0) root         (0)     5931 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/generate_plugins.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/index.template
--rw-rw-rw-   0 root         (0) root         (0)     4687 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/doc/static/
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/static/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)    14111 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/static/development.rst
--rw-rw-rw-   0 root         (0) root         (0)    11428 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/static/file_description.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/doc/static/images/
--rw-rw-rw-   0 root         (0) root         (0)    12938 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/static/images/fastr_core.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/doc/static/images/tools/
--rw-rw-rw-   0 root         (0) root         (0)    40801 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/static/images/tools/tooldefresolveflowchart.png
--rw-rw-rw-   0 root         (0) root         (0)     5507 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/static/introduction.rst
--rw-rw-rw-   0 root         (0) root         (0)    11619 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/static/quick_start.rst
--rw-rw-rw-   0 root         (0) root         (0)     1689 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/static/tools.rst
--rw-rw-rw-   0 root         (0) root         (0)    48948 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/doc/static/user_manual.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/
--rw-rw-rw-   0 root         (0) root         (0)     1769 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/__generate_reference__.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2261 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/add_ints.py
--rw-rw-rw-   0 root         (0) root         (0)     2277 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/add_ints_missing.py
--rw-rw-rw-   0 root         (0) root         (0)     2021 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/add_ints_s3.py
--rw-rw-rw-   0 root         (0) root         (0)     2995 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/advanced_linking.py
--rw-rw-rw-   0 root         (0) root         (0)     2011 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/auto_prefix.py
--rw-rw-rw-   0 root         (0) root         (0)     2851 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/chunk_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1700 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/collapse.py
--rw-rw-rw-   0 root         (0) root         (0)     1730 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/collapse_expand.py
--rw-rw-rw-   0 root         (0) root         (0)     2524 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/cross_validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/add_ints/
--rw-rw-rw-   0 root         (0) root         (0)        2 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/add_ints/value
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/add_ints/values
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/add_ints/values_duplicate
--rw-rw-rw-   0 root         (0) root         (0)       12 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/hello.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/images/
--rw-rw-rw-   0 root         (0) root         (0)      279 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/images/mrwhite.mhd
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/images/mrwhite.raw
--rw-rw-rw-   0 root         (0) root         (0)      289 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/images/mrwhite_duplicate.mhd
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/images/mrwhite_duplicate.raw
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/
--rw-rw-rw-   0 root         (0) root         (0)     3284 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/id_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/id_1_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/id_1_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/id_1_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/id_1_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/id_1_1/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/id_1_1/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/id_1_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/id_1_2/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/id_1_2/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/id_1_3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/id_1_3/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/sink/id_1_3/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/
--rw-rw-rw-   0 root         (0) root         (0)     9335 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)     3716 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      119 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/1/
--rw-rw-rw-   0 root         (0) root         (0)     3716 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/1/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/1/result.json
--rw-rw-rw-   0 root         (0) root         (0)      119 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/1/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/0/
--rw-rw-rw-   0 root         (0) root         (0)     4013 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/1/
--rw-rw-rw-   0 root         (0) root         (0)     4013 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/1/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/1/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/1/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/0/
--rw-rw-rw-   0 root         (0) root         (0)     4013 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/1/
--rw-rw-rw-   0 root         (0) root         (0)     4013 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/1/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/1/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/1/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/0/
--rw-rw-rw-   0 root         (0) root         (0)     4013 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/1/
--rw-rw-rw-   0 root         (0) root         (0)     4013 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/1/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/1/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/1/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/0/
--rw-rw-rw-   0 root         (0) root         (0)     4013 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/1/
--rw-rw-rw-   0 root         (0) root         (0)     4013 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/1/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/1/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/1/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)     5228 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      119 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/1/
--rw-rw-rw-   0 root         (0) root         (0)     5228 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/1/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/1/result.json
--rw-rw-rw-   0 root         (0) root         (0)      119 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/1/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/2/
--rw-rw-rw-   0 root         (0) root         (0)     5228 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/2/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/2/result.json
--rw-rw-rw-   0 root         (0) root         (0)      119 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/2/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/3/
--rw-rw-rw-   0 root         (0) root         (0)     5228 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/3/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/3/result.json
--rw-rw-rw-   0 root         (0) root         (0)      119 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/3/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/4/
--rw-rw-rw-   0 root         (0) root         (0)     5228 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/4/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/4/result.json
--rw-rw-rw-   0 root         (0) root         (0)      119 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/4/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/5/
--rw-rw-rw-   0 root         (0) root         (0)     5228 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/5/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/5/result.json
--rw-rw-rw-   0 root         (0) root         (0)      119 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/5/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/6/
--rw-rw-rw-   0 root         (0) root         (0)     5228 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/6/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/6/result.json
--rw-rw-rw-   0 root         (0) root         (0)      119 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/6/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/0/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/1/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/1/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/1/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/1/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/2/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/2/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/2/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/2/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/3/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/3/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/3/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/3/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/4/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/4/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/4/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/4/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/5/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/5/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/5/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/5/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/6/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/6/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/6/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/6/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/0/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/1/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/1/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/1/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/1/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/2/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/2/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/2/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/2/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/3/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/3/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/3/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/3/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/4/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/4/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/4/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/4/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/5/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/5/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/5/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/5/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/6/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/6/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/6/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/6/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/0/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/1/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/1/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/1/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/1/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/2/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/2/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/2/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/2/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/3/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/3/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/3/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/3/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/4/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/4/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/4/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/4/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/5/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/5/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/5/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/5/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/6/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/6/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/6/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/6/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/0/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/1/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/1/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/1/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/1/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/2/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/2/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/2/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/2/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/3/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/3/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/3/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/3/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/4/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/4/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/4/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/4/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/5/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/5/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/5/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/5/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/6/
--rw-rw-rw-   0 root         (0) root         (0)     5546 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/6/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/6/result.json
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/6/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/
--rw-rw-rw-   0 root         (0) root         (0)     9793 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)     4238 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_0/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_0/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      122 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_0/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_1/0/
--rw-rw-rw-   0 root         (0) root         (0)     4238 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_1/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_1/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      122 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_1/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_2/0/
--rw-rw-rw-   0 root         (0) root         (0)     4238 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_2/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_2/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      122 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_2/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)     4166 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_0/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_0/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      122 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_0/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_1/0/
--rw-rw-rw-   0 root         (0) root         (0)     4166 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_1/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_1/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      122 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_1/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_2/0/
--rw-rw-rw-   0 root         (0) root         (0)     4166 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_2/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_2/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      122 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_2/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)     4238 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_0/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_0/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      122 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_0/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_1/0/
--rw-rw-rw-   0 root         (0) root         (0)     4238 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_1/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_1/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      122 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_1/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_2/0/
--rw-rw-rw-   0 root         (0) root         (0)     4238 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_2/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_2/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      122 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_2/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)     4166 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_0/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_0/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      122 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_0/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_1/0/
--rw-rw-rw-   0 root         (0) root         (0)     4166 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_1/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_1/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      122 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_1/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_2/0/
--rw-rw-rw-   0 root         (0) root         (0)     4166 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_2/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_2/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      122 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_2/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/
--rw-rw-rw-   0 root         (0) root         (0)     7258 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)      149 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_0/0/
--rw-rw-rw-   0 root         (0) root         (0)     3843 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_0/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_0/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_0/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_1/0/
--rw-rw-rw-   0 root         (0) root         (0)     3843 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_1/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_1/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_1/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_2/0/
--rw-rw-rw-   0 root         (0) root         (0)     3843 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_2/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_2/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_2/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_3/0/
--rw-rw-rw-   0 root         (0) root         (0)     3843 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_3/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_3/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_3/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_0/0/
--rw-rw-rw-   0 root         (0) root         (0)     3849 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_0/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_0/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_0/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_1/0/
--rw-rw-rw-   0 root         (0) root         (0)     3849 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_1/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_1/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_1/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_2/0/
--rw-rw-rw-   0 root         (0) root         (0)     3849 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_2/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_2/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_2/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_3/0/
--rw-rw-rw-   0 root         (0) root         (0)     3849 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_3/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_3/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_3/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1427 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)      140 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/1/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/1/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/10/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/10/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/11/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/11/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/2/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/2/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/3/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/3/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/4/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/4/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/5/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/5/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/6/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/6/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/7/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/7/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/8/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/8/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/9/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/sink/all/9/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1447 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)      140 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__0/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__0/1/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__0/1/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__0/2/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__0/2/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__1/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__1/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__1/1/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__1/1/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__1/2/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__1/2/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__2/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__2/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__2/1/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__2/1/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__2/2/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__2/2/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__3/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__3/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__3/1/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__3/1/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__3/2/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/sink/all__3/2/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/
--rw-rw-rw-   0 root         (0) root         (0)     7261 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)       91 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/id_0__fold_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/id_0__fold_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/id_0__fold_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/id_1__fold_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/id_1__fold_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/id_1__fold_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/id_2__fold_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/id_2__fold_1/0/
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/id_2__fold_1/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/id_3__fold_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/id_3__fold_1/0/
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/id_3__fold_1/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/id_4__fold_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/id_4__fold_2/0/
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/sink/id_4__fold_2/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1403 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)      140 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_a__0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_a__0/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_a__0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_a__1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_a__1/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_a__1/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_a__2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_a__2/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_a__2/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_a__3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_a__3/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_a__3/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_b__0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_b__0/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_b__0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_b__1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_b__1/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_b__1/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_b__2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_b__2/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_b__2/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_b__3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_b__3/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_b__3/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_c__0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_c__0/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_c__0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_c__1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_c__1/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_c__1/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_c__2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_c__2/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_c__2/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_c__3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_c__3/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/expand_0.0/sink/sample_c__3/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_macro_top_level_0.0/
--rw-rw-rw-   0 root         (0) root         (0)    23146 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_macro_top_level_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)      148 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_macro_top_level_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_macro_top_level_0.0/sink/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_macro_top_level_0.0/sink/sample_1_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_macro_top_level_0.0/sink/sample_1_0/0/
--rw-rw-rw-   0 root         (0) root         (0)     3854 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_macro_top_level_0.0/sink/sample_1_0/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_macro_top_level_0.0/sink/sample_1_0/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      131 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_macro_top_level_0.0/sink/sample_1_0/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/
--rw-rw-rw-   0 root         (0) root         (0)    14172 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)      149 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_1/sample_1_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_1/sample_1_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_1/sample_1_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_1/sample_1_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_1/sample_1_2/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_1/sample_1_2/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_2/sample_1_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_2/sample_1_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_2/sample_1_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_2/sample_1_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_2/sample_1_1/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_2/sample_1_1/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_3/sample_1_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_3/sample_1_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_3/sample_1_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/1/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/1/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/2/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/2/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/3/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/3/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/4/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/4/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/5/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/5/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/6/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/6/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/7/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/7/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/8/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/8/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_5/sample_1_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_5/sample_1_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/sink_5/sample_1_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/file_copy_0.0/
--rw-rw-rw-   0 root         (0) root         (0)     2439 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/file_copy_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)      108 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/file_copy_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/file_copy_0.0/sink/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/file_copy_0.0/sink/id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/file_copy_0.0/sink/id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       12 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/file_copy_0.0/sink/id_0/0/hello.txt
--rw-rw-rw-   0 root         (0) root         (0)      100 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/file_copy_0.0/sink/id_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/
--rw-rw-rw-   0 root         (0) root         (0)     3512 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_0__id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_0__id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_0__id_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_0__id_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_0__id_1/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_0__id_1/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_0__id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_0__id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_0__id_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_0__id_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_0__id_1/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_0__id_1/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_1__id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_1__id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_1__id_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_1__id_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_1__id_1/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_1__id_1/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_2__id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_2__id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_2__id_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_2__id_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_2__id_1/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_2__id_1/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_3__id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_3__id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_3__id_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_3__id_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_3__id_1/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/sink/id_1_3__id_1/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/
--rw-rw-rw-   0 root         (0) root         (0)     9267 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)      114 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)     4045 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_0/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_0/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_0/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_1/0/
--rw-rw-rw-   0 root         (0) root         (0)     4045 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_1/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_1/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_1/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_2/0/
--rw-rw-rw-   0 root         (0) root         (0)     4045 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_2/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_2/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_2/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_3/0/
--rw-rw-rw-   0 root         (0) root         (0)     4045 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_3/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_3/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_3/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)     4045 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_0/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_0/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_0/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_1/0/
--rw-rw-rw-   0 root         (0) root         (0)     4045 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_1/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_1/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_1/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_2/0/
--rw-rw-rw-   0 root         (0) root         (0)     4045 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_2/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_2/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_2/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_3/0/
--rw-rw-rw-   0 root         (0) root         (0)     4045 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_3/0/__fastr_prov__.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_3/0/result.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_3/0/result_json.prov.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/
--rw-rw-rw-   0 root         (0) root         (0)    21826 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/id_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_1/0/
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_1/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_2/0/
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_2/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_3/0/
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_3/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/
--rw-rw-rw-   0 root         (0) root         (0)     4676 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_0/1/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_0/1/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_0/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_0/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_0/1/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_0/1/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_1/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_1/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_1/1/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_1/1/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_2/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_2/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_2/1/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_2/1/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_3/0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_3/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_3/1/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/sink/id_1_3/1/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1419 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/__fastr_network__.json
--rw-rw-rw-   0 root         (0) root         (0)      140 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/__source_data__.pickle.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/1/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/1/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/2/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/2/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/3/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/3/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/1/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/1/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/2/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/2/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/3/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/3/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/0/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/1/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/1/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/2/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/2/result.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/3/
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/3/result.json
--rwxrwxrwx   0 root         (0) root         (0)     2740 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/elastix_nipype.py
--rw-rw-rw-   0 root         (0) root         (0)     1895 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/envvar.py
--rw-rw-rw-   0 root         (0) root         (0)     1699 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/expand.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/failing_macro.py
--rw-rw-rw-   0 root         (0) root         (0)     1937 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/failing_missing_macro.py
--rw-rw-rw-   0 root         (0) root         (0)     3828 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/failing_network.py
--rw-rw-rw-   0 root         (0) root         (0)     3810 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/failing_network_missing.py
--rw-rw-rw-   0 root         (0) root         (0)     1858 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/filecopy.py
--rwxrwxrwx   0 root         (0) root         (0)     2024 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/input_groups.py
--rw-rw-rw-   0 root         (0) root         (0)     3799 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/macro_node.py
--rw-rw-rw-   0 root         (0) root         (0)     3470 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/macro_node2.py
--rwxrwxrwx   0 root         (0) root         (0)     2028 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/shift_links.py
--rw-rw-rw-   0 root         (0) root         (0)     1673 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/source_sink.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/examples/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1988 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/examples/test/test_examples.py
--rw-rw-rw-   0 root         (0) root         (0)    17029 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/execution/
--rw-rw-rw-   0 root         (0) root         (0)     1030 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/execution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1356 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/execution/basenoderun.py
--rwxrwxrwx   0 root         (0) root         (0)    12984 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/execution/environmentmodules.py
--rwxrwxrwx   0 root         (0) root         (0)     7458 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/execution/executionscript.py
--rw-rw-rw-   0 root         (0) root         (0)     9329 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/execution/flownoderun.py
--rw-rw-rw-   0 root         (0) root         (0)    56219 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/execution/inputoutputrun.py
--rw-rw-rw-   0 root         (0) root         (0)    53162 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/execution/job.py
--rw-rw-rw-   0 root         (0) root         (0)    32012 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/execution/linkrun.py
--rw-rw-rw-   0 root         (0) root         (0)     6918 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/execution/macronoderun.py
--rw-rw-rw-   0 root         (0) root         (0)     2350 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/execution/networkanalyzer.py
--rw-rw-rw-   0 root         (0) root         (0)    10878 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/execution/networkchunker.py
--rw-rw-rw-   0 root         (0) root         (0)    32056 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/execution/networkrun.py
--rw-rw-rw-   0 root         (0) root         (0)    30744 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/execution/noderun.py
--rw-rw-rw-   0 root         (0) root         (0)     9916 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/execution/sinknoderun.py
--rw-rw-rw-   0 root         (0) root         (0)    18268 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/execution/sourcenoderun.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/globals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/helpers/
--rw-rw-rw-   0 root         (0) root         (0)      892 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5709 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/checksum.py
--rw-rw-rw-   0 root         (0) root         (0)     1393 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/classproperty.py
--rwxrwxrwx   0 root         (0) root         (0)     1606 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/clear_pycs.py
--rwxrwxrwx   0 root         (0) root         (0)    22720 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/configmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     2357 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/events.py
--rw-rw-rw-   0 root         (0) root         (0)     5898 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/filesynchelper.py
--rw-rw-rw-   0 root         (0) root         (0)     4844 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/iohelpers.py
--rw-rw-rw-   0 root         (0) root         (0)    19151 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/jsonschemaparser.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/lazy_module.py
--rw-rw-rw-   0 root         (0) root         (0)     3616 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/lockfile.py
--rw-rw-rw-   0 root         (0) root         (0)     1252 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/procutils.py
--rw-rw-rw-   0 root         (0) root         (0)     3178 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/report.py
--rw-rw-rw-   0 root         (0) root         (0)     1794 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/rest_generation.py
--rw-rw-rw-   0 root         (0) root         (0)     5866 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/schematotable.py
--rw-rw-rw-   0 root         (0) root         (0)     1418 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/shellescape.py
--rw-rw-rw-   0 root         (0) root         (0)     7062 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/sysinfo.py
--rw-rw-rw-   0 root         (0) root         (0)     8605 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/helpers/xmltodict.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/planning/
--rw-rw-rw-   0 root         (0) root         (0)      695 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/planning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10985 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/planning/inputgroup.py
--rw-rw-rw-   0 root         (0) root         (0)    10978 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/planning/inputgroupcombiner.py
--rw-rw-rw-   0 root         (0) root         (0)    61448 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/planning/inputoutput.py
--rwxrwxrwx   0 root         (0) root         (0)    25029 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/planning/link.py
--rwxrwxrwx   0 root         (0) root         (0)    35119 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/planning/network.py
--rwxrwxrwx   0 root         (0) root         (0)    58252 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/planning/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/plugins/
--rw-rw-rw-   0 root         (0) root         (0)     1908 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    33212 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/plugins/executionplugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/plugins/managers/
--rw-rw-rw-   0 root         (0) root         (0)      695 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/plugins/managers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1627 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/plugins/managers/executionpluginmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/plugins/managers/interfacemanager.py
--rw-rw-rw-   0 root         (0) root         (0)    11941 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/plugins/managers/iopluginmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     1001 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/plugins/managers/networkmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     6407 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/plugins/managers/objectmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     5279 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/plugins/managers/pluginmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     1310 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/plugins/managers/targetmanager.py
--rwxrwxrwx   0 root         (0) root         (0)     1544 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/plugins/managers/toolmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     2423 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/plugins/reportingplugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/
--rw-rw-rw-   0 root         (0) root         (0)      852 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/datatypes/
--rw-rw-rw-   0 root         (0) root         (0)     2732 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/AnalyzeImageFile.py
--rw-rw-rw-   0 root         (0) root         (0)     3680 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/Boolean.py
--rwxrwxrwx   0 root         (0) root         (0)     2365 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/Directory.py
--rw-rw-rw-   0 root         (0) root         (0)     1329 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/FilePrefix.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/Float.py
--rw-rw-rw-   0 root         (0) root         (0)      992 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/ITKImageFile.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/Int.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/JsonFile.py
--rw-rw-rw-   0 root         (0) root         (0)     4202 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/MetaImageFile.py
--rw-rw-rw-   0 root         (0) root         (0)      894 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/NiftiImageFile.py
--rw-rw-rw-   0 root         (0) root         (0)     2679 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/NiftiImageFileCompressed.py
--rw-rw-rw-   0 root         (0) root         (0)     1932 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/NiftiImageFileUncompressed.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/NrrdImageFile.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/Number.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/ProvNFile.py
--rw-rw-rw-   0 root         (0) root         (0)     1176 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/String.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/TifImageFile.py
--rw-rw-rw-   0 root         (0) root         (0)      818 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/TxtFile.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/UnsignedInt.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/datatypes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/networks/
--rw-rw-rw-   0 root         (0) root         (0)     2150 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/networks/add_ints.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/plugins/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/plugins/collectorplugins/
--rw-rw-rw-   0 root         (0) root         (0)     3020 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/collectorplugins/jsoncollector.py
--rw-rw-rw-   0 root         (0) root         (0)     6227 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/collectorplugins/pathcollector.py
--rw-rw-rw-   0 root         (0) root         (0)     3608 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/collectorplugins/stdoutcollector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/plugins/executionplugins/
--rw-rw-rw-   0 root         (0) root         (0)     2836 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/executionplugins/blockingexecution.py
--rw-rw-rw-   0 root         (0) root         (0)    26375 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/executionplugins/drmaaexecution.py
--rw-rw-rw-   0 root         (0) root         (0)     3587 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/executionplugins/linearexecution.py
--rw-rw-rw-   0 root         (0) root         (0)     5189 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/executionplugins/processpoolexecution.py
--rw-rw-rw-   0 root         (0) root         (0)     4638 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/executionplugins/rqexecution.py
--rw-rw-rw-   0 root         (0) root         (0)    11704 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/executionplugins/slurmexecution.py
--rw-rw-rw-   0 root         (0) root         (0)     3179 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/executionplugins/strongrexecution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/plugins/flowplugins/
--rw-rw-rw-   0 root         (0) root         (0)     3643 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/flowplugins/crossvalidation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/plugins/interfaceplugins/
--rw-rw-rw-   0 root         (0) root         (0)    46619 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/interfaceplugins/fastrinterface.py
--rw-rw-rw-   0 root         (0) root         (0)     8436 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/interfaceplugins/flowinterface.py
--rw-rw-rw-   0 root         (0) root         (0)     9149 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/interfaceplugins/nipypeinterface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/plugins/ioplugins/
--rw-rw-rw-   0 root         (0) root         (0)     6829 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/ioplugins/commaseperatedvaluefile.py
--rw-rw-rw-   0 root         (0) root         (0)     5155 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/ioplugins/filesystem.py
--rw-rw-rw-   0 root         (0) root         (0)     1845 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/ioplugins/httpplugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1879 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/ioplugins/networkscope.py
--rw-rw-rw-   0 root         (0) root         (0)     1707 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/ioplugins/null.py
--rw-rw-rw-   0 root         (0) root         (0)     3329 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/ioplugins/reference.py
--rw-rw-rw-   0 root         (0) root         (0)     7721 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/ioplugins/s3filesystem.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/plugins/ioplugins/test/
--rw-rw-rw-   0 root         (0) root         (0)     5803 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/ioplugins/test/test_virtualfilesystem.py
--rw-rw-rw-   0 root         (0) root         (0)     2861 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/ioplugins/virtualfilesystem.py
--rw-rw-rw-   0 root         (0) root         (0)     5222 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/ioplugins/virtualfilesystemregularexpression.py
--rw-rw-rw-   0 root         (0) root         (0)     2502 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/ioplugins/virtualfilesystemvaluelist.py
--rw-rw-rw-   0 root         (0) root         (0)    28502 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/ioplugins/xnatstorage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/plugins/reportingplugins/
--rw-rw-rw-   0 root         (0) root         (0)     4567 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/reportingplugins/elasticsearchreporter.py
--rw-rw-rw-   0 root         (0) root         (0)    21923 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/reportingplugins/pimreporter.py
--rw-rw-rw-   0 root         (0) root         (0)     2115 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/reportingplugins/simplereport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/plugins/targetplugins/
--rw-rw-rw-   0 root         (0) root         (0)     6192 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/targetplugins/dockertarget.py
--rw-rw-rw-   0 root         (0) root         (0)    11549 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/targetplugins/localbinarytarget.py
--rw-rw-rw-   0 root         (0) root         (0)     2596 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/targetplugins/macrotarget.py
--rw-rw-rw-   0 root         (0) root         (0)     3666 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/plugins/targetplugins/singularitytarget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/schemas/
--rw-rw-rw-   0 root         (0) root         (0)     1780 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/schemas/ConstantNode.schema.json
--rw-rw-rw-   0 root         (0) root         (0)    10601 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/schemas/FastrInterface.schema.json
--rw-rw-rw-   0 root         (0) root         (0)     1019 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/schemas/Link.schema.json
--rw-rw-rw-   0 root         (0) root         (0)     1656 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/schemas/Network.schema.json
--rw-rw-rw-   0 root         (0) root         (0)     1264 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/schemas/Node.schema.json
--rw-rw-rw-   0 root         (0) root         (0)     1381 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/schemas/SinkNode.schema.json
--rw-rw-rw-   0 root         (0) root         (0)     1320 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/schemas/SourceNode.schema.json
--rw-rw-rw-   0 root         (0) root         (0)     5059 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/schemas/Tool.schema.json
--rw-rw-rw-   0 root         (0) root         (0)     2707 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/schemas/common.schema.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/secret/
--rw-rw-rw-   0 root         (0) root         (0)      104 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/secret/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/tools/
--rw-rw-rw-   0 root         (0) root         (0)      699 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/tools/fastr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/tools/fastr/flow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/tools/fastr/flow/1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1409 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/flow/1.0/crossvalidation.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1342 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/add.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1818 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/addint.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/
--rw-rw-rw-   0 root         (0) root         (0)     1340 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/add.py
--rw-rw-rw-   0 root         (0) root         (0)     1355 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/addint.py
--rw-rw-rw-   0 root         (0) root         (0)     1386 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/divide.py
--rw-rw-rw-   0 root         (0) root         (0)     1419 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/intdivide.py
--rw-rw-rw-   0 root         (0) root         (0)      378 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/max.py
--rw-rw-rw-   0 root         (0) root         (0)      378 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/min.py
--rw-rw-rw-   0 root         (0) root         (0)     1347 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/multiply.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/subtract.py
--rw-rw-rw-   0 root         (0) root         (0)     1173 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/sum.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/divide.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1843 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/intdivide.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1302 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/max.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1303 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/min.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1816 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/multiply.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1804 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/subtract.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1469 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/sum.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/test/addint/
--rw-rw-rw-   0 root         (0) root         (0)      322 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/test/addint/__fastr_tool_ref__.json
--rw-rw-rw-   0 root         (0) root         (0)      608 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/test/addint/__fastr_tool_result.pickle.gz
--rw-rw-rw-   0 root         (0) root         (0)      336 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/test/addint/__output__fastr_tool_ref__.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/tools/fastr/test/
--rw-rw-rw-   0 root         (0) root         (0)     7012 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/test/bet_docker.yaml
--rw-rw-rw-   0 root         (0) root         (0)     7191 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/test/bet_singularity.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2390 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/auto_prefix.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2443 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/auto_prefix_negate.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      589 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/auto_prefix.py
--rw-rw-rw-   0 root         (0) root         (0)      602 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/auto_prefix_negate.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/delay.py
--rw-rw-rw-   0 root         (0) root         (0)      672 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/envvar.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/fail.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/passthroughauto.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/range.py
--rw-rw-rw-   0 root         (0) root         (0)     1037 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/stdout.py
--rw-rw-rw-   0 root         (0) root         (0)     1534 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/delay.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2171 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/envvar.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2881 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/fail_0.1.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2881 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/fail_0.2.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2058 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/passthroughauto.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1491 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/range.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1535 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/stdout.yaml
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/resources/tools/fastr/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/test/
--rw-rw-rw-   0 root         (0) root         (0)      696 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6096 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/test/test_datatypes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/utils/
--rw-rw-rw-   0 root         (0) root         (0)      784 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr/utils/cmd/
--rw-rw-rw-   0 root         (0) root         (0)     2981 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/cmd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2712 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/cmd/cat.py
--rw-rw-rw-   0 root         (0) root         (0)     1786 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/cmd/dump.py
--rw-rw-rw-   0 root         (0) root         (0)     1732 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/cmd/execute.py
--rw-rw-rw-   0 root         (0) root         (0)     6339 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/cmd/extract_argparse.py
--rw-rw-rw-   0 root         (0) root         (0)     3245 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/cmd/provenance.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/cmd/pylint.py
--rw-rw-rw-   0 root         (0) root         (0)     1977 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/cmd/report.py
--rw-rw-rw-   0 root         (0) root         (0)     2599 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/cmd/run.py
--rw-rw-rw-   0 root         (0) root         (0)     3913 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/cmd/sink.py
--rw-rw-rw-   0 root         (0) root         (0)     5417 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/cmd/source.py
--rw-rw-rw-   0 root         (0) root         (0)     6801 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/cmd/test.py
--rw-rw-rw-   0 root         (0) root         (0)     5869 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/cmd/trace.py
--rw-rw-rw-   0 root         (0) root         (0)    13343 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/cmd/upgrade.py
--rw-rw-rw-   0 root         (0) root         (0)     1987 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/cmd/verify.py
--rw-rw-rw-   0 root         (0) root         (0)     7304 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/compare.py
--rw-rw-rw-   0 root         (0) root         (0)     4752 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/dicteq.py
--rw-rw-rw-   0 root         (0) root         (0)     1541 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/gettools.py
--rw-rw-rw-   0 root         (0) root         (0)     1720 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/multiprocesswrapper.py
--rw-rw-rw-   0 root         (0) root         (0)    10062 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/utils/verify.py
--rw-rw-rw-   0 root         (0) root         (0)     3797 2022-10-13 07:48:29.000000 fastr-3.3.1/fastr/version.py
--rw-r--r--   0 root         (0) root         (0)       50 2022-10-13 07:48:42.000000 fastr-3.3.1/fastr/versioninfo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2025 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    39037 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      411 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-10-13 07:48:43.000000 fastr-3.3.1/fastr.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      410 2022-10-13 07:48:29.000000 fastr-3.3.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-10-13 07:48:43.000000 fastr-3.3.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     5049 2022-10-13 07:48:29.000000 fastr-3.3.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       46 2022-10-13 07:48:29.000000 fastr-3.3.1/test_requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-10-13 07:48:29.000000 fastr-3.3.1/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)    10174 2024-05-23 10:39:11.000000 fastr-3.4.0/APACHE-LICENSE-2.0
+-rw-rw-rw-   0 root         (0) root         (0)      684 2024-05-23 10:39:11.000000 fastr-3.4.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-23 10:39:11.000000 fastr-3.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2025 2024-05-23 10:39:24.000000 fastr-3.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      821 2024-05-23 10:39:11.000000 fastr-3.4.0/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/
+-rw-rw-rw-   0 root         (0) root         (0)     2632 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/abc/
+-rw-rw-rw-   0 root         (0) root         (0)    12110 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/abc/basemanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     6410 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/abc/baseplugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8792 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/abc/basepluginmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)    11370 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/abc/serializable.py
+-rw-rw-rw-   0 root         (0) root         (0)    10372 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/abc/updateable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/api/
+-rw-rw-rw-   0 root         (0) root         (0)    27859 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/core/
+-rw-rw-rw-   0 root         (0) root         (0)      891 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20756 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/cardinality.py
+-rw-rw-rw-   0 root         (0) root         (0)     5826 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/dimension.py
+-rw-rw-rw-   0 root         (0) root         (0)     6732 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/interface.py
+-rw-rw-rw-   0 root         (0) root         (0)    14694 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/ioplugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     7751 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/provenance.py
+-rw-rw-rw-   0 root         (0) root         (0)     6075 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/resourcelimit.py
+-rw-rw-rw-   0 root         (0) root         (0)    39605 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    10351 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/core/test/
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/test/test_datatypemanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5357 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/test/test_dimension.py
+-rw-rw-rw-   0 root         (0) root         (0)    13348 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/test/test_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)     3230 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/test/test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     4587 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/test/test_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4292 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/test/test_vfs.py
+-rwxrwxrwx   0 root         (0) root         (0)    36397 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/tool.py
+-rwxrwxrwx   0 root         (0) root         (0)     7152 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/version.py
+-rw-rw-rw-   0 root         (0) root         (0)    12813 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/core/vfs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/data/
+-rw-rw-rw-   0 root         (0) root         (0)      743 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6389 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/data/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/datatypes/
+-rw-rw-rw-   0 root         (0) root         (0)    45610 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/datatypes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     1769 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/__generate_reference__.py
+-rw-rw-rw-   0 root         (0) root         (0)      699 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2261 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/add_ints.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/add_ints_missing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2021 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/add_ints_s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     2995 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/advanced_linking.py
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/auto_prefix.py
+-rw-rw-rw-   0 root         (0) root         (0)     2851 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/chunk_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/collapse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1730 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/collapse_expand.py
+-rw-rw-rw-   0 root         (0) root         (0)     2524 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/cross_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/add_ints/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/add_ints/value
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/add_ints/values
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/add_ints/values_duplicate
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/hello.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/images/
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/images/mrwhite.mhd
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/images/mrwhite.raw
+-rw-rw-rw-   0 root         (0) root         (0)      289 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/images/mrwhite_duplicate.mhd
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/images/mrwhite_duplicate.raw
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/id_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/id_1_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/id_1_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/id_1_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/id_1_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/id_1_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/id_1_1/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/id_1_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/id_1_2/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/id_1_2/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/id_1_3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/id_1_3/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/sink/id_1_3/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     9335 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)     3716 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/1/
+-rw-rw-rw-   0 root         (0) root         (0)     3716 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/1/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/1/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/1/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/1/
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/1/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/1/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/1/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/1/
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/1/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/1/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/1/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/1/
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/1/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/1/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/1/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/1/
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/1/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/1/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/1/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)     5228 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/1/
+-rw-rw-rw-   0 root         (0) root         (0)     5228 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/1/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/1/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/1/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/2/
+-rw-rw-rw-   0 root         (0) root         (0)     5228 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/2/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/2/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/2/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/3/
+-rw-rw-rw-   0 root         (0) root         (0)     5228 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/3/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/3/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/3/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/4/
+-rw-rw-rw-   0 root         (0) root         (0)     5228 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/4/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/4/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/4/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/5/
+-rw-rw-rw-   0 root         (0) root         (0)     5228 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/5/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/5/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/5/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/6/
+-rw-rw-rw-   0 root         (0) root         (0)     5228 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/6/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/6/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/6/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/1/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/1/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/1/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/1/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/2/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/2/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/2/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/2/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/3/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/3/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/3/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/3/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/4/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/4/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/4/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/4/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/5/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/5/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/5/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/5/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/6/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/6/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/6/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/6/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/1/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/1/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/1/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/1/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/2/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/2/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/2/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/2/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/3/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/3/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/3/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/3/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/4/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/4/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/4/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/4/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/5/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/5/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/5/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/5/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/6/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/6/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/6/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/6/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/0/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/1/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/1/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/1/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/1/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/2/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/2/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/2/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/2/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/3/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/3/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/3/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/3/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/4/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/4/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/4/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/4/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/5/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/5/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/5/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/5/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/6/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/6/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/6/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/6/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/0/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/1/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/1/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/1/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/1/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/2/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/2/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/2/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/2/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/3/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/3/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/3/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/3/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/4/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/4/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/4/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/4/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/5/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/5/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/5/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/5/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/6/
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/6/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/6/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/6/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     9793 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4238 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_0/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_0/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_0/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4238 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_1/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_1/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_1/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_2/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4238 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_2/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_2/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_2/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_0/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_0/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_0/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_1/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_1/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_1/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_2/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_2/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_2/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_2/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4238 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_0/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_0/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_0/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4238 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_1/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_1/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_1/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_2/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4238 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_2/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_2/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_2/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_0/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_0/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_0/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_1/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_1/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_1/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_2/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_2/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_2/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_2/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7258 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)     3843 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_0/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_0/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_0/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)     3843 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_1/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_1/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_1/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_2/0/
+-rw-rw-rw-   0 root         (0) root         (0)     3843 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_2/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_2/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_2/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_3/0/
+-rw-rw-rw-   0 root         (0) root         (0)     3843 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_3/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_3/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_3/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_0/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_0/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_0/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_1/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_1/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_1/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_2/0/
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_2/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_2/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_2/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_3/0/
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_3/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_3/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_3/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/1/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/1/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/10/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/10/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/11/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/11/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/2/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/2/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/3/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/3/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/4/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/4/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/5/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/5/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/6/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/6/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/7/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/7/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/8/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/8/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/9/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/sink/all/9/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__0/1/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__0/1/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__0/2/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__0/2/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__1/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__1/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__1/1/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__1/1/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__1/2/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__1/2/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__2/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__2/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__2/1/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__2/1/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__2/2/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__2/2/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__3/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__3/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__3/1/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__3/1/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__3/2/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/sink/all__3/2/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7261 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)       91 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/id_0__fold_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/id_0__fold_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/id_0__fold_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/id_1__fold_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/id_1__fold_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/id_1__fold_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/id_2__fold_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/id_2__fold_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/id_2__fold_1/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/id_3__fold_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/id_3__fold_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/id_3__fold_1/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/id_4__fold_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/id_4__fold_2/0/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/sink/id_4__fold_2/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_a__0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_a__0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_a__0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_a__1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_a__1/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_a__1/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_a__2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_a__2/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_a__2/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_a__3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_a__3/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_a__3/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_b__0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_b__0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_b__0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_b__1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_b__1/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_b__1/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_b__2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_b__2/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_b__2/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_b__3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_b__3/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_b__3/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_c__0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_c__0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_c__0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_c__1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_c__1/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_c__1/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_c__2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_c__2/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_c__2/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_c__3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_c__3/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/expand_0.0/sink/sample_c__3/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_macro_top_level_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)    23146 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_macro_top_level_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)      148 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_macro_top_level_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_macro_top_level_0.0/sink/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_macro_top_level_0.0/sink/sample_1_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_macro_top_level_0.0/sink/sample_1_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)     3854 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_macro_top_level_0.0/sink/sample_1_0/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_macro_top_level_0.0/sink/sample_1_0/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_macro_top_level_0.0/sink/sample_1_0/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)    14172 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_1/sample_1_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_1/sample_1_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_1/sample_1_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_1/sample_1_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_1/sample_1_2/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_1/sample_1_2/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_2/sample_1_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_2/sample_1_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_2/sample_1_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_2/sample_1_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_2/sample_1_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_2/sample_1_1/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_3/sample_1_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_3/sample_1_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_3/sample_1_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/1/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/1/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/2/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/2/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/3/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/3/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/4/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/4/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/5/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/5/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/6/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/6/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/7/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/7/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/8/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_4/sample_1_0/8/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_5/sample_1_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_5/sample_1_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/sink_5/sample_1_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/file_copy_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2439 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/file_copy_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/file_copy_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/file_copy_0.0/sink/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/file_copy_0.0/sink/id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/file_copy_0.0/sink/id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/file_copy_0.0/sink/id_0/0/hello.txt
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/file_copy_0.0/sink/id_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     3512 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_0__id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_0__id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_0__id_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_0__id_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_0__id_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_0__id_1/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_0__id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_0__id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_0__id_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_0__id_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_0__id_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_0__id_1/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_1__id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_1__id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_1__id_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_1__id_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_1__id_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_1__id_1/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_2__id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_2__id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_2__id_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_2__id_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_2__id_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_2__id_1/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_3__id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_3__id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_3__id_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_3__id_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_3__id_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/sink/id_1_3__id_1/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     9267 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_0/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_0/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_0/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_1/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_1/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_1/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_2/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_2/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_2/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_2/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_3/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_3/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_3/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_3/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_0/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_0/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_0/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_1/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_1/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_1/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_2/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_2/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_2/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_2/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_3/0/
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_3/0/__fastr_prov__.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_3/0/result.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_3/0/result_json.prov.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)    21826 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/id_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_1/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_2/0/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_2/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_3/0/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/sink/id_1_3/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     4676 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_0/1/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_0/1/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_0/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_0/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_0/1/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_0/1/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_1/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_1/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_1/1/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_1/1/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_2/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_2/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_2/1/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_2/1/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_3/0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_3/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_3/1/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/sink/id_1_3/1/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1419 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/__fastr_network__.json
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/__source_data__.pickle.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/1/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/1/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/2/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/2/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/3/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_a/3/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/1/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/1/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/2/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/2/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/3/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_b/3/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/0/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/1/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/1/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/2/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/2/result.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/3/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/sink/sample_c/3/result.json
+-rwxrwxrwx   0 root         (0) root         (0)     2740 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/elastix_nipype.py
+-rw-rw-rw-   0 root         (0) root         (0)     1895 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/envvar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/expand.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/failing_macro.py
+-rw-rw-rw-   0 root         (0) root         (0)     1937 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/failing_missing_macro.py
+-rw-rw-rw-   0 root         (0) root         (0)     3828 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/failing_network.py
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/failing_network_missing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/filecopy.py
+-rwxrwxrwx   0 root         (0) root         (0)     2024 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/input_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     3799 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/macro_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3470 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/macro_node2.py
+-rwxrwxrwx   0 root         (0) root         (0)     2028 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/shift_links.py
+-rw-rw-rw-   0 root         (0) root         (0)     1673 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/source_sink.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/examples/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/test/test_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/examples/via_file_argument.py
+-rw-rw-rw-   0 root         (0) root         (0)    17029 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/execution/
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/execution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/execution/basenoderun.py
+-rwxrwxrwx   0 root         (0) root         (0)    12984 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/execution/environmentmodules.py
+-rwxrwxrwx   0 root         (0) root         (0)     7769 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/execution/executionscript.py
+-rw-rw-rw-   0 root         (0) root         (0)     9329 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/execution/flownoderun.py
+-rw-rw-rw-   0 root         (0) root         (0)    56219 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/execution/inputoutputrun.py
+-rw-rw-rw-   0 root         (0) root         (0)    53572 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/execution/job.py
+-rw-rw-rw-   0 root         (0) root         (0)    32012 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/execution/linkrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     6918 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/execution/macronoderun.py
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/execution/networkanalyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)    10878 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/execution/networkchunker.py
+-rw-rw-rw-   0 root         (0) root         (0)    32056 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/execution/networkrun.py
+-rw-rw-rw-   0 root         (0) root         (0)    30744 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/execution/noderun.py
+-rw-rw-rw-   0 root         (0) root         (0)     9916 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/execution/sinknoderun.py
+-rw-rw-rw-   0 root         (0) root         (0)    18268 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/execution/sourcenoderun.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/globals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5709 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/checksum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/classproperty.py
+-rwxrwxrwx   0 root         (0) root         (0)     1606 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/clear_pycs.py
+-rwxrwxrwx   0 root         (0) root         (0)    22936 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/configmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2357 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     5898 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/filesynchelper.py
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/iohelpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    19151 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/jsonschemaparser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/lazy_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     3616 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/lockfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/procutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/rest_generation.py
+-rw-rw-rw-   0 root         (0) root         (0)     5866 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/schematotable.py
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/shellescape.py
+-rw-rw-rw-   0 root         (0) root         (0)     7062 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/sysinfo.py
+-rw-rw-rw-   0 root         (0) root         (0)     8605 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/helpers/xmltodict.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/planning/
+-rw-rw-rw-   0 root         (0) root         (0)      695 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/planning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10985 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/planning/inputgroup.py
+-rw-rw-rw-   0 root         (0) root         (0)    10978 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/planning/inputgroupcombiner.py
+-rw-rw-rw-   0 root         (0) root         (0)    61448 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/planning/inputoutput.py
+-rwxrwxrwx   0 root         (0) root         (0)    25029 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/planning/link.py
+-rwxrwxrwx   0 root         (0) root         (0)    35119 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/planning/network.py
+-rwxrwxrwx   0 root         (0) root         (0)    58252 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/planning/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    33212 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/plugins/executionplugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/plugins/managers/
+-rw-rw-rw-   0 root         (0) root         (0)      695 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/plugins/managers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1627 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/plugins/managers/executionpluginmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/plugins/managers/interfacemanager.py
+-rw-rw-rw-   0 root         (0) root         (0)    11941 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/plugins/managers/iopluginmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/plugins/managers/networkmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     6407 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/plugins/managers/objectmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5279 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/plugins/managers/pluginmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/plugins/managers/targetmanager.py
+-rwxrwxrwx   0 root         (0) root         (0)     1544 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/plugins/managers/toolmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2423 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/plugins/reportingplugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      852 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/datatypes/
+-rw-rw-rw-   0 root         (0) root         (0)     2732 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/AnalyzeImageFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3680 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/Boolean.py
+-rwxrwxrwx   0 root         (0) root         (0)     2365 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/Directory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/FilePrefix.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/Float.py
+-rw-rw-rw-   0 root         (0) root         (0)      992 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/ITKImageFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/Int.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/JsonFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/MetaImageFile.py
+-rw-rw-rw-   0 root         (0) root         (0)      894 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/NiftiImageFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     2679 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/NiftiImageFileCompressed.py
+-rw-rw-rw-   0 root         (0) root         (0)     1932 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/NiftiImageFileUncompressed.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/NrrdImageFile.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/Number.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/ProvNFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/String.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/TifImageFile.py
+-rw-rw-rw-   0 root         (0) root         (0)      818 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/TxtFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/UnsignedInt.py
+-rw-rw-rw-   0 root         (0) root         (0)      699 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/datatypes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/networks/
+-rw-rw-rw-   0 root         (0) root         (0)     2150 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/networks/add_ints.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/plugins/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/plugins/collectorplugins/
+-rw-rw-rw-   0 root         (0) root         (0)     3020 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/collectorplugins/jsoncollector.py
+-rw-rw-rw-   0 root         (0) root         (0)     6227 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/collectorplugins/pathcollector.py
+-rw-rw-rw-   0 root         (0) root         (0)     3608 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/collectorplugins/stdoutcollector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/plugins/executionplugins/
+-rw-rw-rw-   0 root         (0) root         (0)     2836 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/executionplugins/blockingexecution.py
+-rw-rw-rw-   0 root         (0) root         (0)    26375 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/executionplugins/drmaaexecution.py
+-rw-rw-rw-   0 root         (0) root         (0)     3587 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/executionplugins/linearexecution.py
+-rw-rw-rw-   0 root         (0) root         (0)     5229 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/executionplugins/processpoolexecution.py
+-rw-rw-rw-   0 root         (0) root         (0)     4638 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/executionplugins/rqexecution.py
+-rw-rw-rw-   0 root         (0) root         (0)    12397 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/executionplugins/slurmexecution.py
+-rw-rw-rw-   0 root         (0) root         (0)     3179 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/executionplugins/strongrexecution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/plugins/flowplugins/
+-rw-rw-rw-   0 root         (0) root         (0)     3643 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/flowplugins/crossvalidation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/plugins/interfaceplugins/
+-rw-rw-rw-   0 root         (0) root         (0)    48398 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/interfaceplugins/fastrinterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     8436 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/interfaceplugins/flowinterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     9149 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/interfaceplugins/nipypeinterface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/plugins/ioplugins/
+-rw-rw-rw-   0 root         (0) root         (0)     6829 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/ioplugins/commaseperatedvaluefile.py
+-rw-rw-rw-   0 root         (0) root         (0)     5155 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/ioplugins/filesystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1845 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/ioplugins/httpplugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1879 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/ioplugins/networkscope.py
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/ioplugins/null.py
+-rw-rw-rw-   0 root         (0) root         (0)     3329 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/ioplugins/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     7721 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/ioplugins/s3filesystem.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/plugins/ioplugins/test/
+-rw-rw-rw-   0 root         (0) root         (0)     5803 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/ioplugins/test/test_virtualfilesystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     2861 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/ioplugins/virtualfilesystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     5222 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/ioplugins/virtualfilesystemregularexpression.py
+-rw-rw-rw-   0 root         (0) root         (0)     2502 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/ioplugins/virtualfilesystemvaluelist.py
+-rw-rw-rw-   0 root         (0) root         (0)    28502 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/ioplugins/xnatstorage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/plugins/reportingplugins/
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/reportingplugins/elasticsearchreporter.py
+-rw-rw-rw-   0 root         (0) root         (0)    21923 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/reportingplugins/pimreporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/reportingplugins/simplereport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/plugins/targetplugins/
+-rw-rw-rw-   0 root         (0) root         (0)     6192 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/targetplugins/dockertarget.py
+-rw-rw-rw-   0 root         (0) root         (0)    11549 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/targetplugins/localbinarytarget.py
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/targetplugins/macrotarget.py
+-rw-rw-rw-   0 root         (0) root         (0)     4889 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/plugins/targetplugins/singularitytarget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/schemas/ConstantNode.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)    10601 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/schemas/FastrInterface.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/schemas/Link.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     1656 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/schemas/Network.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/schemas/Node.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/schemas/SinkNode.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     1320 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/schemas/SourceNode.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     5059 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/schemas/Tool.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     2707 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/schemas/common.schema.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/secret/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/secret/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      699 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/tools/fastr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/tools/fastr/flow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/tools/fastr/flow/1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/flow/1.0/crossvalidation.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1342 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/add.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1818 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/addint.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/add.py
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/addint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/divide.py
+-rw-rw-rw-   0 root         (0) root         (0)     1419 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/intdivide.py
+-rw-rw-rw-   0 root         (0) root         (0)      378 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/max.py
+-rw-rw-rw-   0 root         (0) root         (0)      378 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/min.py
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/multiply.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/subtract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1173 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/sum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/sum_via_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/divide.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/intdivide.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/max.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/min.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/multiply.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/subtract.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/sum.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/sum_via_file.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/test/addint/
+-rw-rw-rw-   0 root         (0) root         (0)      322 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/test/addint/__fastr_tool_ref__.json
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/test/addint/__fastr_tool_result.pickle.gz
+-rw-rw-rw-   0 root         (0) root         (0)      336 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/test/addint/__output__fastr_tool_ref__.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/tools/fastr/test/
+-rw-rw-rw-   0 root         (0) root         (0)     7012 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/test/bet_docker.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     7191 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/test/bet_singularity.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2390 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/auto_prefix.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2443 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/auto_prefix_negate.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      589 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/auto_prefix.py
+-rw-rw-rw-   0 root         (0) root         (0)      602 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/auto_prefix_negate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/delay.py
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/envvar.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/fail.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/passthroughauto.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/range.py
+-rw-rw-rw-   0 root         (0) root         (0)     1037 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/stdout.py
+-rw-rw-rw-   0 root         (0) root         (0)     1534 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/delay.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/envvar.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2881 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/fail_0.1.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2881 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/fail_0.2.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2058 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/passthroughauto.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/range.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/stdout.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/resources/tools/fastr/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/test/
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6096 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/test/test_datatypes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      784 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr/utils/cmd/
+-rw-rw-rw-   0 root         (0) root         (0)     2981 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/cmd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2712 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/cmd/cat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1786 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/cmd/dump.py
+-rw-rw-rw-   0 root         (0) root         (0)     1732 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/cmd/execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     6339 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/cmd/extract_argparse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3245 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/cmd/provenance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/cmd/pylint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1977 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/cmd/report.py
+-rw-rw-rw-   0 root         (0) root         (0)     2599 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/cmd/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     3913 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/cmd/sink.py
+-rw-rw-rw-   0 root         (0) root         (0)     5417 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/cmd/source.py
+-rw-rw-rw-   0 root         (0) root         (0)     6801 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/cmd/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5869 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/cmd/trace.py
+-rw-rw-rw-   0 root         (0) root         (0)    13413 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/cmd/upgrade.py
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/cmd/verify.py
+-rw-rw-rw-   0 root         (0) root         (0)     7304 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/compare.py
+-rw-rw-rw-   0 root         (0) root         (0)     4752 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/dicteq.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/gettools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/multiprocesswrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)    10062 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/utils/verify.py
+-rw-rw-rw-   0 root         (0) root         (0)     3797 2024-05-23 10:39:11.000000 fastr-3.4.0/fastr/version.py
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-23 10:39:23.000000 fastr-3.4.0/fastr/versioninfo
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2025 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    38614 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      257 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-23 10:39:24.000000 fastr-3.4.0/fastr.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-05-23 10:39:11.000000 fastr-3.4.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      145 2024-05-23 10:39:24.000000 fastr-3.4.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     5049 2024-05-23 10:39:11.000000 fastr-3.4.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-23 10:39:11.000000 fastr-3.4.0/test_requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-23 10:39:11.000000 fastr-3.4.0/version
```

### Comparing `fastr-3.3.1/APACHE-LICENSE-2.0` & `fastr-3.4.0/APACHE-LICENSE-2.0`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/LICENSE` & `fastr-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/MANIFEST.in` & `fastr-3.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/PKG-INFO` & `fastr-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastr
-Version: 3.3.1
+Version: 3.4.0
 Summary: Workflow creation and batch execution environment.
 Home-page: https://gitlab.com/radiology/infrastructure/fastr
 Author: H.C. Achterberg, M. Koek
 Author-email: hakim.achterberg@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `fastr-3.3.1/README` & `fastr-3.4.0/README`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/__init__.py` & `fastr-3.4.0/fastr/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/abc/basemanager.py` & `fastr-3.4.0/fastr/abc/basemanager.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/abc/baseplugin.py` & `fastr-3.4.0/fastr/abc/baseplugin.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/abc/basepluginmanager.py` & `fastr-3.4.0/fastr/abc/basepluginmanager.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/abc/serializable.py` & `fastr-3.4.0/fastr/abc/serializable.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/abc/updateable.py` & `fastr-3.4.0/fastr/abc/updateable.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/api/__init__.py` & `fastr-3.4.0/fastr/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/__init__.py` & `fastr-3.4.0/fastr/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/cardinality.py` & `fastr-3.4.0/fastr/core/cardinality.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/dimension.py` & `fastr-3.4.0/fastr/core/dimension.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/interface.py` & `fastr-3.4.0/fastr/core/interface.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/ioplugin.py` & `fastr-3.4.0/fastr/core/ioplugin.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/provenance.py` & `fastr-3.4.0/fastr/core/provenance.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import os
+from pathlib import Path
+from typing import Union
 import urllib.parse
 
 import prov
 from prov.model import ProvDocument
 
 import fastr
 from .. import exceptions
@@ -185,7 +187,13 @@
     def serialize(self, filename, format):
         with open(filename, 'w') as fh_out:
             self.document.serialize(destination=fh_out, format=format)
 
             # Make sure the data gets flushed
             fh_out.flush()
             os.fsync(fh_out.fileno())
+
+    @staticmethod
+    def load(filepath: Union[str, Path]) -> 'Provenance':
+        provenance_data = Provenance()
+        provenance_data.document = prov.read(filepath)
+        return provenance_data
```

### Comparing `fastr-3.3.1/fastr/core/resourcelimit.py` & `fastr-3.4.0/fastr/core/resourcelimit.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/samples.py` & `fastr-3.4.0/fastr/core/samples.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/target.py` & `fastr-3.4.0/fastr/core/target.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/test/__init__.py` & `fastr-3.4.0/fastr/core/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/test/test_datatypemanager.py` & `fastr-3.4.0/fastr/core/test/test_datatypemanager.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/test/test_dimension.py` & `fastr-3.4.0/fastr/core/test/test_dimension.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/test/test_samples.py` & `fastr-3.4.0/fastr/core/test/test_samples.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/test/test_tool.py` & `fastr-3.4.0/fastr/core/test/test_tool.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/test/test_version.py` & `fastr-3.4.0/fastr/core/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/test/test_vfs.py` & `fastr-3.4.0/fastr/core/test/test_vfs.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/tool.py` & `fastr-3.4.0/fastr/core/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,14 +260,19 @@
                 if match['arch'] == arch:
                     match['score'] += 1
 
             matching_targets = sorted(matching_targets, reverse=True, key=lambda x: x['score'])
             log.debug('Sorted matches: {}'.format(matching_targets))
             target = matching_targets[0]
 
+        if len(matching_targets) > 1 and config.preferred_target != '':
+            targets = [x for x in matching_targets if x.get('class', None) == config.preferred_target]
+            if targets:
+                target = targets[0]
+
         # Make sure target is a copy
         target = dict(target)
         cls = self.DEFAULT_TARGET_CLASS.get(self.node_class)
         if cls is None:
             cls = target.pop('class', 'LocalBinaryTarget')
         cls = resources.targets[cls]
 
@@ -278,14 +283,15 @@
         # Check if the argument binary exists (or use bin as alternative)
         if 'binary' not in target and 'bin' in target:
             target['binary'] = target.pop('bin')
 
         # Remove needless fields
         target.pop('os', None)
         target.pop('arch', None)
+        target.pop('score', None)
 
         # Instantiate target
         try:
             self._target = cls(**target)
         except Exception as exception:
             log.error('Could not load tool {} because the following exception was encountered: {}'.format(
                 self.ns_id, exception
```

### Comparing `fastr-3.3.1/fastr/core/version.py` & `fastr-3.4.0/fastr/core/version.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/core/vfs.py` & `fastr-3.4.0/fastr/core/vfs.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/data/__init__.py` & `fastr-3.4.0/fastr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/data/url.py` & `fastr-3.4.0/fastr/data/url.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/datatypes/__init__.py` & `fastr-3.4.0/fastr/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/doc/doc_clean.py` & `fastr-3.4.0/fastr/helpers/clear_pycs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,53 @@
 #!/usr/bin/env python
 
 # Copyright 2011-2014 Biomedical Imaging Group Rotterdam, Departments of
 # Medical Informatics and Radiology, Erasmus MC, Rotterdam, The Netherlands
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pathlib
+"""
+A small tool to wipe all .pyc files from fastr
+"""
+import os
 
 
-def clean():
+def dir_list(directory):
     """
-    Clean the _autogen and main directories of .rst and .txt files
-    """
-    doc_path = pathlib.Path(__file__).parent
-    clean_dir(doc_path)
+    Find all .pyc files
 
-    autogen_path = doc_path / '_autogen'
-    clean_dir(autogen_path)
+    :param str directory: directory to search
+    :return: all .pyc files
+    :rtype: list
+    """
+    output_list = []
+    for root, _, files in os.walk(directory):
+        for filename in files:
+            if filename.endswith('.pyc'):
+                output_list.append(os.path.abspath(os.path.join(root, filename)))
+    return output_list
 
 
-def clean_dir(directory):
-    for filepath in directory.iterdir():
-        if filepath.suffix in ('.rst', '.txt'):
-            filepath.unlink()
-            print(f'removed {filepath}')
+def main():
+    """
+    Main entry poitn
+    """
+    os.chdir(os.path.join(os.path.dirname(os.path.abspath(__file__)), '..'))
+    print("************* REMOVING .pyc FILES ***********************")
+    for filename in dir_list('.'):
+        os.remove(filename)
+        print('removed {}'.format(filename))
+    print("************* ALL .pyc FILES REMOVED ********************")
 
 
 if __name__ == '__main__':
-    clean()
+    main()
```

### Comparing `fastr-3.3.1/fastr/examples/__generate_reference__.py` & `fastr-3.4.0/fastr/examples/__generate_reference__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/__init__.py` & `fastr-3.4.0/fastr/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/add_ints.py` & `fastr-3.4.0/fastr/examples/add_ints.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/add_ints_missing.py` & `fastr-3.4.0/fastr/examples/add_ints_missing.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/add_ints_s3.py` & `fastr-3.4.0/fastr/examples/add_ints_s3.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/advanced_linking.py` & `fastr-3.4.0/fastr/examples/advanced_linking.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/auto_prefix.py` & `fastr-3.4.0/fastr/examples/auto_prefix.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/chunk_test.py` & `fastr-3.4.0/fastr/examples/chunk_test.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/collapse.py` & `fastr-3.4.0/fastr/examples/collapse.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/collapse_expand.py` & `fastr-3.4.0/fastr/examples/collapse_expand.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/cross_validation.py` & `fastr-3.4.0/fastr/examples/cross_validation.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/add_ints_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/add_ints_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/1/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_0/1/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/1/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_0/1/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/1/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_1/1/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/1/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_2/1/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/1/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink1/id_1_3/1/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/1/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/1/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/2/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/2/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/3/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/3/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/4/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/4/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/5/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/5/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/6/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_0/6/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/1/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/1/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/2/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/2/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/3/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/3/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/4/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/4/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/5/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/5/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/6/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_0/6/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/1/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/1/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/2/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/2/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/3/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/3/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/4/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/4/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/5/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/5/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/6/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_1/6/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/1/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/1/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/2/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/2/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/3/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/3/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/4/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/4/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/5/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/5/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/6/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_2/6/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/1/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/1/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/2/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/2/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/3/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/3/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/4/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/4/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/5/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/5/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/6/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/advanced_linking_0.0/sink2/id_1_3/6/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_0/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_0/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_1/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_1/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_2/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_n/id_2/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_0/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_0/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_1/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_1/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_2/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_a_p/id_2/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_0/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_0/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_1/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_1/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_2/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_n/id_2/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_0/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_0/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_1/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_1/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_2/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/auto_prefix_test_0.0/sink_m_p/id_2/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_0/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_0/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_1/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_1/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_2/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_2/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_3/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_1/sample_1_3/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_0/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_0/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_1/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_1/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_2/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_2/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_3/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/chunk_test_0.0/sink_2/sample_1_3/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/collapse_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/collapse_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/collapse_expand_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/collapse_expand_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/cross_validation_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/cross_validation_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/expand_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/expand_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/failing_macro_top_level_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/failing_macro_top_level_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/failing_macro_top_level_0.0/sink/sample_1_0/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/failing_macro_top_level_0.0/sink/sample_1_0/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/failing_network_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/failing_network_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/file_copy_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/file_copy_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/input_groups_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/input_groups_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_0/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_0/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_1/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_1/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_2/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_2/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_3/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_0__id_3/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_0/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_0/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_1/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_1/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_2/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_2/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_3/0/__fastr_prov__.json` & `fastr-3.4.0/fastr/examples/data/reference/macro_node_2_0.0/sink/id_1__id_3/0/__fastr_prov__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/macro_top_level_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/macro_top_level_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/shift_links_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/shift_links_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/data/reference/source_sink_0.0/__fastr_network__.json` & `fastr-3.4.0/fastr/examples/data/reference/source_sink_0.0/__fastr_network__.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/elastix_nipype.py` & `fastr-3.4.0/fastr/examples/elastix_nipype.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/envvar.py` & `fastr-3.4.0/fastr/examples/envvar.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/expand.py` & `fastr-3.4.0/fastr/examples/expand.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/failing_macro.py` & `fastr-3.4.0/fastr/examples/failing_macro.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/failing_missing_macro.py` & `fastr-3.4.0/fastr/examples/failing_missing_macro.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/failing_network.py` & `fastr-3.4.0/fastr/examples/failing_network.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/failing_network_missing.py` & `fastr-3.4.0/fastr/examples/failing_network_missing.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/filecopy.py` & `fastr-3.4.0/fastr/examples/filecopy.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/input_groups.py` & `fastr-3.4.0/fastr/examples/input_groups.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/macro_node.py` & `fastr-3.4.0/fastr/examples/macro_node.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/macro_node2.py` & `fastr-3.4.0/fastr/examples/macro_node2.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/shift_links.py` & `fastr-3.4.0/fastr/examples/shift_links.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/source_sink.py` & `fastr-3.4.0/fastr/examples/source_sink.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/examples/test/test_examples.py` & `fastr-3.4.0/fastr/examples/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/exceptions.py` & `fastr-3.4.0/fastr/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/execution/__init__.py` & `fastr-3.4.0/fastr/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/execution/basenoderun.py` & `fastr-3.4.0/fastr/execution/basenoderun.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/execution/environmentmodules.py` & `fastr-3.4.0/fastr/execution/environmentmodules.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/execution/executionscript.py` & `fastr-3.4.0/fastr/execution/executionscript.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,49 +59,57 @@
 
     logfile_path = job.logfile
     fastr.log.info('Job log path: {}'.format(logfile_path))
 
     fastr.log.info('Running job {}\n  command: {} v{}\n  arguments: {}\n  outputs: {}\n'.format(
         job.id, job.tool_id, job.tool_version, job.input_arguments, job.output_arguments)
     )
+
+    # Checking for old results of a job run before continuing
     try:
-        # Checking for old results of a job run before continuing
         old_job_result = job.get_result()
 
         if old_job_result is not None:
-            fastr.log.info('Found a valid job results, re-using that as output')
-            job = old_job_result
+            fastr.log.info('Found a valid job results, re-using that, abort execution...')
+
+            # Write the update results, note this is needed because of the new run_id and global_node_id
+            old_job_result.write(write_prov=False, write_extra_info=False)
+            return
 
-        else:
-            fastr.log.info('No old result, executing job')
-            job.status = JobState.running
+    except Exception as exception:
+        fastr.log.error(f'Encountered an error when trying to get old result: {exception}, continuing with execution')
+
+    # No result found: start the actual job execution
+    try:
+        fastr.log.info('No old result found, executing job...')
+        job.status = JobState.running
 
-            # Initialize provenance
-            job.provenance.init_provenance(job)
+        # Initialize provenance
+        job.provenance.init_provenance(job)
 
-            job.info_store['hostinfo'] = get_hostinfo()
-            job.info_store['sysinfo_start'] = get_sysinfo()
+        job.info_store['hostinfo'] = get_hostinfo()
+        job.info_store['sysinfo_start'] = get_sysinfo()
 
-            fastr.log.info('DRMAA info: {}'.format(job.info_store['hostinfo']['drmaa']))
+        fastr.log.info('DRMAA info: {}'.format(job.info_store['hostinfo']['drmaa']))
 
-            fastr.log.info('Writing intermediate job info to: {}'.format(logfile_path))
-            job.write()
+        fastr.log.info('Writing intermediate job info to: {}'.format(logfile_path))
+        job.write()
 
-            job.execute()
+        job.execute()
 
-            # Document system information after
-            fastr.log.info('Job subprocess finished')
-            job.info_store['sysinfo_end'] = get_sysinfo()
+        # Document system information after
+        fastr.log.info('Job subprocess finished')
+        job.info_store['sysinfo_end'] = get_sysinfo()
 
-            fastr.log.info('Start hashing results')
-            start = datetime.datetime.now()
-            job.hash_results()
-            end = datetime.datetime.now()
-            fastr.log.info('Finished hashing results in {} seconds'.format((end - start).total_seconds()))
-            fastr.log.info('try end time: {}'.format(datetime.datetime.now()))
+        fastr.log.info('Start hashing results')
+        start = datetime.datetime.now()
+        job.hash_results()
+        end = datetime.datetime.now()
+        fastr.log.info('Finished hashing results in {} seconds'.format((end - start).total_seconds()))
+        fastr.log.info('try end time: {}'.format(datetime.datetime.now()))
     except BaseException as exception:
         fastr.log.warning('Caught exception in execution: [{}] {}'.format(type(exception).__name__,
                                                                           exception))
         job.status = JobState.execution_failed
         traceback.print_exc()
 
         # Log errors to the info store
```

### Comparing `fastr-3.3.1/fastr/execution/flownoderun.py` & `fastr-3.4.0/fastr/execution/flownoderun.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/execution/inputoutputrun.py` & `fastr-3.4.0/fastr/execution/inputoutputrun.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/execution/job.py` & `fastr-3.4.0/fastr/execution/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,20 +375,26 @@
         self.__dict__.update(state)
 
         # Cannot transport reference to Node
         if not hasattr(self, 'node'):
             self.node = None
 
         if not hasattr(self, 'info_store'):
-            self.info_store = {
-                'id': self.id,
-            }
+            if self.extrainfofile.is_file():
+                self.info_store = load_json(self.extrainfofile)
+            else:
+                self.info_store = {
+                    'id': self.id,
+                }
 
         if not hasattr(self, 'provenance'):
-            self.provenance = Provenance()
+            if self.provfile.is_file():
+                self.provenance = Provenance.load(self.provfile)
+            else:
+                self.provenance = Provenance()
 
     def get_result(self):
         """
         Get the result of the job if it is available. Load the output file if
         found and check if the job matches the current object. If so, load and
         return the result.
 
@@ -1120,17 +1126,21 @@
                         log.warning('Non-required output {} is invalid!'.format(id_))
 
             else:
                 raise exceptions.FastrTypeError('Output data is not of correct type (expected a list/dict)')
 
         return valid
 
-    def write(self):
-        self.provenance.serialize(self.provfile, 'json')
-        save_json(self.extrainfofile, self.info_store)
+    def write(self,
+              write_prov: bool = True,
+              write_extra_info: bool = True):
+        if write_prov:
+            self.provenance.serialize(self.provfile, 'json')
+        if write_extra_info:
+            save_json(self.extrainfofile, self.info_store)
         save(self, self.logfile)
 
     def _validate_result(self, output, output_value, payload):
         """
         Validate the result for a specific output/sample
         :param output: the output for which to check
         :param output_value: the value for the output
```

### Comparing `fastr-3.3.1/fastr/execution/linkrun.py` & `fastr-3.4.0/fastr/execution/linkrun.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/execution/macronoderun.py` & `fastr-3.4.0/fastr/execution/macronoderun.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/execution/networkanalyzer.py` & `fastr-3.4.0/fastr/execution/networkanalyzer.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/execution/networkchunker.py` & `fastr-3.4.0/fastr/execution/networkchunker.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/execution/networkrun.py` & `fastr-3.4.0/fastr/execution/networkrun.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/execution/noderun.py` & `fastr-3.4.0/fastr/execution/noderun.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/execution/sinknoderun.py` & `fastr-3.4.0/fastr/execution/sinknoderun.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/execution/sourcenoderun.py` & `fastr-3.4.0/fastr/execution/sourcenoderun.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/__init__.py` & `fastr-3.4.0/fastr/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/checksum.py` & `fastr-3.4.0/fastr/helpers/checksum.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/classproperty.py` & `fastr-3.4.0/fastr/helpers/classproperty.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/configmanager.py` & `fastr-3.4.0/fastr/helpers/configmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,15 +328,21 @@
             '',
             'Redis url e.g. redis://localhost:6379'
         ),
         "queue_report_interval": (
             int,
             0,
             "Interval in which to report the number of queued jobs (default is 0, no reporting)"
-        )
+        ),
+        "preferred_target": (
+            str,
+            '',
+            "Preferred Container Target: DockerTarget, SingularityTarget",
+            lambda x: x in ['DockerTarget', 'SingularityTarget'],
+        ),
     }
 
     # pylint: disable=too-many-instance-attributes
     # The config has many attributes, because its function is to hold
     # this data
 
     def __init__(self, *configfiles):
```

### Comparing `fastr-3.3.1/fastr/helpers/events.py` & `fastr-3.4.0/fastr/helpers/events.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/filesynchelper.py` & `fastr-3.4.0/fastr/helpers/filesynchelper.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/iohelpers.py` & `fastr-3.4.0/fastr/helpers/iohelpers.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/jsonschemaparser.py` & `fastr-3.4.0/fastr/helpers/jsonschemaparser.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/lazy_module.py` & `fastr-3.4.0/fastr/helpers/lazy_module.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/lockfile.py` & `fastr-3.4.0/fastr/helpers/lockfile.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/procutils.py` & `fastr-3.4.0/fastr/helpers/procutils.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/report.py` & `fastr-3.4.0/fastr/helpers/report.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/rest_generation.py` & `fastr-3.4.0/fastr/helpers/rest_generation.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/schematotable.py` & `fastr-3.4.0/fastr/helpers/schematotable.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/shellescape.py` & `fastr-3.4.0/fastr/helpers/shellescape.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/sysinfo.py` & `fastr-3.4.0/fastr/helpers/sysinfo.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/helpers/xmltodict.py` & `fastr-3.4.0/fastr/helpers/xmltodict.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/planning/__init__.py` & `fastr-3.4.0/fastr/planning/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/planning/inputgroup.py` & `fastr-3.4.0/fastr/planning/inputgroup.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/planning/inputgroupcombiner.py` & `fastr-3.4.0/fastr/planning/inputgroupcombiner.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/planning/inputoutput.py` & `fastr-3.4.0/fastr/planning/inputoutput.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/planning/link.py` & `fastr-3.4.0/fastr/planning/link.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/planning/network.py` & `fastr-3.4.0/fastr/planning/network.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/planning/node.py` & `fastr-3.4.0/fastr/planning/node.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/plugins/__init__.py` & `fastr-3.4.0/fastr/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/plugins/executionplugin.py` & `fastr-3.4.0/fastr/plugins/executionplugin.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/plugins/managers/__init__.py` & `fastr-3.4.0/fastr/plugins/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/plugins/managers/executionpluginmanager.py` & `fastr-3.4.0/fastr/plugins/managers/executionpluginmanager.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/plugins/managers/interfacemanager.py` & `fastr-3.4.0/fastr/plugins/managers/interfacemanager.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/plugins/managers/iopluginmanager.py` & `fastr-3.4.0/fastr/plugins/managers/iopluginmanager.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/plugins/managers/networkmanager.py` & `fastr-3.4.0/fastr/plugins/managers/networkmanager.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/plugins/managers/objectmanager.py` & `fastr-3.4.0/fastr/plugins/managers/objectmanager.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/plugins/managers/pluginmanager.py` & `fastr-3.4.0/fastr/plugins/managers/pluginmanager.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/plugins/managers/targetmanager.py` & `fastr-3.4.0/fastr/plugins/managers/targetmanager.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/plugins/managers/toolmanager.py` & `fastr-3.4.0/fastr/plugins/managers/toolmanager.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/plugins/reportingplugin.py` & `fastr-3.4.0/fastr/plugins/reportingplugin.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/__init__.py` & `fastr-3.4.0/fastr/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/AnalyzeImageFile.py` & `fastr-3.4.0/fastr/resources/datatypes/AnalyzeImageFile.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/Boolean.py` & `fastr-3.4.0/fastr/resources/datatypes/Boolean.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/Directory.py` & `fastr-3.4.0/fastr/resources/datatypes/Directory.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/FilePrefix.py` & `fastr-3.4.0/fastr/resources/datatypes/FilePrefix.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/Float.py` & `fastr-3.4.0/fastr/resources/datatypes/Float.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/ITKImageFile.py` & `fastr-3.4.0/fastr/resources/datatypes/ITKImageFile.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/Int.py` & `fastr-3.4.0/fastr/resources/datatypes/Int.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/JsonFile.py` & `fastr-3.4.0/fastr/resources/datatypes/JsonFile.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/MetaImageFile.py` & `fastr-3.4.0/fastr/resources/datatypes/MetaImageFile.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/NiftiImageFile.py` & `fastr-3.4.0/fastr/resources/datatypes/NiftiImageFile.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/NiftiImageFileCompressed.py` & `fastr-3.4.0/fastr/resources/datatypes/NiftiImageFileCompressed.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/NiftiImageFileUncompressed.py` & `fastr-3.4.0/fastr/resources/datatypes/NiftiImageFileUncompressed.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/NrrdImageFile.py` & `fastr-3.4.0/fastr/resources/datatypes/NrrdImageFile.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/Number.py` & `fastr-3.4.0/fastr/resources/datatypes/Number.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/ProvNFile.py` & `fastr-3.4.0/fastr/resources/datatypes/ProvNFile.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/String.py` & `fastr-3.4.0/fastr/resources/datatypes/String.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/TifImageFile.py` & `fastr-3.4.0/fastr/resources/datatypes/TifImageFile.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/TxtFile.py` & `fastr-3.4.0/fastr/resources/datatypes/TxtFile.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/UnsignedInt.py` & `fastr-3.4.0/fastr/resources/datatypes/UnsignedInt.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/datatypes/__init__.py` & `fastr-3.4.0/fastr/resources/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/networks/add_ints.json` & `fastr-3.4.0/fastr/resources/networks/add_ints.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/collectorplugins/jsoncollector.py` & `fastr-3.4.0/fastr/resources/plugins/collectorplugins/jsoncollector.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/collectorplugins/pathcollector.py` & `fastr-3.4.0/fastr/resources/plugins/collectorplugins/pathcollector.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/collectorplugins/stdoutcollector.py` & `fastr-3.4.0/fastr/resources/plugins/collectorplugins/stdoutcollector.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/executionplugins/blockingexecution.py` & `fastr-3.4.0/fastr/resources/plugins/executionplugins/blockingexecution.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/executionplugins/drmaaexecution.py` & `fastr-3.4.0/fastr/resources/plugins/executionplugins/drmaaexecution.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/executionplugins/linearexecution.py` & `fastr-3.4.0/fastr/resources/plugins/executionplugins/linearexecution.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/executionplugins/processpoolexecution.py` & `fastr-3.4.0/fastr/resources/plugins/executionplugins/processpoolexecution.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,16 @@
     def configuration_fields(cls):
         return {
             "process_pool_worker_number": (
                 int,
                 # Default number of workers is core - 1 (to assure system
                 # responsiveness)
                 max(multiprocessing.cpu_count() - 1, 1),
-                "Number of workers to use in a process pool"
+                "Number of workers to use in a process pool",
+                "$CPU_CORE_COUNTS - 1"
             )
         }
 
     def cleanup(self):
         # Close the multiprocess pool
         fastr.log.info('Stopping ProcessPool')
         self.pool.close()
```

### Comparing `fastr-3.3.1/fastr/resources/plugins/executionplugins/rqexecution.py` & `fastr-3.4.0/fastr/resources/plugins/executionplugins/rqexecution.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/executionplugins/slurmexecution.py` & `fastr-3.4.0/fastr/resources/plugins/executionplugins/slurmexecution.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 """#!/bin/bash
 #SBATCH --nodes=1
 #SBATCH --ntasks=1
 #SBATCH --cpus-per-task {cores}
 {memory}
 {time}
 {partition}
+{nodelist}
+{nodes_exclude}
 {gpus}
 #SBATCH --output {stdout}
 #SBATCH --error {stderr}
 {depends}
 {hold}
 
 {command}
@@ -94,14 +96,16 @@
 
     def __init__(self, finished_callback=None, cancelled_callback=None):
         super(SlurmExecution, self).__init__(finished_callback, cancelled_callback)
 
         # Config value
         self.check_interval = fastr.config.slurm_job_check_interval
         self.partition = fastr.config.slurm_partition
+        self.nodelist = fastr.config.slurm_nodelist
+        self.nodes_exclude = fastr.config.slurm_nodes_exclude
 
         # Create job translation table
         self.job_translation_table = dict()
         self.job_lookup_table = dict()
 
         # Start job status checker
         fastr.log.debug('Creating job status checker')
@@ -119,15 +123,17 @@
             self.job_checker.join()
 
     @classproperty
     def configuration_fields(cls):
         return {
             "slurm_job_check_interval": (int, 30, "The interval in which the job checker will start"
                                                   "to check for stale jobs"),
-            "slurm_partition": (str, '', "The slurm partition to use")
+            "slurm_partition": (str, '', "The slurm partition to use"),
+            "slurm_nodelist": (list, [], "List of slurm compute nodes to use"),
+            "slurm_nodes_exclude": (list, [], "List of slurm compute nodes to exclude")
         }
 
     @classmethod
     def test(cls):
         # Check if requirement commands can be called
         try:
             subprocess.check_output([cls.SBATCH, '--help'], stderr=subprocess.STDOUT)
@@ -188,27 +194,39 @@
             required_time = ''
 
         if self.partition:
             partition = '#SBATCH --partition {}'.format(self.partition)
         else:
             partition = ''
 
+        if self.nodelist:
+            nodelist = '#SBATCH --nodelist {}'.format(','.join(self.nodelist))
+        else:
+            nodelist = ''
+
+        if self.nodes_exclude:
+            nodes_exclude = '#SBATCH --exclude {}'.format(','.join(self.nodes_exclude))
+        else:
+            nodes_exclude = ''
+
         # Check if the job is ready to run or must be held
         if job.status == JobState.hold:
             hold = '--hold'
         else:
             hold = ''
 
         # Create SBATCH script from template
         sbatch_script = SBATCH_SCRIPT_TEMPLATE.format(
             cores=job.resources.cores or 1,
             memory=required_memory,
             gpus=required_gpus,
             time=required_time,
             partition=partition,
+            nodelist=nodelist,
+            nodes_exclude=nodes_exclude,
             stdout=job.stdoutfile,
             stderr=job.stderrfile,
             command=command,
             depends=depends,
             hold=hold,
         ).encode()
```

### Comparing `fastr-3.3.1/fastr/resources/plugins/executionplugins/strongrexecution.py` & `fastr-3.4.0/fastr/resources/plugins/executionplugins/strongrexecution.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/flowplugins/crossvalidation.py` & `fastr-3.4.0/fastr/resources/plugins/flowplugins/crossvalidation.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/interfaceplugins/fastrinterface.py` & `fastr-3.4.0/fastr/resources/plugins/interfaceplugins/fastrinterface.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 
 from abc import abstractmethod
 from collections import OrderedDict, namedtuple
 from collections.abc import Mapping, Iterable
 import json
 import os
+from pathlib import Path
 import sys
 import re
 
 import fastr
 from fastr import exceptions
 from fastr.abc.baseplugin import Plugin
 from fastr.abc.serializable import Serializable
@@ -286,14 +287,18 @@
     |               | ``nospace``                     | Flag indicating if there is no space between prefix and value (e.g. --in=val)  |
     |               +---------------------------------+--------------------------------------------------------------------------------+
     |               | ``format``                      | For DataTypes that have multiple representations, indicate which one to use    |
     |               +---------------------------------+--------------------------------------------------------------------------------+
     |               | ``default``                     | Default value for the Input                                                    |
     |               +---------------------------------+--------------------------------------------------------------------------------+
     |               | ``description``                 | Long description for an input                                                  |
+    |               +---------------------------------+--------------------------------------------------------------------------------+
+    |               | ``via_file``                    | Flag to indicate that this input should have its value written to a file and   |
+    |               |                                 | that the path to this file should be supplied as an argument instead. This is  |
+    |               |                                 | useful for arguments with an extremely high cardinality.                       |
     +---------------+---------------------------------+--------------------------------------------------------------------------------+
     | ``outputs[]`` |                                 | List of Outputs that are generated by the Tool (and accessible to fastr)       |
     |               +---------------------------------+--------------------------------------------------------------------------------+
     |               | ``id``                          | ID of the Output                                                               |
     |               +---------------------------------+--------------------------------------------------------------------------------+
     |               | ``name``                        | Longer name of the Output (more human readable)                                |
     |               +---------------------------------+--------------------------------------------------------------------------------+
@@ -534,15 +539,15 @@
         """
         Get the argument list for this interface
 
         :return: return list of arguments
         """
         # Get the argument list
         arguments = list(self.input_map.values()) + list(self.output_map.values())
-        arguments = sorted(arguments, key=lambda x: x.order if x.order >= 0 else sys.maxsize - x.order)
+        arguments = sorted(arguments, key=lambda x: x.order if x.order >= 0 else sys.maxsize + x.order)
 
         argument_list = []
 
         for argument in arguments:
             id_ = argument.id
 
             try:
@@ -766,14 +771,15 @@
             self.format = element.get('format', None)
             self.required = element.get('required', True)
             self.default = element.get('default', None)
             self.order = element.get('order', order)
             self.hidden = element.get('hidden', False)
             self.join = element.get('join', None)
             self.environ = element.get('environ', None)
+            self.via_file = element.get('via_file', False)
         else:
             raise exceptions.FastrTypeError('element should be a dict')
 
     def __eq__(self, other):
         """
         Compare two ParameterDescription instance with eachother. This
         function helps ignores the parent, but once tests the values for
@@ -823,23 +829,52 @@
                 state['datatype'] = typename
                 fastr.types.create_enumtype(typename, tuple(state['enum']), typename)
             else:
                 raise exceptions.FastrValueError('No valid datatype defined for {} in {}'.format(state['id'], state))
 
         self.__dict__.update(state)
 
+    def get_via_file_argument(self, value):
+        # Determine file contents
+        if isinstance(value, tuple):
+            arguments = [self.format_argument_value(x) for x in value]
+        elif isinstance(value, OrderedDict):
+            sep = self.join or ','
+            arguments = []
+
+            for cardinality_nr, (key, value_item) in enumerate(value.items()):
+                value_item = sep.join(self.format_argument_value(x) for x in value_item if x is not None)
+                arguments.extend(self.format_prefix('{}={}'.format(key, value_item), cardinality_nr))
+        else:
+            raise exceptions.FastrTypeError('Argument should be tuple or OrderedDict!')
+
+        # Determine filepath
+        filepath = Path(f'{self.id}.argument.txt')
+
+        # Write contents to file
+        filepath.write_text('\n'.join(arguments))
+
+        # Return new arguments pointing to file
+        return self.format_prefix(str(filepath.absolute()), 0)
+
     def get_commandline_argument(self, value):
         """
         Get the commandline argument for this Parameter given the values
         assigned to it.
 
         :param value: the value(s) for this input
         :return: commandline arguments
         :rtype: list
         """
+
+        # Swap to via_file version if needed
+        if self.via_file:
+            return self.get_via_file_argument(value)
+
+        # Continue normal flow of constructing the argument
         argument = []
         if isinstance(value, tuple):
             if self.join is not None:
                 datatype = fastr.types[self.datatype]
                 value = self.join.join(str(x if datatype.isinstance(x) else datatype(x)) for x in value),
 
             for cardinality_nr, value_item in enumerate(value):
```

### Comparing `fastr-3.3.1/fastr/resources/plugins/interfaceplugins/flowinterface.py` & `fastr-3.4.0/fastr/resources/plugins/interfaceplugins/flowinterface.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/interfaceplugins/nipypeinterface.py` & `fastr-3.4.0/fastr/resources/plugins/interfaceplugins/nipypeinterface.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/ioplugins/commaseperatedvaluefile.py` & `fastr-3.4.0/fastr/resources/plugins/ioplugins/commaseperatedvaluefile.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/ioplugins/filesystem.py` & `fastr-3.4.0/fastr/resources/plugins/ioplugins/filesystem.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/ioplugins/httpplugin.py` & `fastr-3.4.0/fastr/resources/plugins/ioplugins/httpplugin.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/ioplugins/networkscope.py` & `fastr-3.4.0/fastr/resources/plugins/ioplugins/networkscope.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/ioplugins/null.py` & `fastr-3.4.0/fastr/resources/plugins/ioplugins/null.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/ioplugins/reference.py` & `fastr-3.4.0/fastr/resources/plugins/ioplugins/reference.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/ioplugins/s3filesystem.py` & `fastr-3.4.0/fastr/resources/plugins/ioplugins/s3filesystem.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/ioplugins/test/test_virtualfilesystem.py` & `fastr-3.4.0/fastr/resources/plugins/ioplugins/test/test_virtualfilesystem.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/ioplugins/virtualfilesystem.py` & `fastr-3.4.0/fastr/resources/plugins/ioplugins/virtualfilesystem.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/ioplugins/virtualfilesystemregularexpression.py` & `fastr-3.4.0/fastr/resources/plugins/ioplugins/virtualfilesystemregularexpression.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/ioplugins/virtualfilesystemvaluelist.py` & `fastr-3.4.0/fastr/resources/plugins/ioplugins/virtualfilesystemvaluelist.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/ioplugins/xnatstorage.py` & `fastr-3.4.0/fastr/resources/plugins/ioplugins/xnatstorage.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/reportingplugins/elasticsearchreporter.py` & `fastr-3.4.0/fastr/resources/plugins/reportingplugins/elasticsearchreporter.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/reportingplugins/pimreporter.py` & `fastr-3.4.0/fastr/resources/plugins/reportingplugins/pimreporter.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/reportingplugins/simplereport.py` & `fastr-3.4.0/fastr/resources/plugins/reportingplugins/simplereport.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/targetplugins/dockertarget.py` & `fastr-3.4.0/fastr/resources/plugins/targetplugins/dockertarget.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/targetplugins/localbinarytarget.py` & `fastr-3.4.0/fastr/resources/plugins/targetplugins/localbinarytarget.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/targetplugins/macrotarget.py` & `fastr-3.4.0/fastr/resources/plugins/targetplugins/macrotarget.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/plugins/targetplugins/singularitytarget.py` & `fastr-3.4.0/fastr/resources/plugins/targetplugins/singularitytarget.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,40 +19,42 @@
 
 import os
 import subprocess
 
 import fastr
 from fastr import exceptions
 from fastr.core.target import SubprocessBasedTarget
+from fastr.helpers.classproperty import classproperty
 
 
 class SingularityTarget(SubprocessBasedTarget):
     """
     A tool target that is run using a singularity container,
-    see the `singulary website <http://singularity.lbl.gov/>`_
+    see the `Singularity website <http://singularity.lbl.gov/>`_.
 
     * ``binary (required)``: the name of the binary/script to call, can also be called ``bin``
-      for backwards compatibility.
+      for backwards compatibility. The binary/script cannot contain spaces.
     * ``container (required)``: the singularity container to run, this can be in url form for singularity
-                                pull or as a path to a local container
-
+    pull or as a path to a local container
     * ``interpreter``: the interpreter to use to call the binary e.g. ``python``
 
     """
     SINGULARITY_BIN = 'singularity'
 
     def __init__(self, binary, container, interpreter=None):
         """
         Define a new local binary target. Must be defined either using paths and optionally environment_variables
         and initscripts, or enviroment modules.
         """
         self.binary = binary
         self.container = container
         self.interpreter = interpreter
 
+        self.enable_nv = fastr.config.singularity_enable_nv
+
     def __enter__(self):
         """
         Set the environment in such a way that the target will be on the path.
         """
         super(SingularityTarget, self).__enter__()
 
         # TODO Make sure the container is present, otherwise download the container
@@ -61,14 +63,20 @@
     def __exit__(self, exc_type, exc_value, traceback):
         """
         Cleanup the environment
         """
         # TODO We could potentially remove the container again if we downloaded it in the first place?
         pass
 
+    @classproperty
+    def configuration_fields(cls):
+        return {
+            "singularity_enable_nv": (bool, False, "Enable Nvidia support in SingularityTargets"),
+        }
+
     @classmethod
     def test(cls):
         """
         Test if singularity is availble on the path
         """
         try:
             subprocess.check_output([cls.SINGULARITY_BIN, '--help'], stderr=subprocess.STDOUT)
@@ -88,17 +96,34 @@
                 continue
 
             binds.append('--bind')
             binds.append('{x}:{x}'.format(x=mount))
 
         fastr.log.info('Singularity binds: {}'.format(binds))
 
+        # Find the Singularity container pulled through FastrPI, if applicable
+        singularity_dir = os.environ.get('FASTRPI_SINGULARITY_DIR', None)
+        if singularity_dir:
+            if os.path.exists(os.path.join(singularity_dir, self.container)):
+                fastr.log.info("Container {container} was found in {fastrpi_path}.".format(
+                    container=self.container, fastrpi_path=singularity_dir))
+                container = os.path.join(singularity_dir, self.container)
+            else:
+                fastr.log.info("Container {container} cannot be found in {fastrpi_path}.".format(
+                    container=self.container, fastrpi_path=singularity_dir))
+                container = self.container
+        else:
+            container = self.container
+
         # Compose the singularity command
         singularity_command = [self.SINGULARITY_BIN, 'exec']
+        if self.enable_nv:
+            singularity_command.append('--nv')
+        # singularity_command.append('--cleanenv')
         singularity_command.extend(binds)
-        singularity_command.append(self.container)
+        singularity_command.append(container)
         singularity_command.extend(command)
 
         # Create final command
         fastr.log.debug('Command: {}'.format(command))
         fastr.log.debug('Singularity command: {}'.format(singularity_command))
         return self.call_subprocess(singularity_command)
```

### Comparing `fastr-3.3.1/fastr/resources/schemas/ConstantNode.schema.json` & `fastr-3.4.0/fastr/resources/schemas/ConstantNode.schema.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/schemas/FastrInterface.schema.json` & `fastr-3.4.0/fastr/resources/schemas/FastrInterface.schema.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/schemas/Link.schema.json` & `fastr-3.4.0/fastr/resources/schemas/Link.schema.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/schemas/Network.schema.json` & `fastr-3.4.0/fastr/resources/schemas/Network.schema.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/schemas/Node.schema.json` & `fastr-3.4.0/fastr/resources/schemas/Node.schema.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/schemas/SinkNode.schema.json` & `fastr-3.4.0/fastr/resources/schemas/SinkNode.schema.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/schemas/SourceNode.schema.json` & `fastr-3.4.0/fastr/resources/schemas/SourceNode.schema.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/schemas/Tool.schema.json` & `fastr-3.4.0/fastr/resources/schemas/Tool.schema.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/schemas/common.schema.json` & `fastr-3.4.0/fastr/resources/schemas/common.schema.json`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/__init__.py` & `fastr-3.4.0/fastr/resources/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/flow/1.0/crossvalidation.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/flow/1.0/crossvalidation.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/add.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/add.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/addint.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/addint.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/add.py` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/add.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/addint.py` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/addint.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/divide.py` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/divide.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/intdivide.py` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/intdivide.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/multiply.py` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/multiply.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/subtract.py` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/subtract.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/bin/sum.py` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/bin/sum.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/divide.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/divide.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/intdivide.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/intdivide.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/max.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/max.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/min.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/min.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/multiply.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/multiply.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/subtract.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/subtract.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/sum.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/sum.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/math/1.0/test/addint/__fastr_tool_result.pickle.gz` & `fastr-3.4.0/fastr/resources/tools/fastr/math/1.0/test/addint/__fastr_tool_result.pickle.gz`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/test/bet_docker.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/test/bet_docker.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/test/bet_singularity.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/test/bet_singularity.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/auto_prefix.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/auto_prefix.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/auto_prefix_negate.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/auto_prefix_negate.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/auto_prefix.py` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/auto_prefix.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/auto_prefix_negate.py` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/auto_prefix_negate.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/delay.py` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/delay.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/envvar.py` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/envvar.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/fail.py` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/fail.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/passthroughauto.py` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/passthroughauto.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/bin/stdout.py` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/bin/stdout.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/delay.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/delay.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/envvar.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/envvar.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/fail_0.1.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/fail_0.1.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/fail_0.2.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/fail_0.2.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/passthroughauto.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/passthroughauto.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/range.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/range.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/resources/tools/fastr/util/1.0/stdout.yaml` & `fastr-3.4.0/fastr/resources/tools/fastr/util/1.0/stdout.yaml`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/test/__init__.py` & `fastr-3.4.0/fastr/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/test/test_datatypes.py` & `fastr-3.4.0/fastr/test/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/__init__.py` & `fastr-3.4.0/fastr/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/cmd/__init__.py` & `fastr-3.4.0/fastr/utils/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/cmd/cat.py` & `fastr-3.4.0/fastr/utils/cmd/cat.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/cmd/dump.py` & `fastr-3.4.0/fastr/utils/cmd/dump.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/cmd/execute.py` & `fastr-3.4.0/fastr/utils/cmd/execute.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/cmd/extract_argparse.py` & `fastr-3.4.0/fastr/utils/cmd/extract_argparse.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/cmd/provenance.py` & `fastr-3.4.0/fastr/utils/cmd/provenance.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/cmd/pylint.py` & `fastr-3.4.0/fastr/utils/cmd/pylint.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/cmd/report.py` & `fastr-3.4.0/fastr/utils/cmd/report.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/cmd/run.py` & `fastr-3.4.0/fastr/utils/cmd/run.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/cmd/sink.py` & `fastr-3.4.0/fastr/utils/cmd/sink.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/cmd/source.py` & `fastr-3.4.0/fastr/utils/cmd/source.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/cmd/test.py` & `fastr-3.4.0/fastr/utils/cmd/test.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/cmd/trace.py` & `fastr-3.4.0/fastr/utils/cmd/trace.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/cmd/upgrade.py` & `fastr-3.4.0/fastr/utils/cmd/upgrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,20 +304,21 @@
 
     fastr.log.info('Writing output file...')
     with open(outfile, 'w') as output_file_handle:
         output_file_handle.write(code_file.dumps())
 
 
 def upgrade_tool(infile, outfile):
+    from fastr.abc.serializable import load, save
     from fastr.core.tool import Tool
 
     fastr.log.info(f'Loading tool definition from {infile}')
-    tool = Tool.loadf(infile)
+    tool = load(infile, cls=Tool)
     fastr.log.info(f'Saving new tool definition to {outfile}')
-    tool.dumpf(outfile, method='yaml')
+    save(tool, outfile, method='yaml', annotate=False)
 
 
 def main():
     """
     Upgrade a fastr 2.x python file to fastr 3.x syntax
     """
     # No arguments were parsed yet, parse them now
```

### Comparing `fastr-3.3.1/fastr/utils/cmd/verify.py` & `fastr-3.4.0/fastr/utils/cmd/verify.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/compare.py` & `fastr-3.4.0/fastr/utils/compare.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/dicteq.py` & `fastr-3.4.0/fastr/utils/dicteq.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/gettools.py` & `fastr-3.4.0/fastr/utils/gettools.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/multiprocesswrapper.py` & `fastr-3.4.0/fastr/utils/multiprocesswrapper.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/utils/verify.py` & `fastr-3.4.0/fastr/utils/verify.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr/version.py` & `fastr-3.4.0/fastr/version.py`

 * *Files identical despite different names*

### Comparing `fastr-3.3.1/fastr.egg-info/PKG-INFO` & `fastr-3.4.0/fastr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastr
-Version: 3.3.1
+Version: 3.4.0
 Summary: Workflow creation and batch execution environment.
 Home-page: https://gitlab.com/radiology/infrastructure/fastr
 Author: H.C. Achterberg, M. Koek
 Author-email: hakim.achterberg@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `fastr-3.3.1/fastr.egg-info/SOURCES.txt` & `fastr-3.4.0/fastr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,33 +42,14 @@
 fastr/core/test/test_samples.py
 fastr/core/test/test_tool.py
 fastr/core/test/test_version.py
 fastr/core/test/test_vfs.py
 fastr/data/__init__.py
 fastr/data/url.py
 fastr/datatypes/__init__.py
-fastr/doc/Makefile
-fastr/doc/conf.py
-fastr/doc/doc_clean.py
-fastr/doc/doc_generate.py
-fastr/doc/generate_cmd.py
-fastr/doc/generate_config.py
-fastr/doc/generate_modules.py
-fastr/doc/generate_plugins.py
-fastr/doc/index.template
-fastr/doc/make.bat
-fastr/doc/static/changelog.rst
-fastr/doc/static/development.rst
-fastr/doc/static/file_description.rst
-fastr/doc/static/introduction.rst
-fastr/doc/static/quick_start.rst
-fastr/doc/static/tools.rst
-fastr/doc/static/user_manual.rst
-fastr/doc/static/images/fastr_core.png
-fastr/doc/static/images/tools/tooldefresolveflowchart.png
 fastr/examples/__generate_reference__.py
 fastr/examples/__init__.py
 fastr/examples/add_ints.py
 fastr/examples/add_ints_missing.py
 fastr/examples/add_ints_s3.py
 fastr/examples/advanced_linking.py
 fastr/examples/auto_prefix.py
@@ -85,14 +66,15 @@
 fastr/examples/failing_network_missing.py
 fastr/examples/filecopy.py
 fastr/examples/input_groups.py
 fastr/examples/macro_node.py
 fastr/examples/macro_node2.py
 fastr/examples/shift_links.py
 fastr/examples/source_sink.py
+fastr/examples/via_file_argument.py
 fastr/examples/data/hello.txt
 fastr/examples/data/add_ints/value
 fastr/examples/data/add_ints/values
 fastr/examples/data/add_ints/values_duplicate
 fastr/examples/data/images/mrwhite.mhd
 fastr/examples/data/images/mrwhite.raw
 fastr/examples/data/images/mrwhite_duplicate.mhd
@@ -578,23 +560,25 @@
 fastr/resources/tools/fastr/math/1.0/divide.yaml
 fastr/resources/tools/fastr/math/1.0/intdivide.yaml
 fastr/resources/tools/fastr/math/1.0/max.yaml
 fastr/resources/tools/fastr/math/1.0/min.yaml
 fastr/resources/tools/fastr/math/1.0/multiply.yaml
 fastr/resources/tools/fastr/math/1.0/subtract.yaml
 fastr/resources/tools/fastr/math/1.0/sum.yaml
+fastr/resources/tools/fastr/math/1.0/sum_via_file.yaml
 fastr/resources/tools/fastr/math/1.0/bin/add.py
 fastr/resources/tools/fastr/math/1.0/bin/addint.py
 fastr/resources/tools/fastr/math/1.0/bin/divide.py
 fastr/resources/tools/fastr/math/1.0/bin/intdivide.py
 fastr/resources/tools/fastr/math/1.0/bin/max.py
 fastr/resources/tools/fastr/math/1.0/bin/min.py
 fastr/resources/tools/fastr/math/1.0/bin/multiply.py
 fastr/resources/tools/fastr/math/1.0/bin/subtract.py
 fastr/resources/tools/fastr/math/1.0/bin/sum.py
+fastr/resources/tools/fastr/math/1.0/bin/sum_via_file.py
 fastr/resources/tools/fastr/math/1.0/test/addint/__fastr_tool_ref__.json
 fastr/resources/tools/fastr/math/1.0/test/addint/__fastr_tool_result.pickle.gz
 fastr/resources/tools/fastr/math/1.0/test/addint/__output__fastr_tool_ref__.json
 fastr/resources/tools/fastr/test/bet_docker.yaml
 fastr/resources/tools/fastr/test/bet_singularity.yaml
 fastr/resources/tools/fastr/util/__init__.py
 fastr/resources/tools/fastr/util/1.0/__init__.py
```

### Comparing `fastr-3.3.1/setup.py` & `fastr-3.4.0/setup.py`

 * *Files identical despite different names*

