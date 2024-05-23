# Comparing `tmp/hilda-1.4.3.tar.gz` & `tmp/hilda-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilda-1.4.3.tar", last modified: Wed May  1 06:40:09 2024, max compression
+gzip compressed data, was "hilda-2.0.0.tar", last modified: Thu May 23 11:19:32 2024, max compression
```

## Comparing `hilda-1.4.3.tar` & `hilda-2.0.0.tar`

### file list

```diff
@@ -1,89 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:40:09.979252 hilda-1.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:40:09.963252 hilda-1.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:40:09.967252 hilda-1.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-01 06:39:57.000000 hilda-1.4.3/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-01 06:39:57.000000 hilda-1.4.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-01 06:39:57.000000 hilda-1.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-01 06:39:57.000000 hilda-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22398 2024-05-01 06:40:09.979252 hilda-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19741 2024-05-01 06:39:57.000000 hilda-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:40:09.967252 hilda-1.4.3/gifs/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-01 06:39:57.000000 hilda-1.4.3/gifs/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-01 06:39:57.000000 hilda-1.4.3/gifs/ui.png
--rw-r--r--   0 runner    (1001) docker     (127)   939935 2024-05-01 06:39:57.000000 hilda-1.4.3/gifs/xpc_print_message.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:40:09.971252 hilda-1.4.3/hilda/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-01 06:40:09.000000 hilda-1.4.3/hilda/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)   120119 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/hilda_ascii_art.html
--rw-r--r--   0 runner    (1001) docker     (127)    43396 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/hilda_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/launch_lldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/lldb_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:40:09.975252 hilda-1.4.3/hilda/objective_c/
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/objective_c/from_ns_to_json.m
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/objective_c/get_objectivec_class_by_module.m
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/objective_c/get_objectivec_class_description.m
--rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/objective_c/get_objectivec_symbol_data.m
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/objective_c/lsof.m
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/objective_c/to_ns_from_json.m
--rw-r--r--   0 runner    (1001) docker     (127)    11652 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:40:09.975252 hilda-1.4.3/hilda/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/boringssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/dyld.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/fs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:40:09.975252 hilda-1.4.3/hilda/snippets/mach/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/mach/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:40:09.975252 hilda-1.4.3/hilda/snippets/macho/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/macho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/macho/all_image_infos.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/macho/apple_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/macho/image_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/macho/macho.py
--rw-r--r--   0 runner    (1001) docker     (127)    10740 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/macho/macho_load_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/remotepairingd.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/syslog.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/snippets/xpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/symbols_jar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:40:09.975252 hilda-1.4.3/hilda/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/ui/colors.json
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/ui/ui_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-05-01 06:39:57.000000 hilda-1.4.3/hilda/ui/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:40:09.979252 hilda-1.4.3/hilda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22398 2024-05-01 06:40:09.000000 hilda-1.4.3/hilda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-01 06:40:09.000000 hilda-1.4.3/hilda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:40:09.000000 hilda-1.4.3/hilda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-01 06:40:09.000000 hilda-1.4.3/hilda.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 06:40:09.000000 hilda-1.4.3/hilda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 06:40:09.000000 hilda-1.4.3/hilda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-01 06:39:57.000000 hilda-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-01 06:39:57.000000 hilda-1.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 06:40:09.979252 hilda-1.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:40:09.979252 hilda-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/hilda_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/lldb_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:40:09.979252 hilda-1.4.3/tests/test_hilda_client/
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/test_hilda_client/test_from_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/test_hilda_client/test_hilda_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/test_hilda_client/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/test_hilda_client/test_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/test_hilda_client/test_rebind_symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/test_hilda_client/test_registers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:40:09.979252 hilda-1.4.3/tests/test_snippets/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/test_snippets/test_xpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:40:09.979252 hilda-1.4.3/tests/test_symbols/
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/test_symbols/test_objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/test_symbols/test_objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/test_symbols/test_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-01 06:39:57.000000 hilda-1.4.3/tests/test_symbols/test_symbols_jar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.664590 hilda-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.644590 hilda-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.648590 hilda-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 11:19:22.000000 hilda-2.0.0/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-23 11:19:22.000000 hilda-2.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-23 11:19:22.000000 hilda-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-23 11:19:22.000000 hilda-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-23 11:19:22.000000 hilda-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23605 2024-05-23 11:19:32.664590 hilda-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20910 2024-05-23 11:19:22.000000 hilda-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.648590 hilda-2.0.0/gifs/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 11:19:22.000000 hilda-2.0.0/gifs/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 11:19:22.000000 hilda-2.0.0/gifs/ui.png
+-rw-r--r--   0 runner    (1001) docker     (127)   939935 2024-05-23 11:19:22.000000 hilda-2.0.0/gifs/xpc_print_message.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.652590 hilda-2.0.0/hilda/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 11:19:32.000000 hilda-2.0.0/hilda/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120119 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/hilda_ascii_art.html
+-rw-r--r--   0 runner    (1001) docker     (127)    43606 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/hilda_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.656590 hilda-2.0.0/hilda/ipython_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/ipython_extensions/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/ipython_extensions/keybindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/ipython_extensions/magics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/launch_lldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/lldb_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/lldb_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.656590 hilda-2.0.0/hilda/objective_c/
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c/from_ns_to_json.m
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c/get_objectivec_class_by_module.m
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c/get_objectivec_class_description.m
+-rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c/get_objectivec_symbol_data.m
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c/lsof.m
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c/to_ns_from_json.m
+-rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.656590 hilda-2.0.0/hilda/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/boringssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/dyld.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/fs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/hilda/snippets/mach/
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/mach/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/hilda/snippets/macho/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/macho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/macho/all_image_infos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/macho/apple_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/macho/image_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/macho/macho.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/macho/macho_load_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/remotepairingd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/symbols_jar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/hilda/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/ui/colors.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/ui/ui_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/ui/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/hilda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23605 2024-05-23 11:19:32.000000 hilda-2.0.0/hilda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-23 11:19:32.000000 hilda-2.0.0/hilda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:19:32.000000 hilda-2.0.0/hilda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 11:19:32.000000 hilda-2.0.0/hilda.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-23 11:19:32.000000 hilda-2.0.0/hilda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 11:19:32.000000 hilda-2.0.0/hilda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-23 11:19:22.000000 hilda-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-23 11:19:22.000000 hilda-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:19:32.664590 hilda-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/tests/test_hilda_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_hilda_client/test_from_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_hilda_client/test_hilda_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_hilda_client/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_hilda_client/test_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_hilda_client/test_rebind_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_hilda_client/test_registers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/tests/test_snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_snippets/test_xpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/tests/test_symbols/
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_symbols/test_objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_symbols/test_objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_symbols/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_symbols/test_symbols_jar.py
```

### Comparing `hilda-1.4.3/.github/workflows/python-publish.yml` & `hilda-2.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/.gitignore` & `hilda-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/LICENSE` & `hilda-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/PKG-INFO` & `hilda-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilda
-Version: 1.4.3
+Version: 2.0.0
 Summary: LLDB wrapped and empowered by iPython's features
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel cohen <netanelc305@protonmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel cohen <netanelc305@protonmail.com>
 License: Copyright (c) 2012-2023 Doron Zarhi and Metan Perelman
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
@@ -23,14 +23,15 @@
         NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
         LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
         OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
         WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://github.com/doronz88/hilda
 Project-URL: Bug Reports, https://github.com/doronz88/hilda/issues
 Keywords: python,debugger,lldb,ipython,ios,debug
