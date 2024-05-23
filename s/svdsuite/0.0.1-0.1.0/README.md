# Comparing `tmp/svdsuite-0.0.1.tar.gz` & `tmp/svdsuite-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svdsuite-0.0.1.tar", last modified: Fri May  3 23:19:23 2024, max compression
+gzip compressed data, was "svdsuite-0.1.0.tar", last modified: Thu May 23 10:12:10 2024, max compression
```

## Comparing `svdsuite-0.0.1.tar` & `svdsuite-0.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:19:23.644861 svdsuite-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:19:23.636861 svdsuite-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:19:23.640861 svdsuite-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-03 23:19:19.000000 svdsuite-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-03 23:19:19.000000 svdsuite-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-03 23:19:19.000000 svdsuite-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-05-03 23:19:23.644861 svdsuite-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12668 2024-05-03 23:19:19.000000 svdsuite-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-03 23:19:19.000000 svdsuite-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 23:19:23.644861 svdsuite-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:19:23.636861 svdsuite-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:19:23.640861 svdsuite-0.0.1/src/svdsuite/
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-03 23:19:19.000000 svdsuite-0.0.1/src/svdsuite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 23:19:23.000000 svdsuite-0.0.1/src/svdsuite/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    30468 2024-05-03 23:19:19.000000 svdsuite-0.0.1/src/svdsuite/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:19:19.000000 svdsuite-0.0.1/src/svdsuite/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:19:23.640861 svdsuite-0.0.1/src/svdsuite/schema/
--rw-r--r--   0 runner    (1001) docker     (127)    36453 2024-05-03 23:19:19.000000 svdsuite-0.0.1/src/svdsuite/schema/1.3.10.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    39296 2024-05-03 23:19:19.000000 svdsuite-0.0.1/src/svdsuite/schema/1.3.9.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-03 23:19:19.000000 svdsuite-0.0.1/src/svdsuite/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)    28962 2024-05-03 23:19:19.000000 svdsuite-0.0.1/src/svdsuite/svd_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-03 23:19:19.000000 svdsuite-0.0.1/src/svdsuite/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:19:23.644861 svdsuite-0.0.1/src/svdsuite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-05-03 23:19:23.000000 svdsuite-0.0.1/src/svdsuite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-03 23:19:23.000000 svdsuite-0.0.1/src/svdsuite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 23:19:23.000000 svdsuite-0.0.1/src/svdsuite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-03 23:19:23.000000 svdsuite-0.0.1/src/svdsuite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 23:19:23.000000 svdsuite-0.0.1/src/svdsuite.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:19:23.644861 svdsuite-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:19:19.000000 svdsuite-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-03 23:19:19.000000 svdsuite-0.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:19:23.644861 svdsuite-0.0.1/tests/svd/
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-03 23:19:19.000000 svdsuite-0.0.1/tests/svd/parser_testfile.svd
--rw-r--r--   0 runner    (1001) docker     (127)   107129 2024-05-03 23:19:19.000000 svdsuite-0.0.1/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-03 23:19:19.000000 svdsuite-0.0.1/tests/test_serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)   232201 2024-05-03 23:19:19.000000 svdsuite-0.0.1/tests/test_to_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-03 23:19:19.000000 svdsuite-0.0.1/tests/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:12:10.868089 svdsuite-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:12:10.860089 svdsuite-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:12:10.864089 svdsuite-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-23 10:12:06.000000 svdsuite-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-23 10:12:06.000000 svdsuite-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-23 10:12:06.000000 svdsuite-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-05-23 10:12:10.868089 svdsuite-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10688 2024-05-23 10:12:06.000000 svdsuite-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-23 10:12:06.000000 svdsuite-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 10:12:10.868089 svdsuite-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:12:10.864089 svdsuite-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:12:10.864089 svdsuite-0.1.0/src/svdsuite/
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-23 10:12:06.000000 svdsuite-0.1.0/src/svdsuite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 10:12:10.000000 svdsuite-0.1.0/src/svdsuite/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30708 2024-05-23 10:12:06.000000 svdsuite-0.1.0/src/svdsuite/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:12:06.000000 svdsuite-0.1.0/src/svdsuite/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:12:10.868089 svdsuite-0.1.0/src/svdsuite/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)    36453 2024-05-23 10:12:06.000000 svdsuite-0.1.0/src/svdsuite/schema/1.3.10.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    39296 2024-05-23 10:12:06.000000 svdsuite-0.1.0/src/svdsuite/schema/1.3.9.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-23 10:12:06.000000 svdsuite-0.1.0/src/svdsuite/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29988 2024-05-23 10:12:06.000000 svdsuite-0.1.0/src/svdsuite/svd_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-23 10:12:06.000000 svdsuite-0.1.0/src/svdsuite/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:12:10.868089 svdsuite-0.1.0/src/svdsuite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-05-23 10:12:10.000000 svdsuite-0.1.0/src/svdsuite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-23 10:12:10.000000 svdsuite-0.1.0/src/svdsuite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:12:10.000000 svdsuite-0.1.0/src/svdsuite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 10:12:10.000000 svdsuite-0.1.0/src/svdsuite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 10:12:10.000000 svdsuite-0.1.0/src/svdsuite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:12:10.868089 svdsuite-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:12:06.000000 svdsuite-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-23 10:12:06.000000 svdsuite-0.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:12:10.868089 svdsuite-0.1.0/tests/svd/
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-23 10:12:06.000000 svdsuite-0.1.0/tests/svd/parser_testfile.svd
+-rw-r--r--   0 runner    (1001) docker     (127)   107796 2024-05-23 10:12:06.000000 svdsuite-0.1.0/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-23 10:12:06.000000 svdsuite-0.1.0/tests/test_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)   232201 2024-05-23 10:12:06.000000 svdsuite-0.1.0/tests/test_to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-23 10:12:06.000000 svdsuite-0.1.0/tests/test_validate.py
```

### Comparing `svdsuite-0.0.1/.github/workflows/publish.yml` & `svdsuite-0.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `svdsuite-0.0.1/.gitignore` & `svdsuite-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `svdsuite-0.0.1/LICENSE` & `svdsuite-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svdsuite-0.0.1/PKG-INFO` & `svdsuite-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svdsuite
-Version: 0.0.1
+Version: 0.1.0
 Summary: A Python package to parse, process, manipulate, validate, and generate CMSIS SVD files
 Author: Christian Kudera
 License: MIT License
         
         Copyright (c) 2024 ARMify
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -247,89 +247,46 @@
     SauAccessType,
     SVDPeripheral,
     SVDSerializer,
 )
 
 # Create an example device. Alternatevily, you can parse a CMSIS-SVD file and manipulate it.
 device = SVDDevice(
-    size=None,
-    access=None,
-    protection=None,
-    reset_value=None,
-    reset_mask=None,
     xs_no_namespace_schema_location="CMSIS-SVD.xsd",
     schema_version="1.3",
-    vendor=None,
-    vendor_id=None,
     name="STM32F0",
-    series=None,
     version="1.0",
     description="STM32F0 device",
-    license_text=None,
     cpu=SVDCPU(
         name=CPUNameType.CM52,
         revision="r0p0",
         endian=EndianType.LITTLE,
-        mpu_present=False,
-        fpu_present=False,
-        fpu_dp=False,
-        dsp_present=False,
-        icache_present=False,
-        dcache_present=False,
-        itcm_present=False,
-        dtcm_present=False,
-        vtor_present=False,
         nvic_prio_bits=2,
         vendor_systick_config=False,
-        device_num_interrupts=6,
-        sau_num_regions=2,
         sau_regions_config=SVDSauRegionsConfig(
             enabled=True,
             protection_when_disabled=ProtectionStringType.SECURE,
             regions=[
                 SVDSauRegion(
                     enabled=True,
                     name="Region1",
                     base=4096,
                     limit=8192,
                     access=SauAccessType.NON_SECURE,
                 )
             ],
         ),
     ),
-    header_system_filename=None,
-    header_definitions_prefix=None,
     address_unit_bits=8,
     width=32,
     peripherals=[
         SVDPeripheral(
-            size=None,
-            access=None,
-            protection=None,
-            reset_value=None,
-            reset_mask=None,
-            dim=None,
-            dim_increment=None,
-            dim_index=None,
-            dim_name=None,
-            dim_array_index=None,
             name="Timer1",
-            version="1.0",
             description="Timer 1 is a standard timer",
-            alternate_peripheral="Timer1_Alt",
-            group_name="group_name",
-            prepend_to_name="prepend",
-            append_to_name="append",
-            header_struct_name="headerstruct",
-            disable_condition="discond",
             base_address=1073750016,
-            address_blocks=[],
-            interrupts=[],
-            registers_clusters=[],
-            derived_from="test",
         )
     ],
 )
 
 # Serialize the device object. Alternatively, you can use the `device_to_svd_file` method to serialize the device
 # object to an SVD file, or the `device_to_svd_content` method to serialize the device object to bytes string.
 svd_str = SVDSerializer.device_to_svd_str(device, pretty_print=True)
