# Comparing `tmp/krixik-1.1.16.tar.gz` & `tmp/krixik-1.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krixik-1.1.16.tar", last modified: Tue May 14 22:06:18 2024, max compression
+gzip compressed data, was "krixik-1.1.17.tar", last modified: Wed May 22 23:08:15 2024, max compression
```

## Comparing `krixik-1.1.16.tar` & `krixik-1.1.17.tar`

### file list

```diff
@@ -1,234 +1,234 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.110043 krixik-1.1.16/
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-14 22:06:18.110043 krixik-1.1.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-05-14 22:06:07.000000 krixik-1.1.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.082043 krixik-1.1.16/krixik/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/__base__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       60 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.082043 krixik-1.1.16/krixik/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.082043 krixik-1.1.16/krixik/modules/caption/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/caption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/caption/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/caption/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/caption/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.086043 krixik-1.1.16/krixik/modules/json-to-txt/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/json-to-txt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/json-to-txt/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/json-to-txt/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/json-to-txt/module.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/json-to-txt/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.086043 krixik-1.1.16/krixik/modules/keyword-db/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/keyword-db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/keyword-db/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/keyword-db/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/keyword-db/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.086043 krixik-1.1.16/krixik/modules/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/ocr/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/ocr/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/ocr/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.086043 krixik-1.1.16/krixik/modules/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/parser/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/parser/module.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/parser/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.086043 krixik-1.1.16/krixik/modules/sentiment/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/sentiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/sentiment/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/sentiment/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/sentiment/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.086043 krixik-1.1.16/krixik/modules/summarize/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/summarize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/summarize/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/summarize/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/summarize/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.090043 krixik-1.1.16/krixik/modules/text-embedder/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/text-embedder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/text-embedder/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/text-embedder/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/text-embedder/module.yml
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/text-embedder/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.090043 krixik-1.1.16/krixik/modules/transcribe/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/transcribe/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/transcribe/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/transcribe/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.090043 krixik-1.1.16/krixik/modules/translate/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/translate/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/translate/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/translate/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.090043 krixik-1.1.16/krixik/modules/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/utilities/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/utilities/io_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/utilities/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/utilities/model_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/utilities/module_selections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/utilities/read_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.090043 krixik-1.1.16/krixik/modules/vector-db/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/vector-db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/vector-db/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/vector-db/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/modules/vector-db/module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.090043 krixik-1.1.16/krixik/pipeline_builder/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.094043 krixik-1.1.16/krixik/pipeline_builder/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/utilities/chain_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/utilities/config_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/utilities/input_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/utilities/name_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/utilities/savepath_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_builder/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.094043 krixik-1.1.16/krixik/pipeline_examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.094043 krixik-1.1.16/krixik/pipeline_examples/single_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/caption.yml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/json-to-txt.yml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/keyword-db.yml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/ocr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/parser.yml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/sentiment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/summarize.yml
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/text-embedder.yml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/transcribe.yml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/translate.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.094043 krixik-1.1.16/krixik/pipeline_examples/single_module/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/utilities/generate_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/pipeline_examples/single_module/vector-db.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.094043 krixik-1.1.16/krixik/system_builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26703 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.098043 krixik-1.1.16/krixik/system_builder/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/check_process_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/fetch_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/keyword_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/list_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/semantic_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/show_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/functions/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.098043 krixik-1.1.16/krixik/system_builder/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/system_builder/utilities/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.098043 krixik-1.1.16/krixik/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      386 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/cleaners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.098043 krixik-1.1.16/krixik/utilities/converters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/default_clean_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/docx_to_txt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/pdf_to_txt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/pptx_to_txt.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/read_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/unclean_to_clean_txt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.098043 krixik-1.1.16/krixik/utilities/converters/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/utilities/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/utilities/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/converters/video_to_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/file_name_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/tree_illustrator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1486 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.102043 krixik-1.1.16/krixik/utilities/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.102043 krixik-1.1.16/krixik/utilities/validators/data/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/docx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/npy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/pptx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.102043 krixik-1.1.16/krixik/utilities/validators/data/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/utilities/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/utilities/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/utilities/read_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/data/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.102043 krixik-1.1.16/krixik/utilities/validators/system/
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.106043 krixik-1.1.16/krixik/utilities/validators/system/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/clean_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/download_output.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/expire_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/extension_enforcer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1237 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/file_description.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2773 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/file_ids.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5749 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/file_names.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4957 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/file_tags.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/k_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/local_file_path.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      795 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/local_save_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/lower_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/max_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/process_switches.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1146 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/request_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/sort_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/symbolic_path_splitter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9255 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/symbolic_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/timestamp_bookends.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/use_default_clean_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/user_secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.106043 krixik-1.1.16/krixik/utilities/validators/system/base/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/utilities/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/verbose.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/base/wait_for_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.106043 krixik-1.1.16/krixik/utilities/validators/system/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.106043 krixik-1.1.16/krixik/utilities/validators/system/data/audio/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/audio/file_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/audio/local_file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/audio/symbolic_file_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.110043 krixik-1.1.16/krixik/utilities/validators/system/data/image/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/image/file_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/image/local_file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/image/symbolic_file_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.110043 krixik-1.1.16/krixik/utilities/validators/system/data/json/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/json/file_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/json/local_file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/json/symbolic_file_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.110043 krixik-1.1.16/krixik/utilities/validators/system/data/npy/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/npy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/npy/file_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/npy/local_file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/npy/symbolic_file_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.110043 krixik-1.1.16/krixik/utilities/validators/system/data/text/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/text/file_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/text/local_file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/text/symbolic_file_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.110043 krixik-1.1.16/krixik/utilities/validators/system/data/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/system/data/utilities/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.110043 krixik-1.1.16/krixik/utilities/validators/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-14 22:06:07.000000 krixik-1.1.16/krixik/utilities/validators/utilities/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:06:18.082043 krixik-1.1.16/krixik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-14 22:06:18.000000 krixik-1.1.16/krixik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-14 22:06:18.000000 krixik-1.1.16/krixik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 22:06:18.000000 krixik-1.1.16/krixik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-14 22:06:18.000000 krixik-1.1.16/krixik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 22:06:18.000000 krixik-1.1.16/krixik.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 22:06:18.110043 krixik-1.1.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-14 22:06:07.000000 krixik-1.1.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.844376 krixik-1.1.17/
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-22 23:08:15.844376 krixik-1.1.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-22 23:08:08.000000 krixik-1.1.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.816377 krixik-1.1.17/krixik/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/__base__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       60 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.816377 krixik-1.1.17/krixik/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.816377 krixik-1.1.17/krixik/modules/caption/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/caption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/caption/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/caption/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/caption/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.816377 krixik-1.1.17/krixik/modules/json-to-txt/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/json-to-txt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/json-to-txt/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/json-to-txt/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/json-to-txt/module.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/json-to-txt/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.820376 krixik-1.1.17/krixik/modules/keyword-db/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/keyword-db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/keyword-db/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/keyword-db/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/keyword-db/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.820376 krixik-1.1.17/krixik/modules/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/ocr/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/ocr/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/ocr/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.820376 krixik-1.1.17/krixik/modules/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/parser/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/parser/module.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/parser/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.820376 krixik-1.1.17/krixik/modules/sentiment/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/sentiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/sentiment/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/sentiment/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/sentiment/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.820376 krixik-1.1.17/krixik/modules/summarize/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/summarize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/summarize/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/summarize/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/summarize/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.820376 krixik-1.1.17/krixik/modules/text-embedder/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/text-embedder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/text-embedder/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/text-embedder/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/text-embedder/module.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/text-embedder/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.824376 krixik-1.1.17/krixik/modules/transcribe/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/transcribe/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/transcribe/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/transcribe/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.824376 krixik-1.1.17/krixik/modules/translate/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/translate/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/translate/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/translate/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.824376 krixik-1.1.17/krixik/modules/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/utilities/io_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/utilities/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/utilities/model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/utilities/module_selections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/utilities/read_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.824376 krixik-1.1.17/krixik/modules/vector-db/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/vector-db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/vector-db/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/vector-db/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/modules/vector-db/module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.824376 krixik-1.1.17/krixik/pipeline_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_builder/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_builder/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.828376 krixik-1.1.17/krixik/pipeline_builder/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_builder/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_builder/utilities/chain_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_builder/utilities/config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_builder/utilities/input_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_builder/utilities/name_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_builder/utilities/savepath_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_builder/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.828376 krixik-1.1.17/krixik/pipeline_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.828376 krixik-1.1.17/krixik/pipeline_examples/single_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_examples/single_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_examples/single_module/caption.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_examples/single_module/json-to-txt.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_examples/single_module/keyword-db.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_examples/single_module/ocr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_examples/single_module/parser.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_examples/single_module/sentiment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_examples/single_module/summarize.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_examples/single_module/text-embedder.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_examples/single_module/transcribe.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_examples/single_module/translate.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.828376 krixik-1.1.17/krixik/pipeline_examples/single_module/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_examples/single_module/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_examples/single_module/utilities/generate_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/pipeline_examples/single_module/vector-db.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.828376 krixik-1.1.17/krixik/system_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/system_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26687 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/system_builder/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.832376 krixik-1.1.17/krixik/system_builder/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/system_builder/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/system_builder/functions/check_process_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/system_builder/functions/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/system_builder/functions/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/system_builder/functions/fetch_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/system_builder/functions/keyword_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/system_builder/functions/list_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/system_builder/functions/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/system_builder/functions/semantic_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/system_builder/functions/show_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/system_builder/functions/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.832376 krixik-1.1.17/krixik/system_builder/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/system_builder/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/system_builder/utilities/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.832376 krixik-1.1.17/krixik/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      386 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/cleaners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.832376 krixik-1.1.17/krixik/utilities/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/converters/default_clean_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/converters/docx_to_txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/converters/pdf_to_txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/converters/pptx_to_txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/converters/read_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/converters/unclean_to_clean_txt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.832376 krixik-1.1.17/krixik/utilities/converters/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/converters/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/converters/utilities/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/converters/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/converters/video_to_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/file_name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/tree_illustrator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1486 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.832376 krixik-1.1.17/krixik/utilities/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.836377 krixik-1.1.17/krixik/utilities/validators/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/data/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/data/docx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/data/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/data/npy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/data/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/data/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/data/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.836377 krixik-1.1.17/krixik/utilities/validators/data/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/data/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/data/utilities/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/data/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/data/utilities/read_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/data/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.836377 krixik-1.1.17/krixik/utilities/validators/system/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.840376 krixik-1.1.17/krixik/utilities/validators/system/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/clean_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/download_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/expire_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/extension_enforcer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1237 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/file_description.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2773 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/file_ids.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5749 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/file_names.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4957 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/file_tags.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/k_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/local_file_path.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      795 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/local_save_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/lower_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/max_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/process_switches.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1146 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/request_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/sort_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/symbolic_path_splitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9255 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/symbolic_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/timestamp_bookends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/use_default_clean_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/user_secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.840376 krixik-1.1.17/krixik/utilities/validators/system/base/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/base/wait_for_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.840376 krixik-1.1.17/krixik/utilities/validators/system/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.840376 krixik-1.1.17/krixik/utilities/validators/system/data/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/audio/file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/audio/local_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/audio/symbolic_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.840376 krixik-1.1.17/krixik/utilities/validators/system/data/image/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/image/file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/image/local_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/image/symbolic_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.844376 krixik-1.1.17/krixik/utilities/validators/system/data/json/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/json/file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/json/local_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/json/symbolic_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.844376 krixik-1.1.17/krixik/utilities/validators/system/data/npy/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/npy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/npy/file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/npy/local_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/npy/symbolic_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.844376 krixik-1.1.17/krixik/utilities/validators/system/data/text/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/text/file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/text/local_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/text/symbolic_file_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.844376 krixik-1.1.17/krixik/utilities/validators/system/data/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/system/data/utilities/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.844376 krixik-1.1.17/krixik/utilities/validators/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-22 23:08:08.000000 krixik-1.1.17/krixik/utilities/validators/utilities/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:15.816377 krixik-1.1.17/krixik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-22 23:08:15.000000 krixik-1.1.17/krixik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-22 23:08:15.000000 krixik-1.1.17/krixik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 23:08:15.000000 krixik-1.1.17/krixik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-22 23:08:15.000000 krixik-1.1.17/krixik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 23:08:15.000000 krixik-1.1.17/krixik.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 23:08:15.844376 krixik-1.1.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-22 23:08:08.000000 krixik-1.1.17/setup.py
```

### Comparing `krixik-1.1.16/PKG-INFO` & `krixik-1.1.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krixik
-Version: 1.1.16
+Version: 1.1.17
 Summary: Easily assemble and serverlessly consume modular AI pipelines through secure Python APIs.
 Home-page: https://github.com/krixik-ai/krixik-cli
 Author: Jeremy Watt
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: linting
 Provides-Extra: testing
