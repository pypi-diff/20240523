# Comparing `tmp/unii-1.0.0b1.tar.gz` & `tmp/unii-1.0.0b2.tar.gz`

## Comparing `unii-1.0.0b1.tar` & `unii-1.0.0b2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 unii-1.0.0b1/MANIFEST.in
--rw-r--r--   0        0        0    17565 2020-02-02 00:00:00.000000 unii-1.0.0b1/logo.png
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 unii-1.0.0b1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/__init__.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/settings.json
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_auto_reconnect.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_command_data_helpers.py
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_connect_encrypted.py
--rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_connect_unencrypted.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_device_status.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_equipment_information.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_inputs.py
--rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_message.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_message_checksum.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_message_encryption.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_outputs.py
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_sections.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/__init__.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/__main__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/py.typed
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/sia_code.py
--rw-r--r--   0        0        0    18630 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/unii.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/unii_command.py
--rw-r--r--   0        0        0    25805 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/unii_command_data.py
--rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/unii_connection.py
--rw-r--r--   0        0        0    13352 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/unii_message.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 unii-1.0.0b1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 unii-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 unii-1.0.0b1/README.md
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 unii-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 unii-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 unii-1.0.0b2/MANIFEST.in
+-rw-r--r--   0        0        0    17565 2020-02-02 00:00:00.000000 unii-1.0.0b2/logo.png
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 unii-1.0.0b2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 unii-1.0.0b2/tests/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 unii-1.0.0b2/tests/settings.json
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 unii-1.0.0b2/tests/test_unii_auto_reconnect.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 unii-1.0.0b2/tests/test_unii_command_data_helpers.py
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 unii-1.0.0b2/tests/test_unii_connect_encrypted.py
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 unii-1.0.0b2/tests/test_unii_connect_unencrypted.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 unii-1.0.0b2/tests/test_unii_device_status.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 unii-1.0.0b2/tests/test_unii_equipment_information.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 unii-1.0.0b2/tests/test_unii_inputs.py
+-rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 unii-1.0.0b2/tests/test_unii_message.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 unii-1.0.0b2/tests/test_unii_message_checksum.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 unii-1.0.0b2/tests/test_unii_message_encryption.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 unii-1.0.0b2/tests/test_unii_outputs.py
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 unii-1.0.0b2/tests/test_unii_sections.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 unii-1.0.0b2/unii/__init__.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 unii-1.0.0b2/unii/__main__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 unii-1.0.0b2/unii/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unii-1.0.0b2/unii/py.typed
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 unii-1.0.0b2/unii/sia_code.py
+-rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 unii-1.0.0b2/unii/unii.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 unii-1.0.0b2/unii/unii_command.py
+-rw-r--r--   0        0        0    25805 2020-02-02 00:00:00.000000 unii-1.0.0b2/unii/unii_command_data.py
+-rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 unii-1.0.0b2/unii/unii_connection.py
+-rw-r--r--   0        0        0    13352 2020-02-02 00:00:00.000000 unii-1.0.0b2/unii/unii_message.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 unii-1.0.0b2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 unii-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 unii-1.0.0b2/README.md
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 unii-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 unii-1.0.0b2/PKG-INFO
```

### Comparing `unii-1.0.0b1/logo.png` & `unii-1.0.0b2/logo.png`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/.github/workflows/python-publish.yml` & `unii-1.0.0b2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/tests/test_unii_auto_reconnect.py` & `unii-1.0.0b2/tests/test_unii_auto_reconnect.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/tests/test_unii_command_data_helpers.py` & `unii-1.0.0b2/tests/test_unii_command_data_helpers.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/tests/test_unii_connect_encrypted.py` & `unii-1.0.0b2/tests/test_unii_connect_encrypted.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/tests/test_unii_connect_unencrypted.py` & `unii-1.0.0b2/tests/test_unii_connect_unencrypted.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/tests/test_unii_device_status.py` & `unii-1.0.0b2/tests/test_unii_device_status.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/tests/test_unii_equipment_information.py` & `unii-1.0.0b2/tests/test_unii_equipment_information.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/tests/test_unii_inputs.py` & `unii-1.0.0b2/tests/test_unii_inputs.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/tests/test_unii_message.py` & `unii-1.0.0b2/tests/test_unii_message.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/tests/test_unii_message_checksum.py` & `unii-1.0.0b2/tests/test_unii_message_checksum.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/tests/test_unii_message_encryption.py` & `unii-1.0.0b2/tests/test_unii_message_encryption.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/tests/test_unii_outputs.py` & `unii-1.0.0b2/tests/test_unii_outputs.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/tests/test_unii_sections.py` & `unii-1.0.0b2/tests/test_unii_sections.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/unii/__main__.py` & `unii-1.0.0b2/unii/__main__.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/unii/sia_code.py` & `unii-1.0.0b2/unii/sia_code.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/unii/unii.py` & `unii-1.0.0b2/unii/unii.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,18 +343,18 @@
                 self.sections[section.number] = section
             elif section.number in self.sections:
                 self.sections[section.number].update(section)
 
     def _handle_section_status(self, data: UNiiSectionStatus):
         for _, section_status in data.items():
             if section_status.number in self.sections:
-                self.sections[section_status.number].update(section_status)
-                self.sections[section_status.number]["active"] = (
+                section_status["active"] = (
                     section_status.armed_state != UNiiSectionArmedState.NOT_PROGRAMMED
                 )
+                self.sections[section_status.number].update(section_status)
             elif section_status.armed_state != UNiiSectionArmedState.NOT_PROGRAMMED:
                 # This should never happen
                 logger.warning(
                     "Status for unknown section %i changed", section_status.number
                 )
 
     def _handle_input_status_update(self, input_status: UNiiInputStatusRecord):
```

### Comparing `unii-1.0.0b1/unii/unii_command.py` & `unii-1.0.0b2/unii/unii_command.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/unii/unii_command_data.py` & `unii-1.0.0b2/unii/unii_command_data.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/unii/unii_connection.py` & `unii-1.0.0b2/unii/unii_connection.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/unii/unii_message.py` & `unii-1.0.0b2/unii/unii_message.py`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/LICENSE` & `unii-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/README.md` & `unii-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/pyproject.toml` & `unii-1.0.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unii-1.0.0b1/PKG-INFO` & `unii-1.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: unii
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Library to interface with Alphatronics UNii security systems.
 Project-URL: Homepage, https://unii-security.com/
 Project-URL: Repository, https://github.com/unii-security/py-unii
 Project-URL: Issues, https://github.com/unii-security/py-unii/issues
 Author-email: Rogier van Staveren <rogier@batoid.com>
 License: Apache-2.0
 License-File: LICENSE
```