@@ -346,48 +303,30 @@
   <name>STM32F0</name>
   <version>1.0</version>
   <description>STM32F0 device</description>
   <cpu>
     <name>CM52</name>
     <revision>r0p0</revision>
     <endian>little</endian>
-    <mpuPresent>false</mpuPresent>
-    <fpuPresent>false</fpuPresent>
-    <fpuDP>false</fpuDP>
-    <dspPresent>false</dspPresent>
-    <icachePresent>false</icachePresent>
-    <dcachePresent>false</dcachePresent>
-    <itcmPresent>false</itcmPresent>
-    <dtcmPresent>false</dtcmPresent>
-    <vtorPresent>false</vtorPresent>
     <nvicPrioBits>2</nvicPrioBits>
     <vendorSystickConfig>false</vendorSystickConfig>
-    <deviceNumInterrupts>6</deviceNumInterrupts>
-    <sauNumRegions>2</sauNumRegions>
     <sauRegionsConfig enabled="true" protectionWhenDisabled="s">
       <region enabled="true" name="Region1">
         <base>0x1000</base>
         <limit>0x2000</limit>
         <access>n</access>
       </region>
     </sauRegionsConfig>
   </cpu>
   <addressUnitBits>8</addressUnitBits>
   <width>32</width>
   <peripherals>
