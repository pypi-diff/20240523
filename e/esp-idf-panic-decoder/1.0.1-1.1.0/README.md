# Comparing `tmp/esp_idf_panic_decoder-1.0.1.tar.gz` & `tmp/esp_idf_panic_decoder-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-idf-panic-decoder/esp-idf-panic-decoder/dist/.tmp-8sbmf_x5/esp_idf_panic_decoder-1.0.1.tar", last modified: Mon Dec 11 08:47:47 2023, max compression
+gzip compressed data, was "/home/runner/work/esp-idf-panic-decoder/esp-idf-panic-decoder/dist/.tmp-258krhfn/esp_idf_panic_decoder-1.1.0.tar", last modified: Thu May 23 03:38:51 2024, max compression
```

## Comparing `esp_idf_panic_decoder-1.0.1.tar` & `esp_idf_panic_decoder-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 08:47:47.000000 esp_idf_panic_decoder-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2023-12-11 08:47:31.000000 esp_idf_panic_decoder-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15874 2023-12-11 08:47:47.000000 esp_idf_panic_decoder-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2023-12-11 08:47:31.000000 esp_idf_panic_decoder-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 08:47:47.000000 esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-11 08:47:31.000000 esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-11 08:47:31.000000 esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11330 2023-12-11 08:47:31.000000 esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder/gdb_panic_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-12-11 08:47:31.000000 esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder/output_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-12-11 08:47:31.000000 esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder/panic_output_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2023-12-11 08:47:31.000000 esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder/pc_address_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2023-12-11 08:47:31.000000 esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder/pc_address_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 08:47:47.000000 esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15874 2023-12-11 08:47:47.000000 esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      540 2023-12-11 08:47:47.000000 esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 08:47:47.000000 esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-11 08:47:47.000000 esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-11 08:47:47.000000 esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2023-12-11 08:47:31.000000 esp_idf_panic_decoder-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 08:47:47.000000 esp_idf_panic_decoder-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:38:51.000000 esp_idf_panic_decoder-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-05-23 03:38:38.000000 esp_idf_panic_decoder-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15874 2024-05-23 03:38:51.000000 esp_idf_panic_decoder-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-23 03:38:38.000000 esp_idf_panic_decoder-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:38:51.000000 esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-23 03:38:38.000000 esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-23 03:38:38.000000 esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-05-23 03:38:38.000000 esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder/gdb_panic_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-23 03:38:38.000000 esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder/output_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-23 03:38:38.000000 esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder/panic_output_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-23 03:38:38.000000 esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder/pc_address_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-23 03:38:38.000000 esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder/pc_address_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:38:51.000000 esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15874 2024-05-23 03:38:51.000000 esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-23 03:38:51.000000 esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 03:38:51.000000 esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-23 03:38:51.000000 esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 03:38:51.000000 esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-23 03:38:38.000000 esp_idf_panic_decoder-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 03:38:51.000000 esp_idf_panic_decoder-1.1.0/setup.cfg
```

### Comparing `esp_idf_panic_decoder-1.0.1/LICENSE` & `esp_idf_panic_decoder-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esp_idf_panic_decoder-1.0.1/PKG-INFO` & `esp_idf_panic_decoder-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp_idf_panic_decoder
-Version: 1.0.1
+Version: 1.1.0
 Summary: ESP-IDF panic decoder
 Author: Espressif Systems
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `esp_idf_panic_decoder-1.0.1/README.md` & `esp_idf_panic_decoder-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder/gdb_panic_server.py` & `esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder/gdb_panic_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 
 GDB_REGS_INFO = {
     'esp32c3': GDB_REGS_INFO_RISCV_ILP32,
     'esp32c2': GDB_REGS_INFO_RISCV_ILP32,
     'esp32c6': GDB_REGS_INFO_RISCV_ILP32,
     'esp32h2': GDB_REGS_INFO_RISCV_ILP32,
     'esp32p4': GDB_REGS_INFO_RISCV_ILP32,
+    'esp32c5': GDB_REGS_INFO_RISCV_ILP32,
+    'esp32c61': GDB_REGS_INFO_RISCV_ILP32,
 }
 
 PanicInfo = namedtuple('PanicInfo', 'core_id regs stack_base_addr stack_data')
 
 
 def build_riscv_panic_output_parser():  # type: () -> typing.Any[typing.Type[ParserElement]]
     """Builds a parser for the panic handler output using pyparsing"""
@@ -155,14 +157,16 @@
 
 PANIC_OUTPUT_PARSERS = {
     'esp32c3': parse_idf_riscv_panic_output,
     'esp32c2': parse_idf_riscv_panic_output,
     'esp32c6': parse_idf_riscv_panic_output,
     'esp32h2': parse_idf_riscv_panic_output,
     'esp32p4': parse_idf_riscv_panic_output,
+    'esp32c5': parse_idf_riscv_panic_output,
+    'esp32c61': parse_idf_riscv_panic_output,
 }
 
 
 class GdbServer:
     def __init__(self, panic_info, target, log_file=None):  # type: (PanicInfo, str, Optional[str]) -> None
         self.panic_info = panic_info
         self.in_stream = sys.stdin
```