@@ -118,15 +118,15 @@
 ```python
 my_pipeline_1 = krixik.load_pipeline(pipeline=custom_pipeline_1)
 ```
 
 The pipeline is ready! Now you can process audio and video files through it to generate transcripts of them.
 
 ```python
-my_pipeline_1.process(local_file_path='./path/to/my/mp3/or/mp4')
+my_pipeline_1.process(local_file_path='./path/to/my/mp3')
 ```
 
 The outputs of this pipeline will be a timestamped transcript of your input audio/video file, a `file_id` for the processed file, and a `process_id` for the process itself.
 
 
 ### Extending your pipeline
```

### Comparing `krixik-1.1.16/README.md` & `krixik-1.1.17/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 ```python
 my_pipeline_1 = krixik.load_pipeline(pipeline=custom_pipeline_1)
 ```
 
 The pipeline is ready! Now you can process audio and video files through it to generate transcripts of them.
 
 ```python
-my_pipeline_1.process(local_file_path='./path/to/my/mp3/or/mp4')
+my_pipeline_1.process(local_file_path='./path/to/my/mp3')
 ```
 
 The outputs of this pipeline will be a timestamped transcript of your input audio/video file, a `file_id` for the processed file, and a `process_id` for the process itself.
 
 
 ### Extending your pipeline