-    <peripheral derivedFrom="test">
+    <peripheral>
       <name>Timer1</name>
-      <version>1.0</version>
       <description>Timer 1 is a standard timer</description>
-      <alternatePeripheral>Timer1_Alt</alternatePeripheral>
-      <groupName>group_name</groupName>
-      <prependToName>prepend</prependToName>
-      <appendToName>append</appendToName>
-      <headerStructName>headerstruct</headerStructName>
-      <disableCondition>discond</disableCondition>
       <baseAddress>0x40002000</baseAddress>
     </peripheral>
   </peripherals>
 </device>
 ```
 
 ### Validate
```

### Comparing `svdsuite-0.0.1/README.md` & `svdsuite-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -197,89 +197,46 @@
     SauAccessType,
     SVDPeripheral,
     SVDSerializer,
 )
 
 # Create an example device. Alternatevily, you can parse a CMSIS-SVD file and manipulate it.
 device = SVDDevice(
-    size=None,
-    access=None,
-    protection=None,
-    reset_value=None,
-    reset_mask=None,
     xs_no_namespace_schema_location="CMSIS-SVD.xsd",
     schema_version="1.3",
-    vendor=None,
-    vendor_id=None,
     name="STM32F0",
-    series=None,
     version="1.0",
     description="STM32F0 device",
-    license_text=None,
     cpu=SVDCPU(
         name=CPUNameType.CM52,
         revision="r0p0",
         endian=EndianType.LITTLE,
-        mpu_present=False,
-        fpu_present=False,
-        fpu_dp=False,
-        dsp_present=False,
-        icache_present=False,
-        dcache_present=False,
-        itcm_present=False,
-        dtcm_present=False,
-        vtor_present=False,
         nvic_prio_bits=2,
         vendor_systick_config=False,
-        device_num_interrupts=6,
-        sau_num_regions=2,
         sau_regions_config=SVDSauRegionsConfig(
             enabled=True,
             protection_when_disabled=ProtectionStringType.SECURE,
             regions=[
                 SVDSauRegion(
                     enabled=True,
                     name="Region1",
                     base=4096,
                     limit=8192,
                     access=SauAccessType.NON_SECURE,
                 )
             ],
         ),
     ),
-    header_system_filename=None,
-    header_definitions_prefix=None,
     address_unit_bits=8,
     width=32,
     peripherals=[
         SVDPeripheral(
-            size=None,
-            access=None,
-            protection=None,
-            reset_value=None,
-            reset_mask=None,
-            dim=None,
-            dim_increment=None,
-            dim_index=None,
-            dim_name=None,
-            dim_array_index=None,
             name="Timer1",
-            version="1.0",
             description="Timer 1 is a standard timer",
-            alternate_peripheral="Timer1_Alt",
-            group_name="group_name",
-            prepend_to_name="prepend",
-            append_to_name="append",
-            header_struct_name="headerstruct",
-            disable_condition="discond",
             base_address=1073750016,
-            address_blocks=[],
-            interrupts=[],
-            registers_clusters=[],
-            derived_from="test",
         )
     ],
 )
 
 # Serialize the device object. Alternatively, you can use the `device_to_svd_file` method to serialize the device
 # object to an SVD file, or the `device_to_svd_content` method to serialize the device object to bytes string.
 svd_str = SVDSerializer.device_to_svd_str(device, pretty_print=True)
@@ -296,48 +253,30 @@
   <name>STM32F0</name>
   <version>1.0</version>
   <description>STM32F0 device</description>
   <cpu>
     <name>CM52</name>
     <revision>r0p0</revision>
     <endian>little</endian>
-    <mpuPresent>false</mpuPresent>
-    <fpuPresent>false</fpuPresent>
-    <fpuDP>false</fpuDP>
-    <dspPresent>false</dspPresent>
-    <icachePresent>false</icachePresent>
-    <dcachePresent>false</dcachePresent>
-    <itcmPresent>false</itcmPresent>
-    <dtcmPresent>false</dtcmPresent>
-    <vtorPresent>false</vtorPresent>
     <nvicPrioBits>2</nvicPrioBits>
     <vendorSystickConfig>false</vendorSystickConfig>
-    <deviceNumInterrupts>6</deviceNumInterrupts>
-    <sauNumRegions>2</sauNumRegions>
     <sauRegionsConfig enabled="true" protectionWhenDisabled="s">
       <region enabled="true" name="Region1">
         <base>0x1000</base>
         <limit>0x2000</limit>
         <access>n</access>
       </region>
     </sauRegionsConfig>
   </cpu>
   <addressUnitBits>8</addressUnitBits>
   <width>32</width>
   <peripherals>