### Comparing `esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder/panic_output_decoder.py` & `esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder/panic_output_decoder.py`

 * *Files identical despite different names*

### Comparing `esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder/pc_address_decoder.py` & `esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder/pc_address_decoder.py`

 * *Files identical despite different names*

### Comparing `esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder/pc_address_matcher.py` & `esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder/pc_address_matcher.py`

 * *Files identical despite different names*

### Comparing `esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder.egg-info/PKG-INFO` & `esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-panic-decoder
-Version: 1.0.1
+Version: 1.1.0
 Summary: ESP-IDF panic decoder
 Author: Espressif Systems
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `esp_idf_panic_decoder-1.0.1/esp_idf_panic_decoder.egg-info/SOURCES.txt` & `esp_idf_panic_decoder-1.1.0/esp_idf_panic_decoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esp_idf_panic_decoder-1.0.1/pyproject.toml` & `esp_idf_panic_decoder-1.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -32,22 +32,50 @@
 dynamic = ['version']
 dependencies = ["pyelftools"]
 
 [project.urls]
 Homepage = "https://github.com/espressif/esp-idf-panic-decoder"
 
 [project.optional-dependencies]
-dev = ["pre-commit"]
+dev = [
+    "pre-commit",
+    "commitizen",
+]
 
 [tool.setuptools]
 packages = ["esp_idf_panic_decoder"]
 
 [tool.setuptools.dynamic]
 version = {attr = "esp_idf_panic_decoder.__version__"}
 
+[tool.commitizen]
+version = "1.1.0"
+update_changelog_on_bump = true
+tag_format = "v$version"
+changelog_merge_prerelease = true
+annotated_tag = true
+changelog_start_rev = "v0.2.0"
+bump_message = "change: Update version to $new_version"
+version_files = [
+    "esp_idf_panic_decoder/__init__.py:__version__"
+]
+change_type_order = [
+    "BREAKING CHANGE",
+    "New Features",
+    "Bug Fixes",
+    "Code Refactoring",
+    "Performance Improvements"
+]
+
+[tool.commitizen.change_type_map]
+feat = "New Features"
+fix = "Bug Fixes"
+refactor = "Code Refactoring"
+perf = "Performance Improvements"
+
 [tool.pylint]
     [tool.pylint.'BASIC']
         variable-rgx = "[a-z_][a-z0-9_]{1,30}$" # Variable names must start with a lowercase letter or underscore, followed by any combination of lowercase letters, numbers, or underscores, with a total length of 2 to 30 characters.
 
     [tool.pylint.'MESSAGES CONTROL']
         disable = [
             "duplicate-code",             # R0801: Similar lines in %s files
```