+Classifier: Operating System :: MacOS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -52,26 +53,37 @@
 Requires-Dist: tabulate
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 - [Description](#description)
 - [Installation](#installation)
 - [How to use](#how-to-use)
-    * [Starting a Hilda shell](#starting-a-hilda-shell)
-        + [Bare mode](#bare-mode)
-        + [Remote mode](#remote-mode)
-    * [Usage](#usage)
-    * [Symbol objects](#symbol-objects)
-    * [Globalized symbols](#globalized-symbols)
+    - [Starting a Hilda shell](#starting-a-hilda-shell)
+        - [Attach mode](#attach-mode)
+        - [Launch mode](#launch-mode)
+        - [Bare mode](#bare-mode)
+        - [Remote mode](#remote-mode)
+            - [The connected device is connected via network](#the-connected-device-is-connected-via-network)
+        - [Startup Files](#startup-files)
+    - [Usage](#usage)
+    - [Magic functions](#magic-functions)
+    - [Shortcuts](#shortcuts)
+    - [Configurables](#configurables)
+        - [Attributes](#attributes)
+        - [Example Usage](#example-usage)
+    - [UI Configuration](#ui-configuration)
+    - [Symbol objects](#symbol-objects)
+    - [Globalized symbols](#globalized-symbols)
         - [Searching for the right symbol](#searching-for-the-right-symbol)
+        - [Objective-C Classes](#objective-c-classes)
+    - [Objective-C Objects](#objective-c-objects)
+    - [Using snippets](#using-snippets)
+- [Contributing](#contributing)
 
-        + [Objective-C Classes](#objective-c-classes)
-    * [Objective-C Objects](#objective-c-objects)
-    * [Using snippets](#using-snippets)
-    * [Contributing](#contributing)
+Would you like any further adjustments?
 
 # Description
 
 Hilda is a debugger which combines both the power of LLDB and iPython for easier debugging.
 
 The name originates from the TV show "Hilda", which is the best friend of
 [Frida](https://frida.re/). Both Frida and Hilda are meant for pretty much the same purpose, except Hilda takes the
@@ -117,15 +129,29 @@
 
 Use the attach sub-command in order to start an LLDB shell attached to given process.
 
 ```shell
 hilda attach [-p pid] [-n process-name]
 ```
 
-After attaching, simply execute `hilda` command to enter the hilda shell.
+### Launch mode
+
+Use the attach sub-command in order to launch given process.
+
+```shell
+hilda launch /path/to/executable \
+    --argv arg1 --argv arg2 \
+    --envp NAME=Alice --envp AGE=30 \
+    --stdin /path/to/input.txt \
+    --stdout /path/to/output.txt \
+    --stderr /path/to/error.txt \
+    --wd /path/to/working/directory \
+    --flags 0x01 \
+    --stop-at-entry
+  ```
 
 ### Bare mode
 
 Use "Bare mode" to get a "bare-bones" lldb shell, whereas hilda plugin is already loaded and ready to start. This mode
 is useful when you need to have custom commands for attaching to the target process (for example when debugging OSX
 processes).
 
@@ -171,14 +197,31 @@
 
 Run the following command:
 
 ```shell
 hilda remote HOSTNAME PORT
 ``` 
 
+## Startup Files
+
+Each command can accept startup files to execute on start. As opposed to snippets, the startup files can accept Hilda
+syntax.
+
+#### Startup File Example
+
+```python
+cfg.objc_verbose_monitor = True
+p.bp(ADDRESS)
+p.cont()
+```
+
+```shell
+hilda remote HOSTNAME PORT -f startupfile1 -f startupfile2
+```
+
 ## Usage
 
 Upon starting Hilda shell, you are greeted with:
 
 ```
 Hilda has been successfully loaded! 😎
 Use the p global to access all features.
@@ -321,37 +364,52 @@
 
       Feel free to use local variables inside the expression using format string.
       For example:
       currentDevice = objc_get_class('UIDevice').currentDevice
       evaluate_expression(f'[[{currentDevice} systemName] hasPrefix:@"2"]')
 - `import_module`
     - Import & reload given python module (intended mainly for external snippets)
-- `set_evaluation_unwind`
-    - Set whether LLDB will attempt to unwind the stack whenever an expression evaluation error occurs.
-      Use unwind() to restore when an error is raised in this case.
-- `get_evaluation_unwind`
-    - Get evaluation unwind state.
-      When this value is True, LLDB will attempt unwinding the stack on evaluation errors.
-      Otherwise, the stack frame will remain the same on errors to help you investigate the error.
-- `set_evaluation_ignore_breakpoints`
-    - Set whether to ignore breakpoints while evaluating expressions
-- `get_evaluation_ignore_breakpoints`
-    - Get evaluation "ignore-breakpoints" state.
 - `unwind`
     - Unwind the stack (useful when get_evaluation_unwind() == False)
 
 ## Magic functions
 
 Sometimes accessing the python API can be tiring, so we added some magic functions to help you out!
 
 - `%objc <className>`
     - Equivalent to: `className = p.objc_get_class(className)`
 - `%fbp <filename> <addressInHex>`
     - Equivalent to: `p.file_symbol(addressInHex, filename).bp()`
 
+## Shortcuts
+
+- **F7**: Step Into
+- **F8**: Step Over
+- **F9**: Continue
+- **F10**: Stop
+
+## Configurables
+
+The global `cfg` used to configure various settings for evaluation and monitoring.
+
+### Attributes
+
+- `evaluation_unwind_on_error`: Whether to unwind on error during evaluation. (Default: `False`)
+- `evaluation_ignore_breakpoints`: Whether to ignore breakpoints during evaluation. (Default: `False`)
+- `nsobject_exclusion`: Whether to exclude `NSObject` during evaluation, reducing IPython autocomplete results. (
+  Default: `False`)
+- `objc_verbose_monitor`: When set to `True`, using `monitor()` will automatically print Objective-C method arguments. (
+  Default: `False`)
+
+### Example Usage
+
+```python
+cfg.objc_verbose_monitor = True
+```
+
 ## UI Configuration
 
 Hilda contains minimal UI for examining the target state.
 The UI is divided into views:
 
 - Registers
 - Disassembly
@@ -701,13 +759,9 @@
 This will monitor all XPC related traffic in the given process.
 
 ## Contributing
 
 Please run the tests as follows before submitting a PR:
 
 ```shell
-xcrun python3 -m tests aggregated
-
-# wait for lldb shell prompt
-
-run_tests
+xcrun python3 -m pytest
 ```
```

### Comparing `hilda-1.4.3/README.md` & `hilda-2.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 - [Description](#description)
 - [Installation](#installation)
 - [How to use](#how-to-use)
-    * [Starting a Hilda shell](#starting-a-hilda-shell)
-        + [Bare mode](#bare-mode)
-        + [Remote mode](#remote-mode)
-    * [Usage](#usage)
-    * [Symbol objects](#symbol-objects)
-    * [Globalized symbols](#globalized-symbols)
+    - [Starting a Hilda shell](#starting-a-hilda-shell)
+        - [Attach mode](#attach-mode)
+        - [Launch mode](#launch-mode)
+        - [Bare mode](#bare-mode)
+        - [Remote mode](#remote-mode)
+            - [The connected device is connected via network](#the-connected-device-is-connected-via-network)
+        - [Startup Files](#startup-files)
+    - [Usage](#usage)
+    - [Magic functions](#magic-functions)
+    - [Shortcuts](#shortcuts)
+    - [Configurables](#configurables)
+        - [Attributes](#attributes)
+        - [Example Usage](#example-usage)
+    - [UI Configuration](#ui-configuration)
+    - [Symbol objects](#symbol-objects)
+    - [Globalized symbols](#globalized-symbols)
         - [Searching for the right symbol](#searching-for-the-right-symbol)
+        - [Objective-C Classes](#objective-c-classes)
+    - [Objective-C Objects](#objective-c-objects)
+    - [Using snippets](#using-snippets)
+- [Contributing](#contributing)
 
-        + [Objective-C Classes](#objective-c-classes)
-    * [Objective-C Objects](#objective-c-objects)
-    * [Using snippets](#using-snippets)
-    * [Contributing](#contributing)
+Would you like any further adjustments?
 
 # Description
 
 Hilda is a debugger which combines both the power of LLDB and iPython for easier debugging.
 
 The name originates from the TV show "Hilda", which is the best friend of
 [Frida](https://frida.re/). Both Frida and Hilda are meant for pretty much the same purpose, except Hilda takes the
@@ -62,15 +73,29 @@
 
 Use the attach sub-command in order to start an LLDB shell attached to given process.
 
 ```shell
 hilda attach [-p pid] [-n process-name]
 ```
 
-After attaching, simply execute `hilda` command to enter the hilda shell.
+### Launch mode
+
+Use the attach sub-command in order to launch given process.
+
+```shell
+hilda launch /path/to/executable \
+    --argv arg1 --argv arg2 \
+    --envp NAME=Alice --envp AGE=30 \
+    --stdin /path/to/input.txt \
+    --stdout /path/to/output.txt \
+    --stderr /path/to/error.txt \
+    --wd /path/to/working/directory \
+    --flags 0x01 \
+    --stop-at-entry
+  ```
 
 ### Bare mode
 
 Use "Bare mode" to get a "bare-bones" lldb shell, whereas hilda plugin is already loaded and ready to start. This mode
 is useful when you need to have custom commands for attaching to the target process (for example when debugging OSX
 processes).
 
@@ -116,14 +141,31 @@
 
 Run the following command:
 
 ```shell
 hilda remote HOSTNAME PORT
 ``` 
 
+## Startup Files
+
+Each command can accept startup files to execute on start. As opposed to snippets, the startup files can accept Hilda
+syntax.
+
+#### Startup File Example
+
+```python
+cfg.objc_verbose_monitor = True
+p.bp(ADDRESS)
+p.cont()
+```
+
+```shell
+hilda remote HOSTNAME PORT -f startupfile1 -f startupfile2
+```
+
 ## Usage
 
 Upon starting Hilda shell, you are greeted with:
 
 ```
 Hilda has been successfully loaded! 😎
 Use the p global to access all features.
@@ -266,37 +308,52 @@
 
       Feel free to use local variables inside the expression using format string.
       For example:
       currentDevice = objc_get_class('UIDevice').currentDevice
       evaluate_expression(f'[[{currentDevice} systemName] hasPrefix:@"2"]')
 - `import_module`
     - Import & reload given python module (intended mainly for external snippets)
-- `set_evaluation_unwind`
-    - Set whether LLDB will attempt to unwind the stack whenever an expression evaluation error occurs.
-      Use unwind() to restore when an error is raised in this case.
-- `get_evaluation_unwind`
-    - Get evaluation unwind state.
-      When this value is True, LLDB will attempt unwinding the stack on evaluation errors.
-      Otherwise, the stack frame will remain the same on errors to help you investigate the error.
-- `set_evaluation_ignore_breakpoints`
-    - Set whether to ignore breakpoints while evaluating expressions
-- `get_evaluation_ignore_breakpoints`
-    - Get evaluation "ignore-breakpoints" state.
 - `unwind`
     - Unwind the stack (useful when get_evaluation_unwind() == False)
 
 ## Magic functions
 
 Sometimes accessing the python API can be tiring, so we added some magic functions to help you out!
 
 - `%objc <className>`
     - Equivalent to: `className = p.objc_get_class(className)`
 - `%fbp <filename> <addressInHex>`
     - Equivalent to: `p.file_symbol(addressInHex, filename).bp()`
 
+## Shortcuts
+
+- **F7**: Step Into
+- **F8**: Step Over
+- **F9**: Continue
+- **F10**: Stop
+
+## Configurables
+
+The global `cfg` used to configure various settings for evaluation and monitoring.
+
+### Attributes
+
+- `evaluation_unwind_on_error`: Whether to unwind on error during evaluation. (Default: `False`)
+- `evaluation_ignore_breakpoints`: Whether to ignore breakpoints during evaluation. (Default: `False`)
+- `nsobject_exclusion`: Whether to exclude `NSObject` during evaluation, reducing IPython autocomplete results. (
+  Default: `False`)
+- `objc_verbose_monitor`: When set to `True`, using `monitor()` will automatically print Objective-C method arguments. (
+  Default: `False`)
+
+### Example Usage
+
+```python
+cfg.objc_verbose_monitor = True
+```
+
 ## UI Configuration
 
 Hilda contains minimal UI for examining the target state.
 The UI is divided into views:
 
 - Registers
 - Disassembly
@@ -646,13 +703,9 @@
 This will monitor all XPC related traffic in the given process.
 
 ## Contributing
 
 Please run the tests as follows before submitting a PR:
 
 ```shell
-xcrun python3 -m tests aggregated
-
-# wait for lldb shell prompt
-
-run_tests
+xcrun python3 -m pytest
 ```
```

### Comparing `hilda-1.4.3/gifs/xpc_print_message.gif` & `hilda-2.0.0/gifs/xpc_print_message.gif`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/hilda/exceptions.py` & `hilda-2.0.0/hilda/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 __all__ = ['HildaException', 'SymbolAbsentError', 'EvaluatingExpressionError', 'CreatingObjectiveCSymbolError',
            'ConvertingToNsObjectError', 'ConvertingFromNSObjectError', 'DisableJetsamMemoryChecksError',
            'GettingObjectiveCClassError', 'AccessingRegisterError', 'AccessingMemoryError',
-           'BrokenLocalSymbolsJarError', 'AddingLldbSymbolError']
+           'BrokenLocalSymbolsJarError', 'AddingLldbSymbolError', 'LLDBException']
 
 
 class HildaException(Exception):
     """ A domain exception for hilda errors. """
     pass
 
 
+class LLDBException(Exception):
+    """ A domain exception for lldb errors. """
+
+    def __init__(self, message: str):
+        super().__init__()
+        self.message = message
+
+
 class SymbolAbsentError(HildaException):
     """ Raise when trying to get a symbol that doesn't exist. """
     pass
 
 
 class EvaluatingExpressionError(HildaException):
     """ Raise when failing to evaluate an expression. """
```

### Comparing `hilda-1.4.3/hilda/hilda_ascii_art.html` & `hilda-2.0.0/hilda/hilda_ascii_art.html`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/hilda/hilda_client.py` & `hilda-2.0.0/hilda/hilda_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,100 +1,129 @@
-import ast
 import base64
 import builtins
 import importlib
 import importlib.util
 import json
 import logging
 import os
 import pickle
 import struct
+import sys
 import time
 import typing
 from collections import namedtuple
 from contextlib import contextmanager, suppress
+from dataclasses import dataclass, field
 from datetime import datetime, timezone
-from functools import cached_property
+from functools import cached_property, wraps
 from pathlib import Path
 from typing import Any, Callable, List, Optional, Union
 
 import hexdump
 import IPython
-import lldb
 from humanfriendly import prompts
 from humanfriendly.terminal.html import html_to_ansi
 from IPython.core.magic import register_line_magic  # noqa: F401
 from pygments import highlight
 from pygments.formatters import TerminalTrueColorFormatter
 from pygments.lexers import XmlLexer
 from tqdm import tqdm
 from traitlets.config import Config
 
 from hilda import objective_c_class
 from hilda.common import CfSerializable
 from hilda.exceptions import AccessingMemoryError, AccessingRegisterError, AddingLldbSymbolError, \
     BrokenLocalSymbolsJarError, ConvertingFromNSObjectError, ConvertingToNsObjectError, CreatingObjectiveCSymbolError, \
     DisableJetsamMemoryChecksError, EvaluatingExpressionError, HildaException, SymbolAbsentError
-from hilda.launch_lldb import disable_logs  # noqa: F401
+from hilda.lldb_importer import lldb
 from hilda.objective_c_symbol import ObjectiveCSymbol
 from hilda.registers import Registers
 from hilda.snippets.mach import CFRunLoopServiceMachPort_hooks
 from hilda.symbol import Symbol
 from hilda.symbols_jar import SymbolsJar
 from hilda.ui.ui_manager import UiManager
 
 lldb.KEYSTONE_SUPPORT = True
 try:
     from keystone import KS_ARCH_ARM64, KS_ARCH_X86, KS_MODE_64, KS_MODE_LITTLE_ENDIAN, Ks
 except ImportError:
     lldb.KEYSTONE_SUPPORT = False
     print('failed to import keystone. disabling some features')
 
-with open(os.path.join(Path(__file__).resolve().parent, 'hilda_ascii_art.html'), 'r') as f:
-    hilda_art = f.read()
+hilda_art = Path(__file__).resolve().parent.joinpath('hilda_ascii_art.html').read_text()
 
 GREETING = f"""
 {hilda_art}
 
 <b>Hilda has been successfully loaded! 😎
-Use the <span style="color: magenta">p</span> global to access all features.
+Usage:
+ <span style="color: magenta">p</span>   Global to access all features.
+ <span style="color: magenta">F7</span>  Step Into.
+ <span style="color: magenta">F8</span>  Step Over.
+ <span style="color: magenta">F9</span>  Continue.
+ <span style="color: magenta">F10</span> Stop.
+
 Have a nice flight ✈️! Starting an IPython shell...
 """
 
-MAGIC_FUNCTIONS = """
-import shlex
-from IPython.core.magic import register_line_magic, needs_local_scope
-
-@register_line_magic
-@needs_local_scope
-def objc(line, local_ns=None):
-    p = local_ns['p']
-    className = line.strip()
-    if not className:
-        p.log_error("Error: className is required.")
-        return
-    try:
-        local_ns[className] = p.objc_get_class(className)
-        p.log_info(f'{className} class loaded successfully')
-    except Exception:
-        p.log_error(f'Error loading class {className}')
-
-
-@register_line_magic
-@needs_local_scope
-def fbp(line, local_ns=None):
-    p = local_ns['p']
-    module_name, address = shlex.split(line.strip())
-    address = int(address, 16)
-    p.file_symbol(address, module_name).bp()
-"""
+
+def disable_logs() -> None:
+    logging.getLogger('asyncio').disabled = True
+    logging.getLogger('parso.cache').disabled = True
+    logging.getLogger('parso.cache.pickle').disabled = True
+    logging.getLogger('parso.python.diff').disabled = True
+    logging.getLogger('humanfriendly.prompts').disabled = True
+    logging.getLogger('blib2to3.pgen2.driver').disabled = True
+    logging.getLogger('hilda.launch_lldb').disabled = True
+
 
 SerializableSymbol = namedtuple('SerializableSymbol', 'address type_ filename')
 
 
+@dataclass
+class Configs:
+    """ Configuration settings for evaluation and monitoring. """
+    evaluation_unwind_on_error: bool = field(default=False,
+                                             metadata={'doc': 'Whether to unwind on error during evaluation.'})
+    evaluation_ignore_breakpoints: bool = field(default=False,
+                                                metadata={'doc': 'Whether to ignore breakpoints during evaluation.'})
+    nsobject_exclusion: bool = field(default=False, metadata={
+        'doc': 'Whether to exclude NSObject during evaluation - reduce ipython autocomplete results.'})
+    objc_verbose_monitor: bool = field(default=False, metadata={
+        'doc': 'When set to True, using monitor() will automatically print objc methods arguments.'})
+
+    def __repr__(self):
+        return self.__str__()
+
+    def __str__(self):
+        config_str = 'Configuration settings:\n'
+        max_len = max(len(field_name) for field_name in self.__dataclass_fields__) + 2
+
+        for field_name, field_info in self.__dataclass_fields__.items():
+            value = getattr(self, field_name)
+            doc = field_info.metadata.get('doc', 'No docstring available')
+            config_str += f'\t{field_name.ljust(max_len)}: {str(value).ljust(5)} | {doc}\n'
+
+        return config_str
+
+
+def stop_is_needed(func: Callable):
+    """Decorator to check if the process must be stopped before proceeding."""
+
+    @wraps(func)
+    def wrapper(self, *args, **kwargs):
+        is_running = self.process.GetState() == lldb.eStateRunning
+        if is_running:
+            self.logger.error(f'Cannot {func.__name__.replace("_", "-")}: Process must be stopped first.')
+            return
+        return func(self, *args, **kwargs)
+
+    return wrapper
+
+
 class HildaClient:
     Breakpoint = namedtuple('Breakpoint', 'address options forced callback')
 
     RETVAL_BIT_COUNT = 64
 
     def __init__(self, debugger: lldb.SBDebugger):
         self.logger = logging.getLogger(__name__)
@@ -104,21 +133,15 @@
         self.process = self.target.GetProcess()
         self.symbols = SymbolsJar.create(self)
         self.breakpoints = {}
         self.captured_objects = {}
         self.registers = Registers(self)
         self.arch = self.target.GetTriple().split('-')[0]
         self.ui_manager = UiManager(self)
-        # should unwind the stack on errors. change this to False in order to debug self-made calls
-        # within hilda
-        self._evaluation_unwind_on_error = True
-
-        # should ignore breakpoints while evaluation
-        self._evaluation_ignore_breakpoints = True
-
+        self.configs = Configs()
         self._dynamic_env_loaded = False
         self._symbols_loaded = False
 
         # the frame called within the context of the hit BP
         self._bp_frame = None
 
         self._add_global('symbols', self.symbols, [])
@@ -140,15 +163,15 @@
         :return: Mapping between open FDs and their paths
         """
         data = (Path(__file__).parent / 'objective_c' / 'lsof.m').read_text()
         result = json.loads(self.po(data))
         # convert FDs into int
         return {int(k): v for k, v in result.items()}
 
-    def bt(self, should_print=True, depth: Optional[int] = None) -> List:
+    def bt(self, should_print: bool = False, depth: Optional[int] = None) -> List[Union[str, lldb.SBFrame]]:
         """ Print an improved backtrace. """
         backtrace = []
         for i, frame in enumerate(self.thread.frames):
             if i == depth:
                 break
             row = ''
             row += html_to_ansi(f'<span style="color: cyan">0x{frame.addr.GetFileAddress():x}</span> ')
@@ -247,39 +270,42 @@
             for symbol in module:
                 with suppress(AddingLldbSymbolError):
                     self.add_lldb_symbol(symbol)
 
         globals()['symbols'] = self.symbols
         self._symbols_loaded = True
 
+    @stop_is_needed
     def poke(self, address, buf: bytes):
         """
         Write data at given address
         :param address:
         :param buf:
         """
         err = lldb.SBError()
         retval = self.process.WriteMemory(address, buf, err)
 
         if not err.Success():
             raise AccessingMemoryError()
 
         return retval
 
+    @stop_is_needed
     def poke_text(self, address: int, code: str) -> int:
         """
         Write instructions to address.
         :param address:
         :param code:
         """
         if not lldb.KEYSTONE_SUPPORT:
             raise NotImplementedError('Not supported without keystone')
         bytecode, count = self._ks.asm(code, as_bytes=True)
         return self.poke(address, bytecode)
 
+    @stop_is_needed
     def peek(self, address, size: int) -> bytes:
         """
         Read data at given address
         :param address:
         :param size:
         :return:
         """
@@ -290,60 +316,69 @@
         retval = self.process.ReadMemory(address, int(size), err)
 
         if not err.Success():
             raise AccessingMemoryError()
 
         return retval
 
+    @stop_is_needed
     def peek_str(self, address: Symbol) -> str:
         """
         Peek a buffer till null termination
         :param address:
         :return:
         """
         return address.po('char *')[1:-1]  # strip the ""
 
-    def stop(self):
+    def stop(self, *args) -> None:
         """ Stop process. """
         self.debugger.SetAsync(False)
 
         is_running = self.process.GetState() == lldb.eStateRunning
         if not is_running:
             self.log_debug('already stopped')
             return
 
         if not self.process.Stop().Success():
             self.log_critical('failed to stop process')
+        else:
+            self.log_info('Process Stopped')
 
-    def cont(self):
+    def cont(self, *args) -> None:
         """ Continue process. """
         is_running = self.process.GetState() == lldb.eStateRunning
 
         if is_running:
             self.log_debug('already running')
             return
 
         # bugfix:   the debugger may become in sync state, so we make sure
         #           it isn't before trying to continue
         self.debugger.SetAsync(True)
 
         if not self.process.Continue().Success():
             self.log_critical('failed to continue process')
+        else:
+            self.log_info('Process Continued')
 
     def detach(self):
         """
         Detach from process.
 
         Useful in order to exit gracefully so process doesn't get killed
         while you exit
         """
         if not self.process.Detach().Success():
             self.log_critical('failed to detach')
+        else:
+            self.log_info('Process Detached')
 
-    def disass(self, address, buf, flavor='intel', should_print=True) -> lldb.SBInstructionList:
+    @stop_is_needed
+    def disass(self, address: int, buf: bytes, flavor: str = 'intel',
+               should_print: bool = False) -> lldb.SBInstructionList:
         """
         Print disassembly from a given address
         :param flavor:
         :param address:
         :param buf:
         :param should_print:
         :return:
@@ -524,22 +559,24 @@
 
     def finish(self):
         """ Run current frame till its end. """
         with self.sync_mode():
             self.thread.StepOutOfFrame(self.frame)
             self._bp_frame = None
 
-    def step_into(self):
+    @stop_is_needed
+    def step_into(self, *args):
         """ Step into current instruction. """
         with self.sync_mode():
             self.thread.StepInto()
         if self.ui_manager.active:
             self.ui_manager.show()
 
-    def step_over(self):
+    @stop_is_needed
+    def step_over(self, *args):
         """ Step over current instruction. """
         with self.sync_mode():
             self.thread.StepOver()
         if self.ui_manager.active:
             self.ui_manager.show()
 
     def remove_all_hilda_breakpoints(self, remove_forced=False):
@@ -817,17 +854,17 @@
         # prepending a prefix so LLDB knows to return an int type
         if isinstance(expression, int):
             formatted_expression = f'(intptr_t)0x{expression:x}'
         else:
             formatted_expression = str(expression)
 
         options = lldb.SBExpressionOptions()
-        options.SetIgnoreBreakpoints(self._evaluation_ignore_breakpoints)
+        options.SetIgnoreBreakpoints(self.configs.evaluation_ignore_breakpoints)
         options.SetTryAllThreads(True)
-        options.SetUnwindOnError(self._evaluation_unwind_on_error)
+        options.SetUnwindOnError(self.configs.evaluation_unwind_on_error)
 
         e = self.frame.EvaluateExpression(formatted_expression, options)
 
         if not e.error.Success():
             raise EvaluatingExpressionError(str(e.error))
 
         return self.symbol(e.unsigned)
@@ -843,43 +880,14 @@
         if name is None:
             name = os.path.splitext(os.path.basename(filename))[0]
         spec = importlib.util.spec_from_file_location(name, filename)
         m = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(m)
         return m
 
-    def set_evaluation_unwind(self, value: bool):
-        """
-        Set whether LLDB will attempt to unwind the stack whenever an expression evaluation error occurs.
-
-        Use unwind() to restore when an error is raised in this case.
-        """
-        self._evaluation_unwind_on_error = value
-
-    def get_evaluation_unwind(self) -> bool:
-        """
-        Get evaluation unwind state.
-
-        When this value is True, LLDB will attempt unwinding the stack on evaluation errors.
-        Otherwise, the stack frame will remain the same on errors to help you investigate the error.
-        """
-        return self._evaluation_unwind_on_error
-
-    def set_evaluation_ignore_breakpoints(self, value: bool):
-        """
-        Set whether to ignore breakpoints while evaluating expressions
-        """
-        self._evaluation_ignore_breakpoints = value
-
-    def get_evaluation_ignore_breakpoints(self) -> bool:
-        """
-        Get evaluation "ignore-breakpoints" state.
-        """
-        return self._evaluation_ignore_breakpoints
-
     def unwind(self) -> bool:
         """ Unwind the stack (useful when get_evaluation_unwind() == False) """
         return self.thread.UnwindInnermostExpression().Success()
 
     @cached_property
     def pid(self) -> int:
         return self.process.GetProcessID()
@@ -1012,36 +1020,40 @@
 
         # add it into symbols global
         self.symbols[name] = value
         self.symbols[f'{name}{{{value.filename}}}'] = value
 
         return value
 
-    def interact(self, additional_namespace: typing.Mapping = None) -> None:
+    def interact(self, additional_namespace: Optional[typing.Mapping] = None,
+                 startup_files: Optional[List[str]] = None) -> None:
         """ Start an interactive Hilda shell """
         if not self._dynamic_env_loaded:
             self.init_dynamic_environment()
         print('\n')
         self.log_info(html_to_ansi(GREETING))
+        ipython_config = Config()
+        ipython_config.IPCompleter.use_jedi = True
+        ipython_config.BaseIPythonApplication.profile = 'hilda'
+        ipython_config.InteractiveShellApp.extensions = ['hilda.ipython_extensions.magics',
+                                                         'hilda.ipython_extensions.events',
+                                                         'hilda.ipython_extensions.keybindings']
+        ipython_config.InteractiveShellApp.exec_lines = ["disable_logs()"]
+        if startup_files is not None:
+            ipython_config.InteractiveShellApp.exec_files = startup_files
+            self.log_debug(f'Startup files - {startup_files}')
 
-        config = Config()
-        config.IPCompleter.use_jedi = True
-        config.InteractiveShellApp.exec_lines = [
-            """disable_logs()""",
-            """IPython.get_ipython().events.register('pre_run_cell', self._ipython_run_cell_hook)""",
-            MAGIC_FUNCTIONS,
-        ]
-        config.BaseIPythonApplication.profile = 'hilda'
         namespace = globals()
         namespace.update(locals())
         namespace['p'] = self
         if additional_namespace is not None:
             namespace.update(additional_namespace)
-
-        IPython.start_ipython(config=config, user_ns=namespace)
+        sys.argv = ['a']
+        IPython.start_ipython(config=ipython_config, user_ns=namespace)
+        self.detach()
 
     @staticmethod
     def _add_global(name: str, value: Any, reserved_names=None):
         if reserved_names is None or name not in reserved_names:
             # don't override existing symbols
             globals()[name] = value
 
@@ -1104,43 +1116,14 @@
         args_conv = ','.join(params)
 
         if self.arch == 'arm64e':
             address = f'ptrauth_sign_unauthenticated((void *){address}, ptrauth_key_asia, 0)'
 
         return f'((intptr_t(*)({args_type}))({address}))({args_conv})'
 
-    def _ipython_run_cell_hook(self, info):
-        """
-        Enable lazy loading for symbols
-        :param info: IPython's CellInfo object
-        """
-        if info.raw_cell[0] in ['!', '%'] or info.raw_cell.endswith('?'):
-            return
-
-        for node in ast.walk(ast.parse(info.raw_cell)):
-            if not isinstance(node, ast.Name):
-                # we are only interested in names
-                continue
-
-            if node.id in locals() or node.id in globals() or node.id in dir(builtins):
-                # That are undefined
-                continue
-
-            if not hasattr(SymbolsJar, node.id):
-                # ignore SymbolsJar properties
-                try:
-                    symbol = getattr(self.symbols, node.id)
-                except SymbolAbsentError:
-                    pass
-                else:
-                    self._add_global(
-                        node.id,
-                        symbol if symbol.type_ != lldb.eSymbolTypeObjCMetaClass else self.objc_get_class(node.id)
-                    )
-
     @staticmethod
     def _std_string(value):
         if struct.unpack("b", (value + 23).peek(1))[0] >= 0:
             return value.peek_str()
         else:
             return value[0].peek_str()
```

### Comparing `hilda-1.4.3/hilda/lldb_entrypoint.py` & `hilda-2.0.0/hilda/lldb_entrypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import logging
 
 import coloredlogs
 import lldb
 
 from hilda.hilda_client import HildaClient
 
-coloredlogs.install(level=logging.DEBUG)
-
 lldb.hilda_client = None
 
 
 def hilda(debugger, command, result, internal_dict):
+    coloredlogs.install(level=logging.DEBUG)
+
     if lldb.hilda_client is None:
         lldb.hilda_client = HildaClient(debugger)
 
     additional_namespace = {'ui': lldb.hilda_client.ui_manager}
     lldb.hilda_client.interact(additional_namespace=additional_namespace)
```

### Comparing `hilda-1.4.3/hilda/objective_c/from_ns_to_json.m` & `hilda-2.0.0/hilda/objective_c/from_ns_to_json.m`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/hilda/objective_c/get_objectivec_class_by_module.m` & `hilda-2.0.0/hilda/objective_c/get_objectivec_class_by_module.m`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/hilda/objective_c/get_objectivec_class_description.m` & `hilda-2.0.0/hilda/objective_c/get_objectivec_class_description.m`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/hilda/objective_c/get_objectivec_symbol_data.m` & `hilda-2.0.0/hilda/objective_c/get_objectivec_symbol_data.m`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/hilda/objective_c/lsof.m` & `hilda-2.0.0/hilda/objective_c/lsof.m`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/hilda/objective_c/to_ns_from_json.m` & `hilda-2.0.0/hilda/objective_c/to_ns_from_json.m`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/hilda/objective_c_class.py` & `hilda-2.0.0/hilda/objective_c_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,16 @@
         result = set()
 
         for method in self.methods:
             if method.is_class:
                 result.add(method.name.replace(':', '_'))
 
         for sup in self.iter_supers():
+            if self._client.configs.nsobject_exclusion and sup.name == 'NSObject':
+                continue
             for method in sup.methods:
                 if method.is_class:
                     result.add(method.name.replace(':', '_'))
 
         result.update(list(super(Class, self).__dir__()))
         return list(result)
```

### Comparing `hilda-1.4.3/hilda/objective_c_symbol.py` & `hilda-2.0.0/hilda/objective_c_symbol.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,16 @@
         for ivar in self.ivars:
             result.add(ivar.name)
 
         for method in self.methods:
             result.add(method.name.replace(':', '_'))
 
         for sup in self.class_.iter_supers():
+            if self._client.configs.nsobject_exclusion and sup.name == 'NSObject':
+                continue
             for method in sup.methods:
                 result.add(method.name.replace(':', '_'))
 
         result.update(list(super(ObjectiveCSymbol, self).__dir__()))
         return list(result)
 
     def __getitem__(self, item):
```

### Comparing `hilda-1.4.3/hilda/registers.py` & `hilda-2.0.0/hilda/registers.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/hilda/snippets/boringssl.py` & `hilda-2.0.0/hilda/snippets/boringssl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import lldb
+from hilda.lldb_importer import lldb
 
 _FILENAME = '/tmp/hilda-keylog.txt'
 
 
 def _ssl_log_secret_bp(hilda, *args):
     label = hilda.registers.x1.peek_str()
     secret = hilda.registers.x2.peek(hilda.registers.x3).hex()
```

### Comparing `hilda-1.4.3/hilda/snippets/dyld.py` & `hilda-2.0.0/hilda/snippets/dyld.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import lldb
 from cached_property import cached_property
 
+from hilda.lldb_importer import lldb
 from hilda.snippets.macho.all_image_infos import AllImageInfos
 from hilda.snippets.syslog import open_syslog_socket
 
 
 def all_image_infos():
     return AllImageInfos()
```

### Comparing `hilda-1.4.3/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py` & `hilda-2.0.0/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import lldb
-
 from hilda.exceptions import SymbolAbsentError
+from hilda.lldb_importer import lldb
 
 
 def _CFRunLoopServiceMachPort_hook(hilda, *args):
     """
     :param hilda.hilda_client.HildaClient hilda:
      """
     hilda.jump(hilda.CFRunLoopServiceMachPort_while_ea)
```

### Comparing `hilda-1.4.3/hilda/snippets/macho/all_image_infos.py` & `hilda-2.0.0/hilda/snippets/macho/all_image_infos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
-import lldb
 from construct import Array, CString, Hex, If, Int32ub, Int32ul, Int64ul, Pointer, Struct, Tell, this
 from humanfriendly import prompts
 
+from hilda.lldb_importer import lldb
 from hilda.snippets.macho.image_info import ImageInfo, dyld_image_info_t
 from hilda.snippets.macho.macho import mach_header_t
 from hilda.snippets.uuid import uuid_t
 from hilda.symbol import SymbolFormatField
 
 all_image_infos_t = Struct(
     'address' / Tell,
```

### Comparing `hilda-1.4.3/hilda/snippets/macho/image_info.py` & `hilda-2.0.0/hilda/snippets/macho/image_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import lldb
 from construct import CString, If, Int64ul, Pointer, Struct, this
 
+from hilda.lldb_importer import lldb
 from hilda.snippets.macho.macho import mach_header_t
 from hilda.snippets.macho.macho_load_commands import LoadCommands
 from hilda.snippets.uuid import uuid_t
 from hilda.symbol import SymbolFormatField
 
 dyld_image_info_t = Struct(
     '_imageLoadAddress' / SymbolFormatField(lldb.hilda_client),
```

### Comparing `hilda-1.4.3/hilda/snippets/macho/macho.py` & `hilda-2.0.0/hilda/snippets/macho/macho.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/hilda/snippets/macho/macho_load_commands.py` & `hilda-2.0.0/hilda/snippets/macho/macho_load_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
-import lldb
 from construct import Array, Bytes, Enum, Hex, Int8ul, Int32ul, Int64ul, PaddedString, Pointer, Seek, Struct, Switch, \
     Tell, this
 
+from hilda.lldb_importer import lldb
 from hilda.snippets.macho.apple_version import version_t
 from hilda.symbol import SymbolFormatField
 
 # See: https://opensource.apple.com/source/xnu/xnu-7195.81.3/EXTERNAL_HEADERS/mach-o/loader.h
 LC_REQ_DYLD = 0x80000000
 
 LOAD_COMMAND_TYPE = Enum(Int32ul,
```

### Comparing `hilda-1.4.3/hilda/snippets/remotepairingd.py` & `hilda-2.0.0/hilda/snippets/remotepairingd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import lldb
+from hilda.lldb_importer import lldb
 
 TLV_MAP = {
     0x00: 'METHOD',
     0x01: 'IDENTIFIER',
     0x02: 'SALT',
     0x03: 'PUBLIC_KEY',
     0x04: 'PROOF',
```

### Comparing `hilda-1.4.3/hilda/snippets/xpc.py` & `hilda-2.0.0/hilda/snippets/xpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pprint import pformat
 
-import lldb
 from pygments import highlight
 from pygments.formatters import TerminalTrueColorFormatter
 from pygments.lexers import PythonLexer
 
 from hilda.exceptions import ConvertingFromNSObjectError
+from hilda.lldb_importer import lldb
 
 # module global for storing all active xpc connections
 active_xpc_connections = {}
 
 
 def safe_monitor(symbol_name, **kwargs):
     hilda = lldb.hilda_client
```

### Comparing `hilda-1.4.3/hilda/symbol.py` & `hilda-2.0.0/hilda/symbol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import struct
 from contextlib import contextmanager
 from typing import Any, Optional
 
-import lldb
 from construct import FormatField
 
 from hilda.common import CfSerializable
+from hilda.lldb_importer import lldb
 from hilda.objective_c_class import Class
 
 ADDRESS_SIZE_TO_STRUCT_FORMAT = {1: 'B', 2: 'H', 4: 'I', 8: 'Q'}
 
 
 class SymbolFormatField(FormatField):
     """
```

### Comparing `hilda-1.4.3/hilda/symbols_jar.py` & `hilda-2.0.0/hilda/symbols_jar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from contextlib import suppress
 
-import lldb
-
 from hilda.exceptions import AddingLldbSymbolError, SymbolAbsentError
+from hilda.lldb_importer import lldb
 
 
 class SymbolsJar(dict):
     @staticmethod
     def create(client):
         """
         Factory method for creating symbols jars
@@ -136,18 +135,23 @@
     def monitor(self, **args):
         """
         Perform monitor for all symbols in current jar.
         See monitor command for more details.
         :param args: given arguments for monitor command
         """
         for name, address in self.items():
+            args_c = args.copy()
             if name == '_client':
                 continue
-            name = args.get('name', name)
-            address.monitor(name=name, **args)
+            if self.__dict__['_client'].configs.objc_verbose_monitor:
+                arg_count = name.count(':')
+                if arg_count > 0:
+                    args_c['regs'] = {f'x{i + 2}': 'po' for i in range(arg_count)}
+            name = args_c.get('name', name)
+            address.monitor(name=name, **args_c)
 
     def startswith(self, exp, case_sensitive=True):
         """
         Filter only symbols with given prefix
         :param exp: prefix
         :param case_sensitive: is case sensitive
         :return: reduced symbol jar
```

### Comparing `hilda-1.4.3/hilda/ui/ui_manager.py` & `hilda-2.0.0/hilda/ui/ui_manager.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/hilda/ui/views.py` & `hilda-2.0.0/hilda/ui/views.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/hilda.egg-info/PKG-INFO` & `hilda-2.0.0/hilda.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilda
-Version: 1.4.3
+Version: 2.0.0
 Summary: LLDB wrapped and empowered by iPython's features
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel cohen <netanelc305@protonmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel cohen <netanelc305@protonmail.com>
 License: Copyright (c) 2012-2023 Doron Zarhi and Metan Perelman
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
@@ -23,14 +23,15 @@
         NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
         LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
         OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
         WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://github.com/doronz88/hilda
 Project-URL: Bug Reports, https://github.com/doronz88/hilda/issues
 Keywords: python,debugger,lldb,ipython,ios,debug
+Classifier: Operating System :: MacOS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -52,26 +53,37 @@
 Requires-Dist: tabulate
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 - [Description](#description)
 - [Installation](#installation)
 - [How to use](#how-to-use)
-    * [Starting a Hilda shell](#starting-a-hilda-shell)
-        + [Bare mode](#bare-mode)
-        + [Remote mode](#remote-mode)
-    * [Usage](#usage)
-    * [Symbol objects](#symbol-objects)
-    * [Globalized symbols](#globalized-symbols)
+    - [Starting a Hilda shell](#starting-a-hilda-shell)
+        - [Attach mode](#attach-mode)
+        - [Launch mode](#launch-mode)
+        - [Bare mode](#bare-mode)
+        - [Remote mode](#remote-mode)
+            - [The connected device is connected via network](#the-connected-device-is-connected-via-network)
+        - [Startup Files](#startup-files)
+    - [Usage](#usage)
+    - [Magic functions](#magic-functions)
+    - [Shortcuts](#shortcuts)
+    - [Configurables](#configurables)
+        - [Attributes](#attributes)
+        - [Example Usage](#example-usage)
+    - [UI Configuration](#ui-configuration)
+    - [Symbol objects](#symbol-objects)
+    - [Globalized symbols](#globalized-symbols)
         - [Searching for the right symbol](#searching-for-the-right-symbol)
+        - [Objective-C Classes](#objective-c-classes)
+    - [Objective-C Objects](#objective-c-objects)
+    - [Using snippets](#using-snippets)
+- [Contributing](#contributing)
 
-        + [Objective-C Classes](#objective-c-classes)
-    * [Objective-C Objects](#objective-c-objects)
-    * [Using snippets](#using-snippets)
-    * [Contributing](#contributing)
+Would you like any further adjustments?
 
 # Description
 
 Hilda is a debugger which combines both the power of LLDB and iPython for easier debugging.
 
 The name originates from the TV show "Hilda", which is the best friend of
 [Frida](https://frida.re/). Both Frida and Hilda are meant for pretty much the same purpose, except Hilda takes the
@@ -117,15 +129,29 @@
 
 Use the attach sub-command in order to start an LLDB shell attached to given process.
 
 ```shell
 hilda attach [-p pid] [-n process-name]
 ```
 
-After attaching, simply execute `hilda` command to enter the hilda shell.
+### Launch mode
+
+Use the attach sub-command in order to launch given process.
+
+```shell
+hilda launch /path/to/executable \
+    --argv arg1 --argv arg2 \
+    --envp NAME=Alice --envp AGE=30 \
+    --stdin /path/to/input.txt \
+    --stdout /path/to/output.txt \
+    --stderr /path/to/error.txt \
+    --wd /path/to/working/directory \
+    --flags 0x01 \
+    --stop-at-entry
+  ```
 
 ### Bare mode
 
 Use "Bare mode" to get a "bare-bones" lldb shell, whereas hilda plugin is already loaded and ready to start. This mode
 is useful when you need to have custom commands for attaching to the target process (for example when debugging OSX
 processes).
 
@@ -171,14 +197,31 @@
 
 Run the following command:
 
 ```shell
 hilda remote HOSTNAME PORT
 ``` 
 
+## Startup Files
+
+Each command can accept startup files to execute on start. As opposed to snippets, the startup files can accept Hilda
+syntax.
+
+#### Startup File Example
+
+```python
+cfg.objc_verbose_monitor = True
+p.bp(ADDRESS)
+p.cont()
+```
+
+```shell
+hilda remote HOSTNAME PORT -f startupfile1 -f startupfile2
+```
+
 ## Usage
 
 Upon starting Hilda shell, you are greeted with:
 
 ```
 Hilda has been successfully loaded! 😎
 Use the p global to access all features.
@@ -321,37 +364,52 @@
 
       Feel free to use local variables inside the expression using format string.
       For example:
       currentDevice = objc_get_class('UIDevice').currentDevice
       evaluate_expression(f'[[{currentDevice} systemName] hasPrefix:@"2"]')
 - `import_module`
     - Import & reload given python module (intended mainly for external snippets)
-- `set_evaluation_unwind`
-    - Set whether LLDB will attempt to unwind the stack whenever an expression evaluation error occurs.
-      Use unwind() to restore when an error is raised in this case.
-- `get_evaluation_unwind`
-    - Get evaluation unwind state.
-      When this value is True, LLDB will attempt unwinding the stack on evaluation errors.
-      Otherwise, the stack frame will remain the same on errors to help you investigate the error.
-- `set_evaluation_ignore_breakpoints`
-    - Set whether to ignore breakpoints while evaluating expressions
-- `get_evaluation_ignore_breakpoints`
-    - Get evaluation "ignore-breakpoints" state.
 - `unwind`
     - Unwind the stack (useful when get_evaluation_unwind() == False)
 
 ## Magic functions
 
 Sometimes accessing the python API can be tiring, so we added some magic functions to help you out!
 
 - `%objc <className>`
     - Equivalent to: `className = p.objc_get_class(className)`
 - `%fbp <filename> <addressInHex>`
     - Equivalent to: `p.file_symbol(addressInHex, filename).bp()`
 
+## Shortcuts
+
+- **F7**: Step Into
+- **F8**: Step Over
+- **F9**: Continue
+- **F10**: Stop
+
+## Configurables
+
+The global `cfg` used to configure various settings for evaluation and monitoring.
+
+### Attributes
+
+- `evaluation_unwind_on_error`: Whether to unwind on error during evaluation. (Default: `False`)
+- `evaluation_ignore_breakpoints`: Whether to ignore breakpoints during evaluation. (Default: `False`)
+- `nsobject_exclusion`: Whether to exclude `NSObject` during evaluation, reducing IPython autocomplete results. (
+  Default: `False`)
+- `objc_verbose_monitor`: When set to `True`, using `monitor()` will automatically print Objective-C method arguments. (
+  Default: `False`)
+
+### Example Usage
+
+```python
+cfg.objc_verbose_monitor = True
+```
+
 ## UI Configuration
 
 Hilda contains minimal UI for examining the target state.
 The UI is divided into views:
 
 - Registers
 - Disassembly
@@ -701,13 +759,9 @@
 This will monitor all XPC related traffic in the given process.
 
 ## Contributing
 
 Please run the tests as follows before submitting a PR:
 
 ```shell
-xcrun python3 -m tests aggregated
-
-# wait for lldb shell prompt
-
-run_tests
+xcrun python3 -m pytest
 ```
```

### Comparing `hilda-1.4.3/hilda.egg-info/SOURCES.txt` & `hilda-2.0.0/hilda.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 .gitignore
+.pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 .github/workflows/python-app.yml
 .github/workflows/python-publish.yml
 gifs/.gitattributes
 gifs/ui.png
 gifs/xpc_print_message.gif
 hilda/__init__.py
 hilda/__main__.py
 hilda/_version.py
+hilda/cli.py
 hilda/common.py
 hilda/exceptions.py
 hilda/hilda_ascii_art.html
 hilda/hilda_client.py
 hilda/launch_lldb.py
 hilda/lldb_entrypoint.py
+hilda/lldb_importer.py
 hilda/objective_c_class.py
 hilda/objective_c_symbol.py
 hilda/registers.py
 hilda/symbol.py
 hilda/symbols_jar.py
 hilda.egg-info/PKG-INFO
 hilda.egg-info/SOURCES.txt
 hilda.egg-info/dependency_links.txt
 hilda.egg-info/entry_points.txt
 hilda.egg-info/requires.txt
 hilda.egg-info/top_level.txt
+hilda/ipython_extensions/events.py
+hilda/ipython_extensions/keybindings.py
+hilda/ipython_extensions/magics.py
 hilda/objective_c/from_ns_to_json.m
 hilda/objective_c/get_objectivec_class_by_module.m
 hilda/objective_c/get_objectivec_class_description.m
 hilda/objective_c/get_objectivec_symbol_data.m
 hilda/objective_c/lsof.m
 hilda/objective_c/to_ns_from_json.m
 hilda/snippets/__init__.py
@@ -51,18 +57,15 @@
 hilda/snippets/macho/image_info.py
 hilda/snippets/macho/macho.py
 hilda/snippets/macho/macho_load_commands.py
 hilda/ui/colors.json
 hilda/ui/ui_manager.py
 hilda/ui/views.py
 tests/__init__.py
-tests/__main__.py
 tests/conftest.py
-tests/hilda_tests.py
-tests/lldb_entrypoint.py
 tests/test_hilda_client/test_from_ns.py
 tests/test_hilda_client/test_hilda_client.py
 tests/test_hilda_client/test_monitor.py
 tests/test_hilda_client/test_ns.py
 tests/test_hilda_client/test_rebind_symbols.py
 tests/test_hilda_client/test_registers.py
 tests/test_snippets/test_xpc.py
```

### Comparing `hilda-1.4.3/pyproject.toml` & `hilda-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 ]
 maintainers = [
     { name = "doronz88", email = "doron88@gmail.com" },
     { name = "matan", email = "matan1008@gmail.com" },
     { name = "netanel cohen", email = "netanelc305@protonmail.com" }
 ]
 classifiers = [
+    "Operating System :: MacOS",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -42,15 +43,15 @@
 package-data = { "hilda" = ["*.html", "*.m", "ui/*.json"] }
 
 [tool.setuptools.packages.find]
 exclude = ["docs*", "tests*"]
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
-version = {attr = "hilda._version.__version__"}
+version = { attr = "hilda._version.__version__" }
 
 [tool.setuptools_scm]
 version_file = "hilda/_version.py"
 
 [build-system]
 requires = ["setuptools>=43.0.0", "setuptools_scm>=8", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `hilda-1.4.3/tests/test_hilda_client/test_from_ns.py` & `hilda-2.0.0/tests/test_hilda_client/test_from_ns.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/tests/test_hilda_client/test_hilda_client.py` & `hilda-2.0.0/tests/test_hilda_client/test_hilda_client.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/tests/test_hilda_client/test_monitor.py` & `hilda-2.0.0/tests/test_hilda_client/test_monitor.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/tests/test_hilda_client/test_ns.py` & `hilda-2.0.0/tests/test_hilda_client/test_ns.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/tests/test_hilda_client/test_registers.py` & `hilda-2.0.0/tests/test_hilda_client/test_registers.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/tests/test_snippets/test_xpc.py` & `hilda-2.0.0/tests/test_snippets/test_xpc.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/tests/test_symbols/test_objective_c_class.py` & `hilda-2.0.0/tests/test_symbols/test_objective_c_class.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/tests/test_symbols/test_objective_c_symbol.py` & `hilda-2.0.0/tests/test_symbols/test_objective_c_symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/tests/test_symbols/test_symbol.py` & `hilda-2.0.0/tests/test_symbols/test_symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-1.4.3/tests/test_symbols/test_symbols_jar.py` & `hilda-2.0.0/tests/test_symbols/test_symbols_jar.py`

 * *Files identical despite different names*