-    <peripheral derivedFrom="test">
+    <peripheral>
       <name>Timer1</name>
-      <version>1.0</version>
       <description>Timer 1 is a standard timer</description>
-      <alternatePeripheral>Timer1_Alt</alternatePeripheral>
-      <groupName>group_name</groupName>
-      <prependToName>prepend</prependToName>
-      <appendToName>append</appendToName>
-      <headerStructName>headerstruct</headerStructName>
-      <disableCondition>discond</disableCondition>
       <baseAddress>0x40002000</baseAddress>
     </peripheral>
   </peripherals>
 </device>
 ```
 
 ### Validate
```

### Comparing `svdsuite-0.0.1/pyproject.toml` & `svdsuite-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `svdsuite-0.0.1/src/svdsuite/__init__.py` & `svdsuite-0.1.0/src/svdsuite/__init__.py`

 * *Files identical despite different names*

### Comparing `svdsuite-0.0.1/src/svdsuite/parse.py` & `svdsuite-0.1.0/src/svdsuite/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,21 @@
 def _to_int(value: None | str, base: int = 0) -> None | int: ...
 
 
 def _to_int(value: None | str, base: int = 0) -> None | int:
     if value is None:
         return None
 
-    return int(value, base)
+    # transfer binary value to a string int function can handle
+    value = value.replace("#", "0b")
+
+    try:
+        return int(value, base)
+    except ValueError as exc:
+        raise NotImplementedError(f"can't parse value '{value}' in function _to_int") from exc
 
 
 class SVDParserException(Exception):
     pass
 
 
 class SVDParser:
```

### Comparing `svdsuite-0.0.1/src/svdsuite/schema/1.3.10.xsd` & `svdsuite-0.1.0/src/svdsuite/schema/1.3.10.xsd`

 * *Files identical despite different names*

### Comparing `svdsuite-0.0.1/src/svdsuite/schema/1.3.9.xsd` & `svdsuite-0.1.0/src/svdsuite/schema/1.3.9.xsd`

 * *Files identical despite different names*

### Comparing `svdsuite-0.0.1/src/svdsuite/serialize.py` & `svdsuite-0.1.0/src/svdsuite/serialize.py`

 * *Files identical despite different names*

### Comparing `svdsuite-0.0.1/src/svdsuite/svd_model.py` & `svdsuite-0.1.0/src/svdsuite/svd_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Tuple, Union
 from enum import Enum
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 import lxml.etree
 
 
 def _append_element(name: str, text: str) -> lxml.etree._Element:  # pyright: ignore[reportPrivateUsage]
     element = lxml.etree.Element(name)
     element.text = text
     return element
@@ -189,18 +189,18 @@
     def from_str(cls, label: str):
         try:
             return cls(label)
         except ValueError as exc:
             raise NotImplementedError from exc
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SVDSauRegion:
-    enabled: None | bool
-    name: None | str
+    enabled: None | bool = None
+    name: None | str = None
     base: int
     limit: int
     access: SauAccessType
 
     def to_xml(self) -> lxml.etree._Element:  # pyright: ignore[reportPrivateUsage]
         element = lxml.etree.Element("region")
 
@@ -213,19 +213,19 @@
         element.append(_append_element("base", text=f"{self.base:#x}"))
         element.append(_append_element("limit", text=f"{self.limit:#x}"))
         element.append(_append_element("access", text=self.access.value))
 
         return element
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SVDSauRegionsConfig:
-    enabled: None | bool
-    protection_when_disabled: None | ProtectionStringType
-    regions: List[SVDSauRegion]
+    enabled: None | bool = None
+    protection_when_disabled: None | ProtectionStringType = None
+    regions: List[SVDSauRegion] = field(default_factory=list)
 
     def to_xml(self) -> lxml.etree._Element:  # pyright: ignore[reportPrivateUsage]
         element = lxml.etree.Element("sauRegionsConfig")
 
         if self.enabled is not None:
             element.attrib["enabled"] = str(self.enabled).lower()
 
@@ -238,33 +238,33 @@
 
         for region in self.regions:
             element.append(region.to_xml())
 
         return element
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SVDCPU:
     name: CPUNameType
     revision: str
     endian: EndianType
-    mpu_present: None | bool
-    fpu_present: None | bool
-    fpu_dp: None | bool
-    dsp_present: None | bool
-    icache_present: None | bool
-    dcache_present: None | bool
-    itcm_present: None | bool
-    dtcm_present: None | bool
-    vtor_present: None | bool
+    mpu_present: None | bool = None
+    fpu_present: None | bool = None
+    fpu_dp: None | bool = None
+    dsp_present: None | bool = None
+    icache_present: None | bool = None
+    dcache_present: None | bool = None
+    itcm_present: None | bool = None
+    dtcm_present: None | bool = None
+    vtor_present: None | bool = None
     nvic_prio_bits: int
     vendor_systick_config: bool