```

### Comparing `krixik-1.1.16/krixik/main.py` & `krixik-1.1.17/krixik/main.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/__init__.py` & `krixik-1.1.17/krixik/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/caption/io.py` & `krixik-1.1.17/krixik/modules/caption/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/caption/models.py` & `krixik-1.1.17/krixik/modules/caption/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/json-to-txt/io.py` & `krixik-1.1.17/krixik/modules/json-to-txt/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/json-to-txt/models.py` & `krixik-1.1.17/krixik/modules/json-to-txt/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/json-to-txt/params.py` & `krixik-1.1.17/krixik/modules/json-to-txt/params.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/keyword-db/io.py` & `krixik-1.1.17/krixik/modules/keyword-db/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/keyword-db/models.py` & `krixik-1.1.17/krixik/modules/keyword-db/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/ocr/io.py` & `krixik-1.1.17/krixik/modules/ocr/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/ocr/models.py` & `krixik-1.1.17/krixik/modules/ocr/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/parser/io.py` & `krixik-1.1.17/krixik/modules/parser/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/parser/models.py` & `krixik-1.1.17/krixik/modules/parser/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/parser/params.py` & `krixik-1.1.17/krixik/modules/parser/params.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/sentiment/io.py` & `krixik-1.1.17/krixik/modules/sentiment/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/sentiment/models.py` & `krixik-1.1.17/krixik/modules/sentiment/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/summarize/io.py` & `krixik-1.1.17/krixik/modules/summarize/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/summarize/models.py` & `krixik-1.1.17/krixik/modules/summarize/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/text-embedder/io.py` & `krixik-1.1.17/krixik/modules/text-embedder/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/text-embedder/models.py` & `krixik-1.1.17/krixik/modules/text-embedder/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/text-embedder/module.yml` & `krixik-1.1.17/krixik/modules/text-embedder/module.yml`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/transcribe/io.py` & `krixik-1.1.17/krixik/modules/transcribe/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/transcribe/models.py` & `krixik-1.1.17/krixik/modules/transcribe/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/translate/io.py` & `krixik-1.1.17/krixik/modules/translate/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/translate/models.py` & `krixik-1.1.17/krixik/modules/translate/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/utilities/decorators.py` & `krixik-1.1.17/krixik/modules/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/utilities/io_validator.py` & `krixik-1.1.17/krixik/modules/utilities/io_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import copy
 import importlib
 from krixik.utilities.validators.data import available_data_types
 
 
 def format_checker(format_: str, local_file_path: str) -> None:
     if format_ not in available_data_types:
-        raise ValueError("FAILURE: format not supported")
+        raise ValueError(f"FAILURE: format {format_} not yet supported")
 
     if format_ == "json":
         try:
             with open(local_file_path, "r") as file:
                 data = json.load(file)
                 first_dict = data[0]
         except Exception as e:
```

