# Comparing `tmp/lions-1.2.1.tar.gz` & `tmp/lions-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lions-1.2.1.tar", last modified: Thu May 23 09:56:13 2024, max compression
+gzip compressed data, was "lions-1.3.1.tar", last modified: Thu May 23 13:43:13 2024, max compression
```

## Comparing `lions-1.2.1.tar` & `lions-1.3.1.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 09:56:13.242908 lions-1.2.1/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.2.1/LICENSE
--rw-r--r--   0 diogoferreira   (501) staff       (20)     7769 2024-05-23 09:56:13.242834 lions-1.2.1/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)     6916 2024-05-23 09:53:23.000000 lions-1.2.1/README.md
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 09:56:13.236194 lions-1.2.1/lions/
--rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.2.1/lions/__init__.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 09:56:13.238016 lions-1.2.1/lions/cpp_gen/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.2.1/lions/cpp_gen/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2705 2024-05-23 08:42:03.000000 lions-1.2.1/lions/cpp_gen/cpp_generator.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 09:56:13.239883 lions-1.2.1/lions/cpp_gen/templates/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1202 2024-05-22 12:07:18.000000 lions-1.2.1/lions/cpp_gen/templates/lions.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1125 2024-05-22 12:07:18.000000 lions-1.2.1/lions/cpp_gen/templates/lions.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2218 2024-05-23 08:42:03.000000 lions-1.2.1/lions/cpp_gen/templates/msg.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1519 2024-05-23 08:42:03.000000 lions-1.2.1/lions/cpp_gen/templates/msg.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3480 2024-05-23 08:42:03.000000 lions-1.2.1/lions/errors.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 09:56:13.240364 lions-1.2.1/lions/js_gen/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:42:03.000000 lions-1.2.1/lions/js_gen/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2780 2024-05-23 08:42:03.000000 lions-1.2.1/lions/js_gen/js_generator.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.2.1/lions/lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3023 2024-05-23 08:42:03.000000 lions-1.2.1/lions/main.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.2.1/lions/yaml_parser.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 09:56:13.237807 lions-1.2.1/lions.egg-info/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     7769 2024-05-23 09:56:13.000000 lions-1.2.1/lions.egg-info/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)      668 2024-05-23 09:56:13.000000 lions-1.2.1/lions.egg-info/SOURCES.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-23 09:56:13.000000 lions-1.2.1/lions.egg-info/dependency_links.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-23 09:56:13.000000 lions-1.2.1/lions.egg-info/entry_points.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-23 09:56:13.000000 lions-1.2.1/lions.egg-info/requires.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-23 09:56:13.000000 lions-1.2.1/lions.egg-info/top_level.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-23 09:56:13.243220 lions-1.2.1/setup.cfg
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-23 09:55:12.000000 lions-1.2.1/setup.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 09:56:13.241657 lions-1.2.1/tests/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.2.1/tests/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1609 2024-05-23 08:42:03.000000 lions-1.2.1/tests/test_cpp_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-23 08:42:03.000000 lions-1.2.1/tests/test_js_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-23 08:42:03.000000 lions-1.2.1/tests/test_lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-23 08:42:03.000000 lions-1.2.1/tests/test_yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:43:13.070033 lions-1.3.1/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.3.1/LICENSE
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     7975 2024-05-23 13:43:13.069966 lions-1.3.1/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     7122 2024-05-23 12:59:39.000000 lions-1.3.1/README.md
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:43:13.065780 lions-1.3.1/lions/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.3.1/lions/__init__.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:43:13.066899 lions-1.3.1/lions/cpp_gen/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.3.1/lions/cpp_gen/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2705 2024-05-23 08:42:03.000000 lions-1.3.1/lions/cpp_gen/cpp_generator.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:43:13.067883 lions-1.3.1/lions/cpp_gen/templates/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1202 2024-05-22 12:07:18.000000 lions-1.3.1/lions/cpp_gen/templates/lions.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1125 2024-05-22 12:07:18.000000 lions-1.3.1/lions/cpp_gen/templates/lions.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2218 2024-05-23 08:42:03.000000 lions-1.3.1/lions/cpp_gen/templates/msg.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1519 2024-05-23 08:42:03.000000 lions-1.3.1/lions/cpp_gen/templates/msg.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3480 2024-05-23 08:42:03.000000 lions-1.3.1/lions/errors.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:43:13.068196 lions-1.3.1/lions/js_gen/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:42:03.000000 lions-1.3.1/lions/js_gen/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2780 2024-05-23 08:42:03.000000 lions-1.3.1/lions/js_gen/js_generator.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     5223 2024-05-23 12:34:35.000000 lions-1.3.1/lions/lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3176 2024-05-23 12:20:07.000000 lions-1.3.1/lions/main.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:43:13.068513 lions-1.3.1/lions/ts_gen/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-23 12:01:55.000000 lions-1.3.1/lions/ts_gen/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3271 2024-05-23 12:17:43.000000 lions-1.3.1/lions/ts_gen/ts_generator.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.3.1/lions/yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:43:13.066698 lions-1.3.1/lions.egg-info/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     7975 2024-05-23 13:43:13.000000 lions-1.3.1/lions.egg-info/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)      748 2024-05-23 13:43:13.000000 lions-1.3.1/lions.egg-info/SOURCES.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-23 13:43:13.000000 lions-1.3.1/lions.egg-info/dependency_links.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-23 13:43:13.000000 lions-1.3.1/lions.egg-info/entry_points.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-23 13:43:13.000000 lions-1.3.1/lions.egg-info/requires.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-23 13:43:13.000000 lions-1.3.1/lions.egg-info/top_level.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-23 13:43:13.070239 lions-1.3.1/setup.cfg
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-23 13:43:04.000000 lions-1.3.1/setup.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:43:13.069378 lions-1.3.1/tests/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.3.1/tests/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1609 2024-05-23 08:42:03.000000 lions-1.3.1/tests/test_cpp_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-23 13:00:37.000000 lions-1.3.1/tests/test_js_gen copy.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-23 08:42:03.000000 lions-1.3.1/tests/test_lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-23 13:01:41.000000 lions-1.3.1/tests/test_ts_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-23 08:42:03.000000 lions-1.3.1/tests/test_yaml_parser.py
```

### Comparing `lions-1.2.1/LICENSE` & `lions-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lions-1.2.1/PKG-INFO` & `lions-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.2.1
+Version: 1.3.1
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,26 +21,26 @@
 
 # LIONS (Lightweight IoT Network Specification)
 
 ## Index
 
 <!-- TOC start (generated with https://github.com/derlin/bitdowntoc) -->
 
--   [Description](#lions)
+-   [Description](#description)
 -   [Install](#install)
 -   [Usage](#usage)
 -   [Raw Message format](#raw-message-format)
-    -   [C++ representation](#c-representation)
+    -   [Code representation](#code-representation)
 -   [Defining Messages](#defining-messages)
     -   [Structure of Message Files](#structure-of-message-files)
-    -   [Generated Code Overview](#generated-code-overview) - [Constants](#constants)
-    -   [Message Class Structure](#message-class-structure)
+    -   [Generated code](#generated-code)
+        -   [Constants](#constants)
+        -   [Message struct/class](#message-structclass)
 -   [Examples](#examples)
--   [Target language support](#target-language-support)
-
+-   [Target Language Support](#target-language-support)
 <!-- TOC end -->
 
 <!-- TOC --><a name="lions"></a>
 
 ## Description
 
 LIONS is a communication protocol coupled with a compiler, specifically designed for low-bandwidth IoT mesh and ad hoc networks. Originally tailored for LoRa, LIONS is versatile enough to be adapted to various communication standards, thanks to its protocol-agnostic message encoding approach.
@@ -73,18 +73,19 @@
 | 0          | src      | 1            | Source identifier                                 |
 | 1          | dst      | 1            | Destination identifier                            |
 | 2          | next_hop | 1            | Next hop identifier (used for message forwarding) |
 | 3          | msg_id   | 1            | Message identifier                                |
 | 4-5        | checksum | 2            | Checksum for error checking                       |
 | 6-249      | payload  | 244          | Actual data payload                               |
 
-### Raw Message code representation
+### Code representation
 
 -   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c++/generated_code/lions.hpp)
 -   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/lions.js)
+-   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/ts/generated_code/lions.ts)
 
 ## Defining Messages
 
 LIONS uses `.lmsg.yaml` files to define message specifications for IoT networks. Each file can contain multiple message definitions that are used by the LIONS compiler to generate C++ code for message handling.
 
 ### Structure of Message Files
 
@@ -133,15 +134,15 @@
 
 ping:
     id: 0x03
     period: 1000
     description: "Ping message"
 ```
 
-### Generated Code
+### Generated code
 
 The LIONS compiler auto-generates code to facilitate handling, encoding and decoding of messages defined in `.lmsg.yaml` files. Below is an example of how part of the generated code might look for the yaml file above.
 
 #### Constants
 
 The code defines namespaces to hold constants for message IDs and periods, ensuring easy reference throughout the codebase:
 
@@ -157,15 +158,15 @@
 namespace msg_period {
     constexpr uint8_t ACCELEROMETER = 1000;
     constexpr uint8_t MICROPHONE = 0;
     constexpr uint8_t PING = 1000;
 }  // namespace msg_period
 ```
 
-#### Message Struct/Class
+#### Message struct/class
 
 For each message type defined in the YAML files, the LIONS compiler generates a corresponding struct/class. This class includes the specific fields of the message, two constructors, and an encode method.
 
 1. **Initialization Constructor**
 
     - Used to create a new instance of the message class with predefined field values. This constructor initializes the message with specific data relevant to its type.
 
@@ -173,21 +174,23 @@
 
     - Transforms a generic, raw-form message (`LMsg`) into the structured format of the class. This conversion facilitates easier manipulation and interpretation of the message contents within the application.
 
 3. **Encode Method**
     - Converts the structured message back into its raw binary form (`LMsg`) for transmission. This method ensures that the message is properly packaged with its header and payload according to the protocol specifications before being sent over the network.
 
 ---
+
 -   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c%2B%2B/generated_code/my_messages_lmsg.hpp)
 -   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/my_messages_lmsg.js)
+-   [TypeScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/ts/generated_code/my_messages_lmsg.ts)
 
 ## Examples
 
 [Examples](https://github.com/ItsNotSoftware/lions/tree/main/examples)
 
-## Target language support
+## Target Language Support
 
 -   [x] C++
 -   [x] JavaScript
--   [ ] TypeScript
+-   [x] TypeScript
 -   [ ] C
 -   [ ] Python
```

### Comparing `lions-1.2.1/README.md` & `lions-1.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # LIONS (Lightweight IoT Network Specification)
 
 ## Index
 
 <!-- TOC start (generated with https://github.com/derlin/bitdowntoc) -->
 
--   [Description](#lions)
+-   [Description](#description)
 -   [Install](#install)
 -   [Usage](#usage)
 -   [Raw Message format](#raw-message-format)
-    -   [C++ representation](#c-representation)
+    -   [Code representation](#code-representation)
 -   [Defining Messages](#defining-messages)
     -   [Structure of Message Files](#structure-of-message-files)
-    -   [Generated Code Overview](#generated-code-overview) - [Constants](#constants)
-    -   [Message Class Structure](#message-class-structure)
+    -   [Generated code](#generated-code)
+        -   [Constants](#constants)
+        -   [Message struct/class](#message-structclass)
 -   [Examples](#examples)
--   [Target language support](#target-language-support)
-
+-   [Target Language Support](#target-language-support)
 <!-- TOC end -->
 
 <!-- TOC --><a name="lions"></a>
 
 ## Description
 
 LIONS is a communication protocol coupled with a compiler, specifically designed for low-bandwidth IoT mesh and ad hoc networks. Originally tailored for LoRa, LIONS is versatile enough to be adapted to various communication standards, thanks to its protocol-agnostic message encoding approach.
@@ -52,18 +52,19 @@
 | 0          | src      | 1            | Source identifier                                 |
 | 1          | dst      | 1            | Destination identifier                            |
 | 2          | next_hop | 1            | Next hop identifier (used for message forwarding) |
 | 3          | msg_id   | 1            | Message identifier                                |
 | 4-5        | checksum | 2            | Checksum for error checking                       |
 | 6-249      | payload  | 244          | Actual data payload                               |
 
-### Raw Message code representation
+### Code representation
 
 -   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c++/generated_code/lions.hpp)
 -   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/lions.js)
+-   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/ts/generated_code/lions.ts)
 
 ## Defining Messages
 
 LIONS uses `.lmsg.yaml` files to define message specifications for IoT networks. Each file can contain multiple message definitions that are used by the LIONS compiler to generate C++ code for message handling.
 
 ### Structure of Message Files
 
@@ -112,15 +113,15 @@
 
 ping:
     id: 0x03
     period: 1000
     description: "Ping message"
 ```
 
-### Generated Code
+### Generated code
 
 The LIONS compiler auto-generates code to facilitate handling, encoding and decoding of messages defined in `.lmsg.yaml` files. Below is an example of how part of the generated code might look for the yaml file above.
 
 #### Constants
 
 The code defines namespaces to hold constants for message IDs and periods, ensuring easy reference throughout the codebase:
 
@@ -136,15 +137,15 @@
 namespace msg_period {
     constexpr uint8_t ACCELEROMETER = 1000;
     constexpr uint8_t MICROPHONE = 0;
     constexpr uint8_t PING = 1000;
 }  // namespace msg_period
 ```
 
-#### Message Struct/Class
+#### Message struct/class
 
 For each message type defined in the YAML files, the LIONS compiler generates a corresponding struct/class. This class includes the specific fields of the message, two constructors, and an encode method.
 
 1. **Initialization Constructor**
 
     - Used to create a new instance of the message class with predefined field values. This constructor initializes the message with specific data relevant to its type.
 
@@ -152,21 +153,23 @@
 
     - Transforms a generic, raw-form message (`LMsg`) into the structured format of the class. This conversion facilitates easier manipulation and interpretation of the message contents within the application.
 
 3. **Encode Method**
     - Converts the structured message back into its raw binary form (`LMsg`) for transmission. This method ensures that the message is properly packaged with its header and payload according to the protocol specifications before being sent over the network.
 
 ---
+
 -   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c%2B%2B/generated_code/my_messages_lmsg.hpp)
 -   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/my_messages_lmsg.js)
+-   [TypeScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/ts/generated_code/my_messages_lmsg.ts)
 
 ## Examples
 
 [Examples](https://github.com/ItsNotSoftware/lions/tree/main/examples)
 
-## Target language support
+## Target Language Support
 
 -   [x] C++
 -   [x] JavaScript
--   [ ] TypeScript
+-   [x] TypeScript
 -   [ ] C
 -   [ ] Python
```

### Comparing `lions-1.2.1/lions/cpp_gen/cpp_generator.py` & `lions-1.3.1/lions/cpp_gen/cpp_generator.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.1/lions/cpp_gen/templates/lions.cpp.jinja` & `lions-1.3.1/lions/cpp_gen/templates/lions.cpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.2.1/lions/cpp_gen/templates/lions.hpp.jinja` & `lions-1.3.1/lions/cpp_gen/templates/lions.hpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.2.1/lions/cpp_gen/templates/msg.cpp.jinja` & `lions-1.3.1/lions/cpp_gen/templates/msg.cpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.2.1/lions/cpp_gen/templates/msg.hpp.jinja` & `lions-1.3.1/lions/cpp_gen/templates/msg.hpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.2.1/lions/errors.py` & `lions-1.3.1/lions/errors.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.1/lions/js_gen/js_generator.py` & `lions-1.3.1/lions/js_gen/js_generator.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.1/lions/lmsg.py` & `lions-1.3.1/lions/lmsg.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     """
 
     parent_msg_name: str
     name: str
     type: str
     size: int
     start: int = 0
+    buff_type: str = ""
 
     @field_validator("size")
     @classmethod
     def validate_size(cls, v: int) -> int:
         """
         Validate if the size of the field is valid
```

### Comparing `lions-1.2.1/lions/main.py` & `lions-1.3.1/lions/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Copyright (c) 2024 Diogo Ferreira. All rights reserved.
     This code is licensed under the MIT License.
 """
 
 import sys
 import colorama
 from lions.cpp_gen.cpp_generator import CppGenerator
+from lions.ts_gen.ts_generator import TsGenerator
 from lions.yaml_parser import YamlParser
 from colorama import Fore, Style
 from lions.js_gen.js_generator import JsGenerator
 from lions.errors import InvalidTargetLanguageError
 
 
 def print_title():
@@ -58,14 +59,15 @@
 
         # targert language help
         print(
             """
     Target Language:
         cpp - C++
         js - JavaScript
+        ts - TypeScript
         """
         )
 
         sys.exit(1)
 
     msg_files_dir = sys.argv[1]
     output_dir = sys.argv[2]
@@ -77,14 +79,16 @@
     code_generator = None
 
     # Check the target language and initialize the corresponding code generator
     if sys.argv[3] == "c++" or sys.argv[3] == "cpp":
         code_generator = CppGenerator(output_dir)
     elif sys.argv[3] == "js":
         code_generator = JsGenerator(output_dir)
+    elif sys.argv[3] == "ts":
+        code_generator = TsGenerator(output_dir)
     else:
         raise InvalidTargetLanguageError(sys.argv[3])
 
     # Parse the message files and generate the corresponding C++ files
     for filename, msgs in parser.parse_file():
         code_generator.generate_msg_files(filename, msgs)
```

### Comparing `lions-1.2.1/lions/yaml_parser.py` & `lions-1.3.1/lions/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.1/lions.egg-info/PKG-INFO` & `lions-1.3.1/lions.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.2.1
+Version: 1.3.1
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,26 +21,26 @@
 
 # LIONS (Lightweight IoT Network Specification)
 
 ## Index
 
 <!-- TOC start (generated with https://github.com/derlin/bitdowntoc) -->
 
--   [Description](#lions)
+-   [Description](#description)
 -   [Install](#install)
 -   [Usage](#usage)
 -   [Raw Message format](#raw-message-format)
-    -   [C++ representation](#c-representation)
+    -   [Code representation](#code-representation)
 -   [Defining Messages](#defining-messages)
     -   [Structure of Message Files](#structure-of-message-files)
-    -   [Generated Code Overview](#generated-code-overview) - [Constants](#constants)
-    -   [Message Class Structure](#message-class-structure)
+    -   [Generated code](#generated-code)
+        -   [Constants](#constants)
+        -   [Message struct/class](#message-structclass)
 -   [Examples](#examples)
--   [Target language support](#target-language-support)
-
+-   [Target Language Support](#target-language-support)
 <!-- TOC end -->
 
 <!-- TOC --><a name="lions"></a>
 
 ## Description
 
 LIONS is a communication protocol coupled with a compiler, specifically designed for low-bandwidth IoT mesh and ad hoc networks. Originally tailored for LoRa, LIONS is versatile enough to be adapted to various communication standards, thanks to its protocol-agnostic message encoding approach.
@@ -73,18 +73,19 @@
 | 0          | src      | 1            | Source identifier                                 |
 | 1          | dst      | 1            | Destination identifier                            |
 | 2          | next_hop | 1            | Next hop identifier (used for message forwarding) |
 | 3          | msg_id   | 1            | Message identifier                                |
 | 4-5        | checksum | 2            | Checksum for error checking                       |
 | 6-249      | payload  | 244          | Actual data payload                               |
 
-### Raw Message code representation
+### Code representation
 
 -   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c++/generated_code/lions.hpp)
 -   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/lions.js)
+-   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/ts/generated_code/lions.ts)
 
 ## Defining Messages
 
 LIONS uses `.lmsg.yaml` files to define message specifications for IoT networks. Each file can contain multiple message definitions that are used by the LIONS compiler to generate C++ code for message handling.
 
 ### Structure of Message Files
 
@@ -133,15 +134,15 @@
 
 ping:
     id: 0x03
     period: 1000
     description: "Ping message"
 ```
 
-### Generated Code
+### Generated code
 
 The LIONS compiler auto-generates code to facilitate handling, encoding and decoding of messages defined in `.lmsg.yaml` files. Below is an example of how part of the generated code might look for the yaml file above.
 
 #### Constants
 
 The code defines namespaces to hold constants for message IDs and periods, ensuring easy reference throughout the codebase:
 
@@ -157,15 +158,15 @@
 namespace msg_period {
     constexpr uint8_t ACCELEROMETER = 1000;
     constexpr uint8_t MICROPHONE = 0;
     constexpr uint8_t PING = 1000;
 }  // namespace msg_period
 ```
 
-#### Message Struct/Class
+#### Message struct/class
 
 For each message type defined in the YAML files, the LIONS compiler generates a corresponding struct/class. This class includes the specific fields of the message, two constructors, and an encode method.
 
 1. **Initialization Constructor**
 
     - Used to create a new instance of the message class with predefined field values. This constructor initializes the message with specific data relevant to its type.
 
@@ -173,21 +174,23 @@
 
     - Transforms a generic, raw-form message (`LMsg`) into the structured format of the class. This conversion facilitates easier manipulation and interpretation of the message contents within the application.
 
 3. **Encode Method**
     - Converts the structured message back into its raw binary form (`LMsg`) for transmission. This method ensures that the message is properly packaged with its header and payload according to the protocol specifications before being sent over the network.
 
 ---
+
 -   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c%2B%2B/generated_code/my_messages_lmsg.hpp)
 -   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/my_messages_lmsg.js)
+-   [TypeScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/ts/generated_code/my_messages_lmsg.ts)
 
 ## Examples
 
 [Examples](https://github.com/ItsNotSoftware/lions/tree/main/examples)
 
-## Target language support
+## Target Language Support
 
 -   [x] C++
 -   [x] JavaScript
--   [ ] TypeScript
+-   [x] TypeScript
 -   [ ] C
 -   [ ] Python
```

### Comparing `lions-1.2.1/lions.egg-info/SOURCES.txt` & `lions-1.3.1/lions.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -17,12 +17,15 @@
 lions/cpp_gen/cpp_generator.py
 lions/cpp_gen/templates/lions.cpp.jinja
 lions/cpp_gen/templates/lions.hpp.jinja
 lions/cpp_gen/templates/msg.cpp.jinja
 lions/cpp_gen/templates/msg.hpp.jinja
 lions/js_gen/__init__.py
 lions/js_gen/js_generator.py
+lions/ts_gen/__init__.py
+lions/ts_gen/ts_generator.py
 tests/__init__.py
 tests/test_cpp_gen.py
-tests/test_js_gen.py
+tests/test_js_gen copy.py
 tests/test_lmsg.py
+tests/test_ts_gen.py
 tests/test_yaml_parser.py
```

### Comparing `lions-1.2.1/setup.py` & `lions-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lions",
-    version="1.2.1",
+    version="1.3.1",
     author="Diogo Ferreira",
     author_email="itsnotsoftware@gmail.com",
     description="LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={"lions": ["cpp_gen/templates/*.jinja"]},
     url="https://github.com/ItsNotSoftware/lions",
```

### Comparing `lions-1.2.1/tests/test_cpp_gen.py` & `lions-1.3.1/tests/test_cpp_gen.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.1/tests/test_js_gen.py` & `lions-1.3.1/tests/test_js_gen copy.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.1/tests/test_lmsg.py` & `lions-1.3.1/tests/test_lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.1/tests/test_yaml_parser.py` & `lions-1.3.1/tests/test_yaml_parser.py`

 * *Files identical despite different names*