-    device_num_interrupts: None | int
-    sau_num_regions: None | int
-    sau_regions_config: None | SVDSauRegionsConfig
+    device_num_interrupts: None | int = None
+    sau_num_regions: None | int = None
+    sau_regions_config: None | SVDSauRegionsConfig = None
 
     def to_xml(self) -> lxml.etree._Element:  # pyright: ignore[reportPrivateUsage]
         element = lxml.etree.Element("cpu")
 
         element.append(_append_element("name", text=self.name.value))
         element.append(_append_element("revision", text=self.revision))
         element.append(_append_element("endian", text=self.endian.value))
@@ -307,20 +307,20 @@
 
         if self.sau_regions_config is not None:
             element.append(self.sau_regions_config.to_xml())
 
         return element
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SVDEnumeratedValueMap:
     name: str
-    description: None | str
-    value: None | str  # int value, but can contain 'do not care' bits represented by >x<
-    is_default: None | bool
+    description: None | str = None
+    value: None | str = None  # int value, but can contain 'do not care' bits represented by >x<
+    is_default: None | bool = None
 
     def to_xml(self) -> lxml.etree._Element:  # pyright: ignore[reportPrivateUsage]
         element = lxml.etree.Element("enumeratedValue")
 
         element.append(_append_element("name", text=self.name))
 
         if self.description is not None:
@@ -331,17 +331,17 @@
 
         if self.is_default is not None:
             element.append(_append_element("isDefault", text=str(self.is_default).lower()))
 
         return element
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SVDDimArrayIndex:
-    header_enum_name: None | str
+    header_enum_name: None | str = None
     enumerated_values_map: List[SVDEnumeratedValueMap]
 
     def to_xml(self) -> lxml.etree._Element:  # pyright: ignore[reportPrivateUsage]
         element = lxml.etree.Element("dimArrayIndex")
 
         if self.header_enum_name is not None:
             element.append(_append_element("headerEnumName", text=self.header_enum_name))
@@ -352,56 +352,56 @@
 
         for value in self.enumerated_values_map:
             element.append(value.to_xml())
 
         return element
 
 
-@dataclass
+@dataclass(kw_only=True)
 class _SVDDimElementGroup:
-    dim: None | int
-    dim_increment: None | int
-    dim_index: None | str
-    dim_name: None | str
-    dim_array_index: None | SVDDimArrayIndex
+    dim: None | int = None
+    dim_increment: None | int = None
+    dim_index: None | str = None
+    dim_name: None | str = None
+    dim_array_index: None | SVDDimArrayIndex = None
 
 
-@dataclass
+@dataclass(kw_only=True)
 class _SVDRegisterPropertiesGroup:
-    size: None | int
-    access: None | AccessType
-    protection: None | ProtectionStringType
-    reset_value: None | int
-    reset_mask: None | int
+    size: None | int = None
+    access: None | AccessType = None
+    protection: None | ProtectionStringType = None
+    reset_value: None | int = None
+    reset_mask: None | int = None
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SVDAddressBlock:
     offset: int
     size: int
     usage: EnumeratedTokenType
-    protection: None | ProtectionStringType
+    protection: None | ProtectionStringType = None
 
     def to_xml(self) -> lxml.etree._Element:  # pyright: ignore[reportPrivateUsage]
         element = lxml.etree.Element("addressBlock")
 
         element.append(_append_element("offset", text=f"{self.offset:#x}"))
         element.append(_append_element("size", text=f"{self.size:#x}"))
         element.append(_append_element("usage", text=self.usage.value))
 
         if self.protection is not None:
             element.append(_append_element("protection", text=self.protection.value))
 
         return element
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SVDInterrupt:
     name: str
-    description: None | str
+    description: None | str = None
     value: int
 
     def to_xml(self) -> lxml.etree._Element:  # pyright: ignore[reportPrivateUsage]
         element = lxml.etree.Element("interrupt")
 
         element.append(_append_element("name", text=self.name))
 
@@ -409,19 +409,19 @@
             element.append(_append_element("description", text=self.description))
 
         element.append(_append_element("value", text=str(self.value)))
 
         return element
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SVDWriteConstraint:
-    write_as_read: None | bool
-    use_enumerated_values: None | bool
-    range_: None | Tuple[int, int]
+    write_as_read: None | bool = None
+    use_enumerated_values: None | bool = None
+    range_: None | Tuple[int, int] = None
 
     def to_xml(self) -> lxml.etree._Element:  # pyright: ignore[reportPrivateUsage]
         element = lxml.etree.Element("writeConstraint")
 
         if self.write_as_read is not None:
             element.append(_append_element("writeAsRead", text=str(self.write_as_read).lower()))
 
@@ -437,21 +437,21 @@
         # ensure that we get <writeConstraint ... ></writeConstraint> and not <writeConstraint ... />
         if self.write_as_read is None and self.use_enumerated_values is None and self.range_ is None:
             element.text = ""
 
         return element
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SVDEnumeratedValue:
-    name: None | str
-    header_enum_name: None | str
-    usage: None | EnumUsageType
+    name: None | str = None
+    header_enum_name: None | str = None
+    usage: None | EnumUsageType = None
     enumerated_values_map: List[SVDEnumeratedValueMap]