### Comparing `krixik-1.1.16/krixik/modules/utilities/model.py` & `krixik-1.1.17/krixik/modules/utilities/model.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/utilities/module_selections.py` & `krixik-1.1.17/krixik/modules/utilities/module_selections.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/utilities/read_config.py` & `krixik-1.1.17/krixik/modules/utilities/read_config.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/vector-db/io.py` & `krixik-1.1.17/krixik/modules/vector-db/io.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/modules/vector-db/models.py` & `krixik-1.1.17/krixik/modules/vector-db/models.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/pipeline_builder/module.py` & `krixik-1.1.17/krixik/pipeline_builder/module.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/pipeline_builder/pipeline.py` & `krixik-1.1.17/krixik/pipeline_builder/pipeline.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/pipeline_builder/utilities/chain_checker.py` & `krixik-1.1.17/krixik/pipeline_builder/utilities/chain_checker.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/pipeline_builder/utilities/config_checker.py` & `krixik-1.1.17/krixik/pipeline_builder/utilities/config_checker.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/pipeline_builder/utilities/input_checker.py` & `krixik-1.1.17/krixik/pipeline_builder/utilities/input_checker.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/pipeline_builder/utilities.py` & `krixik-1.1.17/krixik/pipeline_builder/utilities.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/pipeline_examples/single_module/text-embedder.yml` & `krixik-1.1.17/krixik/pipeline_examples/single_module/text-embedder.yml`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/pipeline_examples/single_module/utilities/generate_examples.py` & `krixik-1.1.17/krixik/pipeline_examples/single_module/utilities/generate_examples.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/system_builder/base.py` & `krixik-1.1.17/krixik/system_builder/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,15 +439,15 @@
         wait_for_process : bool, optional
             whether to process the file asynchronously, by default False
         local_save_directory: str
             local directory for process output, by default os.getcwd()
         download_output: bool
             boolean switch, download process output (set True) or not (set False)
         og_local_file_path: str, optional