-    derived_from: None | str
+    derived_from: None | str = None
 
     def to_xml(self) -> lxml.etree._Element:  # pyright: ignore[reportPrivateUsage]
         element = lxml.etree.Element("enumeratedValues")
 
         if self.derived_from is not None:
             element.attrib["derivedFrom"] = self.derived_from
 
@@ -470,29 +470,29 @@
 
         for value in self.enumerated_values_map:
             element.append(value.to_xml())
 
         return element
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SVDField(_SVDDimElementGroup):
     name: str
-    description: None | str
-    bit_offset: None | int
-    bit_width: None | int
-    lsb: None | int
-    msb: None | int
-    bit_range: None | str
-    access: None | AccessType
-    modified_write_values: None | ModifiedWriteValuesType
-    write_constraint: None | SVDWriteConstraint
-    read_action: None | ReadActionType
-    enumerated_values: List[SVDEnumeratedValue]
-    derived_from: None | str
+    description: None | str = None
+    bit_offset: None | int = None
+    bit_width: None | int = None
+    lsb: None | int = None
+    msb: None | int = None
+    bit_range: None | str = None
+    access: None | AccessType = None
+    modified_write_values: None | ModifiedWriteValuesType = None
+    write_constraint: None | SVDWriteConstraint = None
+    read_action: None | ReadActionType = None
+    enumerated_values: List[SVDEnumeratedValue] = field(default_factory=list)
+    derived_from: None | str = None
 
     def to_xml(self) -> lxml.etree._Element:  # pyright: ignore[reportPrivateUsage]
         element = lxml.etree.Element("field")
 
         if self.derived_from is not None:
             element.attrib["derivedFrom"] = self.derived_from
 
@@ -541,28 +541,28 @@
 
         for value in self.enumerated_values:
             element.append(value.to_xml())
 
         return element
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SVDRegister(_SVDDimElementGroup, _SVDRegisterPropertiesGroup):
     name: str
-    display_name: None | str
-    description: None | str
-    alternate_group: None | str
-    alternate_register: None | str
+    display_name: None | str = None
+    description: None | str = None
+    alternate_group: None | str = None
+    alternate_register: None | str = None
     address_offset: int
-    data_type: None | DataTypeType
-    modified_write_values: None | ModifiedWriteValuesType
-    write_constraint: None | SVDWriteConstraint
-    read_action: None | ReadActionType
-    fields: List[SVDField]
-    derived_from: None | str
+    data_type: None | DataTypeType = None
+    modified_write_values: None | ModifiedWriteValuesType = None
+    write_constraint: None | SVDWriteConstraint = None
+    read_action: None | ReadActionType = None
+    fields: List[SVDField] = field(default_factory=list)
+    derived_from: None | str = None
 
     def to_xml(self) -> lxml.etree._Element:  # pyright: ignore[reportPrivateUsage]
         element = lxml.etree.Element("register")
 
         if self.derived_from is not None:
             element.attrib["derivedFrom"] = self.derived_from
 
@@ -623,31 +623,31 @@
 
         if self.read_action is not None:
             element.append(_append_element("readAction", text=self.read_action.value))
 
         if self.fields:
             fields_element = lxml.etree.Element("fields")
 
-            for field in self.fields:
-                fields_element.append(field.to_xml())
+            for field_ in self.fields:
+                fields_element.append(field_.to_xml())
 
             element.append(fields_element)
 
         return element
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SVDCluster(_SVDDimElementGroup, _SVDRegisterPropertiesGroup):
     name: str
-    description: None | str
-    alternate_cluster: None | str
-    header_struct_name: None | str
+    description: None | str = None
+    alternate_cluster: None | str = None
+    header_struct_name: None | str = None
     address_offset: int
-    registers_clusters: List[Union[SVDRegister, "SVDCluster"]]
-    derived_from: None | str
+    registers_clusters: List[Union[SVDRegister, "SVDCluster"]] = field(default_factory=list)
+    derived_from: None | str = None
 
     def to_xml(self) -> lxml.etree._Element:  # pyright: ignore[reportPrivateUsage]
         element = lxml.etree.Element("cluster")
 
         if self.derived_from is not None:
             element.attrib["derivedFrom"] = self.derived_from
 
@@ -696,30 +696,30 @@
 
         for register_cluster in self.registers_clusters:
             element.append(register_cluster.to_xml())
 
         return element
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SVDPeripheral(_SVDDimElementGroup, _SVDRegisterPropertiesGroup):
     name: str
-    version: None | str
-    description: None | str
-    alternate_peripheral: None | str
-    group_name: None | str
-    prepend_to_name: None | str
-    append_to_name: None | str
-    header_struct_name: None | str
-    disable_condition: None | str
+    version: None | str = None
+    description: None | str = None
+    alternate_peripheral: None | str = None
+    group_name: None | str = None
+    prepend_to_name: None | str = None
+    append_to_name: None | str = None
+    header_struct_name: None | str = None
+    disable_condition: None | str = None
     base_address: int
-    address_blocks: List[SVDAddressBlock]
-    interrupts: List[SVDInterrupt]
-    registers_clusters: List[SVDRegister | SVDCluster]
-    derived_from: None | str
+    address_blocks: List[SVDAddressBlock] = field(default_factory=list)
+    interrupts: List[SVDInterrupt] = field(default_factory=list)
+    registers_clusters: List[SVDRegister | SVDCluster] = field(default_factory=list)
+    derived_from: None | str = None
 
     def to_xml(self) -> lxml.etree._Element:  # pyright: ignore[reportPrivateUsage]
         element = lxml.etree.Element("peripheral")
 
         if self.derived_from is not None:
             element.attrib["derivedFrom"] = self.derived_from
 
@@ -794,31 +794,31 @@
                 registers_element.append(register_cluster.to_xml())
 
             element.append(registers_element)
 
         return element
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SVDDevice(_SVDRegisterPropertiesGroup):
     xs_no_namespace_schema_location: str
     schema_version: str
-    vendor: None | str
-    vendor_id: None | str
+    vendor: None | str = None
+    vendor_id: None | str = None
     name: str
-    series: None | str
+    series: None | str = None
     version: str
     description: str
-    license_text: None | str
-    cpu: None | SVDCPU
-    header_system_filename: None | str
-    header_definitions_prefix: None | str
+    license_text: None | str = None
+    cpu: None | SVDCPU = None
+    header_system_filename: None | str = None
+    header_definitions_prefix: None | str = None
     address_unit_bits: int
     width: int
-    peripherals: List[SVDPeripheral]
+    peripherals: List[SVDPeripheral] = field(default_factory=list)
 
     def to_xml(self) -> lxml.etree._Element:  # pyright: ignore[reportPrivateUsage]
         _xs = "http://www.w3.org/2001/XMLSchema-instance"
 
         element = lxml.etree.Element("device", nsmap={"xs": _xs})
 
         element.attrib[
```

### Comparing `svdsuite-0.0.1/src/svdsuite/validate.py` & `svdsuite-0.1.0/src/svdsuite/validate.py`

 * *Files identical despite different names*

### Comparing `svdsuite-0.0.1/src/svdsuite.egg-info/PKG-INFO` & `svdsuite-0.1.0/src/svdsuite.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svdsuite
-Version: 0.0.1
+Version: 0.1.0
 Summary: A Python package to parse, process, manipulate, validate, and generate CMSIS SVD files
 Author: Christian Kudera
 License: MIT License
         
         Copyright (c) 2024 ARMify
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -247,89 +247,46 @@
     SauAccessType,
     SVDPeripheral,
     SVDSerializer,
 )
 
 # Create an example device. Alternatevily, you can parse a CMSIS-SVD file and manipulate it.
 device = SVDDevice(
-    size=None,
-    access=None,
-    protection=None,
-    reset_value=None,
-    reset_mask=None,
     xs_no_namespace_schema_location="CMSIS-SVD.xsd",
     schema_version="1.3",
-    vendor=None,
-    vendor_id=None,
     name="STM32F0",
-    series=None,
     version="1.0",
     description="STM32F0 device",
-    license_text=None,
     cpu=SVDCPU(
         name=CPUNameType.CM52,
         revision="r0p0",
         endian=EndianType.LITTLE,
-        mpu_present=False,
-        fpu_present=False,
-        fpu_dp=False,
-        dsp_present=False,
-        icache_present=False,
-        dcache_present=False,
-        itcm_present=False,
-        dtcm_present=False,
-        vtor_present=False,
         nvic_prio_bits=2,
         vendor_systick_config=False,
-        device_num_interrupts=6,
-        sau_num_regions=2,
         sau_regions_config=SVDSauRegionsConfig(
             enabled=True,
             protection_when_disabled=ProtectionStringType.SECURE,
             regions=[
                 SVDSauRegion(
                     enabled=True,
                     name="Region1",
                     base=4096,
                     limit=8192,
                     access=SauAccessType.NON_SECURE,
                 )
             ],
         ),
     ),
-    header_system_filename=None,
-    header_definitions_prefix=None,
     address_unit_bits=8,
     width=32,
     peripherals=[
         SVDPeripheral(
-            size=None,
-            access=None,
-            protection=None,
-            reset_value=None,
-            reset_mask=None,
-            dim=None,
-            dim_increment=None,
-            dim_index=None,
-            dim_name=None,
-            dim_array_index=None,
             name="Timer1",
-            version="1.0",
             description="Timer 1 is a standard timer",
-            alternate_peripheral="Timer1_Alt",
-            group_name="group_name",
-            prepend_to_name="prepend",
-            append_to_name="append",
-            header_struct_name="headerstruct",
-            disable_condition="discond",
             base_address=1073750016,
-            address_blocks=[],
-            interrupts=[],
-            registers_clusters=[],
-            derived_from="test",
         )
     ],
 )
 
 # Serialize the device object. Alternatively, you can use the `device_to_svd_file` method to serialize the device
 # object to an SVD file, or the `device_to_svd_content` method to serialize the device object to bytes string.
 svd_str = SVDSerializer.device_to_svd_str(device, pretty_print=True)