-            local file path used for any file conversion (e.g., mp4 to mp3, controlled internally
+            local file path used for any file conversion - controlled internally
         Returns
         -------
         dict | None
             a dictionary containing the status_code, request_id, and message indicating success or failure
         """
 
         if local_file_path is None:
@@ -556,15 +556,15 @@
         if not download_output:
             vprint("INFO: downlaod_output set to False, not fetching output", verbose=verbose)
 
         if download_output and output_data is not None:
             try:
                 file_id = output_data["file_id"]
                 file_output = self.fetch_output(file_id=file_id, local_save_directory=local_save_directory)
-                vprint("SUCCESS: process output downloaded", verbose=verbose)
+                vprint("SUCCESS: process output downloaded.", verbose=verbose)
                 return file_output
             except Exception as e:
                 raise e
         output_data["status_code"] = 200
         return output_data
 
     @kwargs_checker
```

### Comparing `krixik-1.1.16/krixik/system_builder/functions/check_process_status.py` & `krixik-1.1.17/krixik/system_builder/functions/check_process_status.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/system_builder/functions/checkin.py` & `krixik-1.1.17/krixik/system_builder/functions/checkin.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/system_builder/functions/delete.py` & `krixik-1.1.17/krixik/system_builder/functions/delete.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/system_builder/functions/fetch_output.py` & `krixik-1.1.17/krixik/system_builder/functions/fetch_output.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/system_builder/functions/keyword_search.py` & `krixik-1.1.17/krixik/system_builder/functions/keyword_search.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/system_builder/functions/list_files.py` & `krixik-1.1.17/krixik/system_builder/functions/list_files.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/system_builder/functions/process.py` & `krixik-1.1.17/krixik/system_builder/functions/process.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/system_builder/functions/semantic_search.py` & `krixik-1.1.17/krixik/system_builder/functions/semantic_search.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/system_builder/functions/show_tree.py` & `krixik-1.1.17/krixik/system_builder/functions/show_tree.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/system_builder/functions/update.py` & `krixik-1.1.17/krixik/system_builder/functions/update.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/system_builder/utilities/decorators.py` & `krixik-1.1.17/krixik/system_builder/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/converters/default_clean_options.py` & `krixik-1.1.17/krixik/utilities/converters/default_clean_options.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/converters/docx_to_txt.py` & `krixik-1.1.17/krixik/utilities/converters/docx_to_txt.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/converters/pdf_to_txt.py` & `krixik-1.1.17/krixik/utilities/converters/pdf_to_txt.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/converters/pptx_to_txt.py` & `krixik-1.1.17/krixik/utilities/converters/pptx_to_txt.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/converters/unclean_to_clean_txt.py` & `krixik-1.1.17/krixik/utilities/converters/unclean_to_clean_txt.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/converters/utilities/decorators.py` & `krixik-1.1.17/krixik/utilities/converters/utilities/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from krixik.utilities.converters.read_config import convert_extension
 from krixik.utilities.converters.unclean_to_clean_txt import (
     convert as convert_unclean_text,
 )
 from krixik.utilities.converters.docx_to_txt import convert as convert_docx
 from krixik.utilities.converters.pdf_to_txt import convert as convert_pdf
 from krixik.utilities.converters.pptx_to_txt import convert as convert_pptx
-from krixik.utilities.converters.video_to_audio import convert as convert_video
+
+# from krixik.utilities.converters.video_to_audio import convert as convert_video
 from krixik.utilities.utilities import vprint, get_input
 
 
 def datatype_converter_wrapper(func):
     @wraps(func)
     def converter_wrapper(*args, **kwargs):
         try:
@@ -23,21 +24,21 @@
 
             if local_file_path is not None:
                 extension = local_file_path.split(".")[-1]
                 conversion = convert_extension(extension)
                 if conversion is not None:
                     with tempfile.TemporaryDirectory() as conversion_save_directory:
                         og_local_file_path = copy.deepcopy(local_file_path)
-                        if extension == "mp4":
-                            local_file_path = convert_video(
-                                local_file_path=local_file_path,
-                                local_save_directory=conversion_save_directory,
-                                verbose=verbose,
-                            )
-                        elif extension == "pdf":
+                        # if extension == "mp4":
+                        #     local_file_path = convert_video(
+                        #         local_file_path=local_file_path,
+                        #         local_save_directory=conversion_save_directory,
+                        #         verbose=verbose,
+                        #     )
+                        if extension == "pdf":
                             local_file_path = convert_pdf(
                                 local_file_path=local_file_path,
                                 local_save_directory=conversion_save_directory,
                                 verbose=verbose,
                             )
                         elif extension == "docx":
                             local_file_path = convert_docx(
```

### Comparing `krixik-1.1.16/krixik/utilities/converters/video_to_audio.py` & `krixik-1.1.17/krixik/utilities/converters/video_to_audio.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,99 +1,101 @@
-import os
-from moviepy.editor import VideoFileClip
-from krixik.utilities.validators.system.base.utilities.decorators import (
-    file_converters_input_check,
-)
-from krixik.utilities.validators.data.video import is_size as is_video_size
-from krixik.utilities.validators.data.audio import is_size as is_audio_size
-from krixik.utilities.utilities import vprint
-
-
-def delete_file(*, file_path: str, exception: str) -> None:
-    if file_path is not None:
-        if os.path.exists(file_path):
-            os.remove(file_path)
-        raise ValueError(f"audio extraction failed with exception: {str(exception)}")
-
-
-@file_converters_input_check
-def extract_audio(*, local_file_path: str, audio_filepath: str) -> None:
-    try:
-        video = VideoFileClip(local_file_path)
-        audio = video.audio
-        if audio is not None:
-            audio.write_audiofile(audio_filepath, verbose=False, logger=None)
-    except Exception as e:
-        raise ValueError(f"error extracting audio from video {local_file_path}, exception: {e}")
-
-
-@file_converters_input_check
-def convert(
-    *,
-    local_file_path: str | None,
-    local_save_directory: str | None,
-    verbose: bool = True,
-) -> str:
-    """video to audio converter - strips audio mp3 from video file using moviepy library
-
-    Parameters
-    ----------
-    local_file_path : str | None
-        path to local file to convert
-    local_save_directory : str | None
-        local directory to save converted file
-    verbose : bool, optional
-        by default True
-
-    Returns
-    -------
-    str | None
-        if conversion successful returns path to converted file
-    """
-
-    if local_file_path is not None and local_save_directory is not None:
-        audio_filepath = None
-        try:
-            # get file_name video_file_path
-            file_name = "krixik_converted_version_" + os.path.splitext(os.path.basename(local_file_path))[0]
-
-            # format audio file path
-            extension = ".mp3"
-            audio_filepath = os.path.join(local_save_directory, file_name + extension)
-
-            # remove file if it already exists
-            if os.path.exists(audio_filepath):
-                os.remove(audio_filepath)
-
-            # check input file is mp4
-            is_video_size(local_file_path=local_file_path, minimum_file_size=0.1)
-
-            # extract audio from video
-            extract_audio(local_file_path=local_file_path, audio_filepath=audio_filepath)
-
-            # report size check
-            vprint(
-                "INFO: Checking that file size falls within acceptable parameters...",
-                verbose=verbose,
-            )
-            is_audio_size(local_file_path=audio_filepath, minimum_file_size=0.05)
-            vprint("INFO:...success!", verbose=verbose)
-
-            return audio_filepath
-        except ValueError as ve:
-            vprint(
-                "INFO:...failure!  The converted (audio) file does not fall within acceptable size parameters.",
-                verbose=verbose,
-            )
-            if audio_filepath is not None:
-                delete_file(file_path=audio_filepath, exception=str(ve))
-            raise
-        except AttributeError as ae:
-            if audio_filepath is not None:
-                delete_file(file_path=audio_filepath, exception=str(ae))
-            raise ValueError(f"video contains no visual content, cannot convert to audio - {local_file_path}")
-        except Exception as e:
-            if audio_filepath is not None:
-                delete_file(file_path=audio_filepath, exception=str(e))
-            raise
-    else:
-        raise ValueError("the input local_file_path and/or local_save_directory is null")
+# import os
+# from moviepy.editor import VideoFileClip
+# from krixik.utilities.validators.system.base.utilities.decorators import (
+#     file_converters_input_check,
+# )
+# from krixik.utilities.validators.data.video import is_size as is_video_size
+# from krixik.utilities.validators.data.audio import is_size as is_audio_size
+# from krixik.utilities.utilities import vprint
+
+
+# def delete_file(*, file_path: str, exception: str) -> None:
+#     if file_path is not None:
+#         if os.path.exists(file_path):
+#             os.remove(file_path)
+#         raise ValueError(f"audio extraction failed with exception: {str(exception)}")
+
+
+# @file_converters_input_check
+# def extract_audio(*, local_file_path: str, audio_filepath: str) -> None:
+#     try:
+#         video = VideoFileClip(local_file_path)
+#         audio = video.audio
+#         if audio is not None:
+#             audio.write_audiofile(audio_filepath, verbose=False, logger=None)
+#             audio.close()
+#             video.close()
+#     except Exception as e:
+#         raise ValueError(f"error extracting audio from video {local_file_path}, exception: {e}")
+
+
+# @file_converters_input_check
+# def convert(
+#     *,
+#     local_file_path: str | None,
+#     local_save_directory: str | None,
+#     verbose: bool = True,
+# ) -> str:
+#     """video to audio converter - strips audio mp3 from video file using moviepy library
+
+#     Parameters
+#     ----------
+#     local_file_path : str | None
+#         path to local file to convert
+#     local_save_directory : str | None
+#         local directory to save converted file
+#     verbose : bool, optional
+#         by default True
+
+#     Returns
+#     -------
+#     str | None
+#         if conversion successful returns path to converted file
+#     """
+
+#     if local_file_path is not None and local_save_directory is not None:
+#         audio_filepath = None
+#         try:
+#             # get file_name video_file_path
+#             file_name = "krixik_converted_version_" + os.path.splitext(os.path.basename(local_file_path))[0]
+
+#             # format audio file path
+#             extension = ".mp3"
+#             audio_filepath = os.path.join(local_save_directory, file_name + extension)
+
+#             # remove file if it already exists
+#             if os.path.exists(audio_filepath):
+#                 os.remove(audio_filepath)
+
+#             # check input file is mp4
+#             is_video_size(local_file_path=local_file_path, minimum_file_size=0.1)
+
+#             # extract audio from video
+#             extract_audio(local_file_path=local_file_path, audio_filepath=audio_filepath)
+
+#             # report size check
+#             vprint(
+#                 "INFO: Checking that file size falls within acceptable parameters...",
+#                 verbose=verbose,
+#             )
+#             is_audio_size(local_file_path=audio_filepath, minimum_file_size=0.05)
+#             vprint("INFO:...success!", verbose=verbose)
+
+#             return audio_filepath
+#         except ValueError as ve:
+#             vprint(
+#                 "INFO:...failure!  The converted (audio) file does not fall within acceptable size parameters.",
+#                 verbose=verbose,
+#             )
+#             if audio_filepath is not None:
+#                 delete_file(file_path=audio_filepath, exception=str(ve))
+#             raise
+#         except AttributeError as ae:
+#             if audio_filepath is not None:
+#                 delete_file(file_path=audio_filepath, exception=str(ae))
+#             raise ValueError(f"video contains no visual content, cannot convert to audio - {local_file_path}")
+#         except Exception as e:
+#             if audio_filepath is not None:
+#                 delete_file(file_path=audio_filepath, exception=str(e))
+#             raise
+#     else:
+#         raise ValueError("the input local_file_path and/or local_save_directory is null")
```

### Comparing `krixik-1.1.16/krixik/utilities/file_name_generator.py` & `krixik-1.1.17/krixik/utilities/file_name_generator.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/tree_illustrator.py` & `krixik-1.1.17/krixik/utilities/tree_illustrator.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/utilities.py` & `krixik-1.1.17/krixik/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/data/audio.py` & `krixik-1.1.17/krixik/utilities/validators/data/video.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,75 +1,79 @@
 import os
-from pydub import AudioSegment
-from moviepy.editor import AudioFileClip
+from moviepy.editor import VideoFileClip
 from pydub.exceptions import PydubException
 
 
-def is_valid(local_file_path: str | None) -> None:
-    if local_file_path is None:
-        raise ValueError("input file is None")
+def is_valid(local_file_path: str) -> None:
+    if not os.path.exists(local_file_path):
+        raise ValueError(f"input file does not exist - {local_file_path}")
+
+    if not local_file_path.endswith(".mp4"):
+        raise ValueError(f"input file must end with .mp4 extension, not a valid video file - {local_file_path}")
 
-    # check that local_file_path represents audio file
     try:
-        duration = 100
-        AudioSegment.from_file(local_file_path, format="mp3", duration=duration)
-    except PydubException as e:
-        raise ValueError(f"input file is not a valid audio file - {local_file_path} - see exception {e}")
+        start_time = 0
+        end_time = 3
+        clip = VideoFileClip(local_file_path).subclip(start_time, end_time)
+        clip.close()
+    except PydubException:
+        raise ValueError(f"input file is not a valid video file - {local_file_path}")
     except FileNotFoundError:
         raise FileNotFoundError(f"The file '{local_file_path}' does not exist.")
     except Exception as e:
-        raise ValueError(f"Error reading audio: {e}")
+        raise ValueError(f"video validation failed with exception {e}")
 
 
 def is_size(
     *,
     local_file_path: str,
     minimum_seconds: int = 1,
     maximum_seconds: int = 180,
-    minimum_file_size: float = 0.00001,
-    maximum_file_size: float = 3.000001,
+    minimum_file_size: float = 0.2,
+    maximum_file_size: float = 100.000001,
 ) -> None:
     # proper size
     def compute_size(file_path: str):
         try:
             # Get the size of the file in bytes
             file_size_bytes = os.path.getsize(file_path)
 
             # Convert the size to megabytes (MB)
             file_size_mb = file_size_bytes / (1024 * 1024)
             return file_size_mb
         except Exception as e:
-            raise ValueError(f"audio extraction failed with exception {e}")
+            raise ValueError(f"audio compute size failed with exception {e}")
 
-    def compute_duration(file_path: str) -> float:
+    def compute_duration(file_path):
         try:
-            audio_clip = AudioFileClip(file_path)
-            duration_in_seconds = round(audio_clip.duration, 1)
+            video_clip = VideoFileClip(file_path)
+            duration_in_seconds = round(video_clip.duration, 1)
             return duration_in_seconds
         except Exception as e:
-            raise ValueError(f"audio duration calculation failed with exception {e}")
+            raise ValueError(f"audio compute duration failed with exception {e}")
 
-    try:
-        # check that local_file_path is valid
-        is_valid(local_file_path)
+    # check that local_file_path is valid
+    is_valid(local_file_path)
 
+    try:
         # compute file size
         file_size = compute_size(local_file_path)
 
         # check that file size in megabytes is greater than minimum_file_size and less than maximum_file_size
         if file_size < minimum_file_size or file_size > maximum_file_size:
             raise ValueError(
                 f"input file size is {round(file_size,2)} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
             )
 
         # compute length of audio file in seconds
         audio_duration = compute_duration(local_file_path)
 
         # check that audio file is  greater than minimum_seconds and less than maximum_seconds
-        if audio_duration < minimum_seconds or audio_duration > maximum_seconds:
-            raise ValueError(
-                f"audio file is {round(audio_duration,2)} seconds - this is either less than {minimum_seconds} seconds (current minimum size allowable) or greater than {maximum_seconds} seconds (current maximum size allowable)"
-            )
+        if audio_duration < minimum_seconds:
+            raise ValueError(f"audio file is {audio_duration} seconds - this is less than {minimum_seconds} seconds (current minimum size allowable)")
+        if audio_duration > maximum_seconds:
+            raise ValueError(f"audio file or greater than {maximum_seconds} seconds (current maximum size allowable)")
+
     except ValueError as ve:
         raise ve
     except Exception as e:
         raise ValueError(f"audio extraction failed with exception {e}")
```

### Comparing `krixik-1.1.16/krixik/utilities/validators/data/docx.py` & `krixik-1.1.17/krixik/utilities/validators/data/docx.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/data/image.py` & `krixik-1.1.17/krixik/utilities/validators/data/image.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/data/json.py` & `krixik-1.1.17/krixik/utilities/validators/data/json.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/data/npy.py` & `krixik-1.1.17/krixik/utilities/validators/data/npy.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/data/pdf.py` & `krixik-1.1.17/krixik/utilities/validators/data/pdf.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/data/pptx.py` & `krixik-1.1.17/krixik/utilities/validators/data/pptx.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/data/text.py` & `krixik-1.1.17/krixik/utilities/validators/data/text.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/data/utilities/decorators.py` & `krixik-1.1.17/krixik/utilities/validators/data/utilities/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from functools import wraps
 
 from krixik.utilities.validators.data.audio import is_size as is_audio_size
-from krixik.utilities.validators.data.video import is_size as is_video_size
+
+# from krixik.utilities.validators.data.video import is_size as is_video_size
 from krixik.utilities.validators.data.text import is_size as is_text_size
 from krixik.utilities.validators.data.pdf import is_size as is_pdf_size
 from krixik.utilities.validators.data.json import is_size as is_json_size
 from krixik.utilities.validators.data.image import is_size as is_image_size
 from krixik.utilities.validators.data.docx import is_size as is_docx_size
 from krixik.utilities.validators.data.pptx import is_size as is_pptx_size
 from krixik.utilities.validators.data.npy import is_size as is_npy_size
@@ -34,16 +35,16 @@
                     is_image_size(local_file_path=local_file_path)
                 elif extension == "docx":
                     is_docx_size(local_file_path=local_file_path)
                 elif extension == "pptx":
                     is_pptx_size(local_file_path=local_file_path)
                 elif extension == "mp3":
                     is_audio_size(local_file_path=local_file_path)
-                elif extension == "mp4":
-                    is_video_size(local_file_path=local_file_path)
+                # elif extension == "mp4":
+                #     is_video_size(local_file_path=local_file_path)
                 elif extension == "npy":
                     is_npy_size(local_file_path=local_file_path)
                 else:
                     raise ValueError(f"invalid file extension: '{extension}'")
             return func(*args, **kwargs)
         except ValueError as e:
             raise ValueError(e)
```

### Comparing `krixik-1.1.16/krixik/utilities/validators/data/utilities/read_config.py` & `krixik-1.1.17/krixik/utilities/validators/data/utilities/read_config.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/data/video.py` & `krixik-1.1.17/krixik/utilities/validators/data/audio.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,85 @@
 import os
-from moviepy.editor import VideoFileClip
-from pydub.exceptions import PydubException
-
-
-def is_valid(local_file_path: str) -> None:
-    if not os.path.exists(local_file_path):
-        raise ValueError(f"input file does not exist - {local_file_path}")
-
-    if not local_file_path.endswith(".mp4"):
-        raise ValueError(f"input file must end with .mp4 extension, not a valid video file - {local_file_path}")
-
-    try:
-        start_time = 0
-        end_time = 3
-        VideoFileClip(local_file_path).subclip(start_time, end_time)
-    except PydubException:
-        raise ValueError(f"input file is not a valid video file - {local_file_path}")
-    except FileNotFoundError:
-        raise FileNotFoundError(f"The file '{local_file_path}' does not exist.")
-    except Exception as e:
-        raise ValueError(f"video validation failed with exception {e}")
+# from pydub import AudioSegment
+# from moviepy.editor import AudioFileClip
+# from pydub.exceptions import PydubException
+
+
+# def is_valid(local_file_path: str | None) -> None:
+#     if local_file_path is None:
+#         raise ValueError("input file is None")
+
+#     # check that local_file_path represents audio file
+#     try:
+#         duration = 100
+#         AudioSegment.from_file(local_file_path, format="mp3", duration=duration)
+#     except PydubException as e:
+#         raise ValueError(f"input file is not a valid audio file - {local_file_path} - see exception {e}")
+#     except FileNotFoundError:
+#         raise FileNotFoundError(f"The file '{local_file_path}' does not exist.")
+#     except Exception as e:
+#         raise ValueError(f"Error reading audio: {e}")
+
+
+def is_valid(local_file_path: str | None) -> None:
+    if local_file_path is None:
+        raise ValueError("input local_file_path is None")
+    if not isinstance(local_file_path, str):
+        raise ValueError(f"input local_file_path is not a string: '{local_file_path}'")
+    if not local_file_path.endswith("mp3"):
+        raise ValueError(f"input local_file_path does not end with required extension 'mp3' {local_file_path}")
 
 
 def is_size(
     *,
     local_file_path: str,
     minimum_seconds: int = 1,
     maximum_seconds: int = 180,
-    minimum_file_size: float = 0.2,
-    maximum_file_size: float = 100.000001,
+    minimum_file_size: float = 0.00001,
+    maximum_file_size: float = 3.000001,
 ) -> None:
     # proper size
     def compute_size(file_path: str):
         try:
             # Get the size of the file in bytes
             file_size_bytes = os.path.getsize(file_path)
 
             # Convert the size to megabytes (MB)
             file_size_mb = file_size_bytes / (1024 * 1024)
             return file_size_mb
         except Exception as e:
-            raise ValueError(f"audio compute size failed with exception {e}")
+            raise ValueError(f"audio extraction failed with exception {e}")
 
-    def compute_duration(file_path):
-        try:
-            video_clip = VideoFileClip(file_path)
-            duration_in_seconds = round(video_clip.duration, 1)
-            return duration_in_seconds
-        except Exception as e:
-            raise ValueError(f"audio compute duration failed with exception {e}")
-
-    # check that local_file_path is valid
-    is_valid(local_file_path)
+    # def compute_duration(file_path: str) -> float:
+    #     try:
+    #         audio_clip = AudioFileClip(file_path)
+    #         duration_in_seconds = round(audio_clip.duration, 1)
+    #         audio_clip.close()
+    #         return duration_in_seconds
+    #     except Exception as e:
+    #         raise ValueError(f"audio duration calculation failed with exception {e}")
 
     try:
+        # check that local_file_path is valid
+        is_valid(local_file_path)
+
         # compute file size
         file_size = compute_size(local_file_path)
 
         # check that file size in megabytes is greater than minimum_file_size and less than maximum_file_size
         if file_size < minimum_file_size or file_size > maximum_file_size:
             raise ValueError(
                 f"input file size is {round(file_size,2)} megabytes: either less than {minimum_file_size} megabytes (current minimum size allowable) or greater than {maximum_file_size} megabytes (current maximum size allowable) - {local_file_path}"
             )
 
-        # compute length of audio file in seconds
-        audio_duration = compute_duration(local_file_path)
-
-        # check that audio file is  greater than minimum_seconds and less than maximum_seconds
-        if audio_duration < minimum_seconds:
-            raise ValueError(f"audio file is {audio_duration} seconds - this is less than {minimum_seconds} seconds (current minimum size allowable)")
-        if audio_duration > maximum_seconds:
-            raise ValueError(f"audio file or greater than {maximum_seconds} seconds (current maximum size allowable)")
+        # # compute length of audio file in seconds
+        # audio_duration = compute_duration(local_file_path)
 
+        # # check that audio file is  greater than minimum_seconds and less than maximum_seconds
+        # if audio_duration < minimum_seconds or audio_duration > maximum_seconds:
+        #     raise ValueError(
+        #         f"audio file is {round(audio_duration,2)} seconds - this is either less than {minimum_seconds} seconds (current minimum size allowable) or greater than {maximum_seconds} seconds (current maximum size allowable)"
+        #     )
     except ValueError as ve:
         raise ve
     except Exception as e:
         raise ValueError(f"audio extraction failed with exception {e}")
```

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/clean_options.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/clean_options.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/expire_time.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/expire_time.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/file_description.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/file_description.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/file_ids.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/file_ids.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/file_names.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/file_names.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/file_tags.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/file_tags.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/k_nn.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/k_nn.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/local_save_directory.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/local_save_directory.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/lower_case.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/lower_case.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/max_files.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/max_files.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/process_switches.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/process_switches.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/query.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/query.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/request_id.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/request_id.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/sort_order.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/sort_order.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/symbolic_paths.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/symbolic_paths.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/timestamp_bookends.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/timestamp_bookends.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/user_secrets.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/user_secrets.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/base/utilities/decorators.py` & `krixik-1.1.17/krixik/utilities/validators/system/base/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/audio/file_names.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/audio/file_names.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/audio/local_file_path.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/audio/local_file_path.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/audio/symbolic_file_paths.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/audio/symbolic_file_paths.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/image/file_names.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/image/file_names.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/image/local_file_path.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/image/local_file_path.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/image/symbolic_file_paths.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/image/symbolic_file_paths.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/json/file_names.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/json/file_names.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/json/local_file_path.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/json/local_file_path.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/json/symbolic_file_paths.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/json/symbolic_file_paths.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/npy/file_names.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/npy/file_names.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/npy/local_file_path.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/npy/local_file_path.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/npy/symbolic_file_paths.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/npy/symbolic_file_paths.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/text/file_names.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/text/file_names.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/text/local_file_path.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/text/local_file_path.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/text/symbolic_file_paths.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/text/symbolic_file_paths.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/system/data/utilities/decorators.py` & `krixik-1.1.17/krixik/utilities/validators/system/data/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik/utilities/validators/utilities/decorators.py` & `krixik-1.1.17/krixik/utilities/validators/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/krixik.egg-info/PKG-INFO` & `krixik-1.1.17/krixik.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krixik
-Version: 1.1.16
+Version: 1.1.17
 Summary: Easily assemble and serverlessly consume modular AI pipelines through secure Python APIs.
 Home-page: https://github.com/krixik-ai/krixik-cli
 Author: Jeremy Watt
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: linting
 Provides-Extra: testing
@@ -118,15 +118,15 @@
 ```python
 my_pipeline_1 = krixik.load_pipeline(pipeline=custom_pipeline_1)
 ```
 
 The pipeline is ready! Now you can process audio and video files through it to generate transcripts of them.
 
 ```python
-my_pipeline_1.process(local_file_path='./path/to/my/mp3/or/mp4')
+my_pipeline_1.process(local_file_path='./path/to/my/mp3')
 ```
 
 The outputs of this pipeline will be a timestamped transcript of your input audio/video file, a `file_id` for the processed file, and a `process_id` for the process itself.
 
 
 ### Extending your pipeline
```

### Comparing `krixik-1.1.16/krixik.egg-info/SOURCES.txt` & `krixik-1.1.17/krixik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `krixik-1.1.16/setup.py` & `krixik-1.1.17/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from setuptools import setup
 from setuptools import find_packages
 
 setup(
     name="krixik",
-    version="1.1.16",
+    version="1.1.17",
     description="Easily assemble and serverlessly consume modular AI pipelines through secure Python APIs.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Jeremy Watt",
     email="jeremy@krixik.com",
     url="https://github.com/krixik-ai/krixik-cli",
     packages=find_packages(include=["krixik*"]),
     package_data={"": ["*.yml", "*.yaml"]},
     include_package_data=True,
     python_requires=">=3.10",
     install_requires=[
         "boto3",
-        "ffmpeg-python",
-        "moviepy",
         "nltk",
         "numpy",
         "pillow",
         "pyaml",
-        "pydub",
         "pypdf",
         "pytest",
         "pytest-subtests",
         "python-docx",
         "python-dotenv",
         "python-pptx",
         "requests",
@@ -35,21 +32,18 @@
         "linting": [
             "ruff",
         ],
         "testing": [
             "pytest",
             "pytest-xdist",
             "boto3",
-            "ffmpeg-python",
-            "moviepy",
             "nltk",
             "numpy",
             "pillow",
             "pyaml",
-            "pydub",
             "pypdf",
             "pytest",
             "pytest-subtests",
             "python-docx",
             "python-dotenv",
             "python-pptx",
             "requests",
```