@@ -346,48 +303,30 @@
   <name>STM32F0</name>
   <version>1.0</version>
   <description>STM32F0 device</description>
   <cpu>
     <name>CM52</name>
     <revision>r0p0</revision>
     <endian>little</endian>
-    <mpuPresent>false</mpuPresent>
-    <fpuPresent>false</fpuPresent>
-    <fpuDP>false</fpuDP>
-    <dspPresent>false</dspPresent>
-    <icachePresent>false</icachePresent>
-    <dcachePresent>false</dcachePresent>
-    <itcmPresent>false</itcmPresent>
-    <dtcmPresent>false</dtcmPresent>
-    <vtorPresent>false</vtorPresent>
     <nvicPrioBits>2</nvicPrioBits>
     <vendorSystickConfig>false</vendorSystickConfig>
-    <deviceNumInterrupts>6</deviceNumInterrupts>
-    <sauNumRegions>2</sauNumRegions>
     <sauRegionsConfig enabled="true" protectionWhenDisabled="s">
       <region enabled="true" name="Region1">
         <base>0x1000</base>
         <limit>0x2000</limit>
         <access>n</access>
       </region>
     </sauRegionsConfig>
   </cpu>
   <addressUnitBits>8</addressUnitBits>
   <width>32</width>
   <peripherals>
-    <peripheral derivedFrom="test">
+    <peripheral>
       <name>Timer1</name>
-      <version>1.0</version>
       <description>Timer 1 is a standard timer</description>
-      <alternatePeripheral>Timer1_Alt</alternatePeripheral>
-      <groupName>group_name</groupName>
-      <prependToName>prepend</prependToName>
-      <appendToName>append</appendToName>
-      <headerStructName>headerstruct</headerStructName>
-      <disableCondition>discond</disableCondition>
       <baseAddress>0x40002000</baseAddress>
     </peripheral>
   </peripherals>
 </device>
 ```
 
 ### Validate
```

### Comparing `svdsuite-0.0.1/src/svdsuite.egg-info/SOURCES.txt` & `svdsuite-0.1.0/src/svdsuite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `svdsuite-0.0.1/tests/conftest.py` & `svdsuite-0.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `svdsuite-0.0.1/tests/svd/parser_testfile.svd` & `svdsuite-0.1.0/tests/svd/parser_testfile.svd`

 * *Files identical despite different names*

### Comparing `svdsuite-0.0.1/tests/test_parsing.py` & `svdsuite-0.1.0/tests/test_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Callable, Any
 import pytest
 
-from svdsuite.parse import SVDParser, SVDParserException
+from svdsuite.parse import SVDParser, SVDParserException, _to_int  # type: ignore
 from svdsuite.svd_model import (
     SVDAddressBlock,
     SVDCluster,
     SVDCPU,
     SVDDevice,
     SVDEnumeratedValue,
     SVDEnumeratedValueMap,
@@ -83,14 +83,37 @@
     def test_cls_for_xml_content(self, get_test_svd_file_content: Callable[[str], bytes]):
         file_content = get_test_svd_file_content("parser_testfile.svd")
         parser = SVDParser.for_xml_content(file_content)
 
         assert isinstance(parser, SVDParser)
 
 
+class TestToInt:
+    @pytest.mark.parametrize(
+        "test_input,expected",
+        [
+            ("+5", 5),
+            ("+0x5", 5),
+            ("+0X5", 5),
+            ("+0xaAbB", 43707),
+            ("+0x9f", 159),
+            ("5", 5),
+            ("0x5", 5),
+            ("0X5", 5),
+            ("0xaAbB", 43707),
+            ("0x9f", 159),
+            ("+#101", 5),
+            pytest.param(None, None),
+            pytest.param("+!", None, marks=pytest.mark.xfail(strict=True, raises=NotImplementedError)),
+        ],
+    )
+    def test_to_int(self, test_input: str, expected: int):
+        assert _to_int(test_input) == expected
+
+
 class TestDeviceParsing:
     def test_xs_no_namespace_schema_location(self, get_device: Callable[[], SVDDevice]):
         device = get_device()
 
         assert device.xs_no_namespace_schema_location == "CMSIS-SVD.xsd"
 
     def test_schema_version(self, get_device: Callable[[], SVDDevice]):
```

### Comparing `svdsuite-0.0.1/tests/test_serialize.py` & `svdsuite-0.1.0/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `svdsuite-0.0.1/tests/test_to_xml.py` & `svdsuite-0.1.0/tests/test_to_xml.py`

 * *Files identical despite different names*

### Comparing `svdsuite-0.0.1/tests/test_validate.py` & `svdsuite-0.1.0/tests/test_validate.py`

 * *Files identical despite different names*

