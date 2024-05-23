# Comparing `tmp/lions-1.2.0.tar.gz` & `tmp/lions-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lions-1.2.0.tar", last modified: Thu May 23 08:51:03 2024, max compression
+gzip compressed data, was "lions-1.2.1.tar", last modified: Thu May 23 09:56:13 2024, max compression
```

## Comparing `lions-1.2.0.tar` & `lions-1.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:51:03.368620 lions-1.2.0/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.2.0/LICENSE
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8244 2024-05-23 08:51:03.368493 lions-1.2.0/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)     7391 2024-05-22 12:07:18.000000 lions-1.2.0/README.md
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:51:03.364705 lions-1.2.0/lions/
--rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.2.0/lions/__init__.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:51:03.365796 lions-1.2.0/lions/cpp_gen/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.2.0/lions/cpp_gen/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2705 2024-05-23 08:42:03.000000 lions-1.2.0/lions/cpp_gen/cpp_generator.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:51:03.366825 lions-1.2.0/lions/cpp_gen/templates/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1202 2024-05-22 12:07:18.000000 lions-1.2.0/lions/cpp_gen/templates/lions.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1125 2024-05-22 12:07:18.000000 lions-1.2.0/lions/cpp_gen/templates/lions.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2218 2024-05-23 08:42:03.000000 lions-1.2.0/lions/cpp_gen/templates/msg.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1519 2024-05-23 08:42:03.000000 lions-1.2.0/lions/cpp_gen/templates/msg.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3480 2024-05-23 08:42:03.000000 lions-1.2.0/lions/errors.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:51:03.367108 lions-1.2.0/lions/js_gen/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:42:03.000000 lions-1.2.0/lions/js_gen/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2780 2024-05-23 08:42:03.000000 lions-1.2.0/lions/js_gen/js_generator.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.2.0/lions/lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3023 2024-05-23 08:42:03.000000 lions-1.2.0/lions/main.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.2.0/lions/yaml_parser.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:51:03.365593 lions-1.2.0/lions.egg-info/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8244 2024-05-23 08:51:03.000000 lions-1.2.0/lions.egg-info/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)      668 2024-05-23 08:51:03.000000 lions-1.2.0/lions.egg-info/SOURCES.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-23 08:51:03.000000 lions-1.2.0/lions.egg-info/dependency_links.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-23 08:51:03.000000 lions-1.2.0/lions.egg-info/entry_points.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-23 08:51:03.000000 lions-1.2.0/lions.egg-info/requires.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-23 08:51:03.000000 lions-1.2.0/lions.egg-info/top_level.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-23 08:51:03.368818 lions-1.2.0/setup.cfg
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-23 08:42:03.000000 lions-1.2.0/setup.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:51:03.367964 lions-1.2.0/tests/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.2.0/tests/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1609 2024-05-23 08:42:03.000000 lions-1.2.0/tests/test_cpp_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-23 08:42:03.000000 lions-1.2.0/tests/test_js_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-23 08:42:03.000000 lions-1.2.0/tests/test_lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-23 08:42:03.000000 lions-1.2.0/tests/test_yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 09:56:13.242908 lions-1.2.1/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.2.1/LICENSE
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     7769 2024-05-23 09:56:13.242834 lions-1.2.1/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     6916 2024-05-23 09:53:23.000000 lions-1.2.1/README.md
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 09:56:13.236194 lions-1.2.1/lions/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.2.1/lions/__init__.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 09:56:13.238016 lions-1.2.1/lions/cpp_gen/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.2.1/lions/cpp_gen/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2705 2024-05-23 08:42:03.000000 lions-1.2.1/lions/cpp_gen/cpp_generator.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 09:56:13.239883 lions-1.2.1/lions/cpp_gen/templates/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1202 2024-05-22 12:07:18.000000 lions-1.2.1/lions/cpp_gen/templates/lions.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1125 2024-05-22 12:07:18.000000 lions-1.2.1/lions/cpp_gen/templates/lions.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2218 2024-05-23 08:42:03.000000 lions-1.2.1/lions/cpp_gen/templates/msg.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1519 2024-05-23 08:42:03.000000 lions-1.2.1/lions/cpp_gen/templates/msg.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3480 2024-05-23 08:42:03.000000 lions-1.2.1/lions/errors.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 09:56:13.240364 lions-1.2.1/lions/js_gen/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:42:03.000000 lions-1.2.1/lions/js_gen/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2780 2024-05-23 08:42:03.000000 lions-1.2.1/lions/js_gen/js_generator.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.2.1/lions/lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3023 2024-05-23 08:42:03.000000 lions-1.2.1/lions/main.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.2.1/lions/yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 09:56:13.237807 lions-1.2.1/lions.egg-info/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     7769 2024-05-23 09:56:13.000000 lions-1.2.1/lions.egg-info/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)      668 2024-05-23 09:56:13.000000 lions-1.2.1/lions.egg-info/SOURCES.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-23 09:56:13.000000 lions-1.2.1/lions.egg-info/dependency_links.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-23 09:56:13.000000 lions-1.2.1/lions.egg-info/entry_points.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-23 09:56:13.000000 lions-1.2.1/lions.egg-info/requires.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-23 09:56:13.000000 lions-1.2.1/lions.egg-info/top_level.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-23 09:56:13.243220 lions-1.2.1/setup.cfg
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-23 09:55:12.000000 lions-1.2.1/setup.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 09:56:13.241657 lions-1.2.1/tests/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.2.1/tests/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1609 2024-05-23 08:42:03.000000 lions-1.2.1/tests/test_cpp_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-23 08:42:03.000000 lions-1.2.1/tests/test_js_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-23 08:42:03.000000 lions-1.2.1/tests/test_lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-23 08:42:03.000000 lions-1.2.1/tests/test_yaml_parser.py
```

### Comparing `lions-1.2.0/LICENSE` & `lions-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lions-1.2.0/PKG-INFO` & `lions-1.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.2.0
+Version: 1.2.1
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -53,62 +53,38 @@
 
 ## Install
 
     $ pip install lions
 
 ## Usage
 
-    $ lions [msg_files_dir] [output_dir]
+    $ lions <msg_files_dir> <output_dir> <target_language>
 
 -   **msg_files_dir**: Directory containing your .lmsg.yaml files
 -   **output_dir**: Directory to place the generated code
+-   **target_language**: Target language for the generated code
+    -   cpp; c; js; ts; py
 
 ## Raw Message format
 
 The message structure is composed of a 6-byte header, followed by a variable-length payload. The payload length can range from 0 to 244 bytes, allowing for flexible data encapsulation. Fields within the payload are tightly packed, with no intervening spaces, to maximize message efficiency and minimize overhead.
 
 | Byte Index | Field    | Size (Bytes) | Description                                       |
 | ---------- | -------- | ------------ | ------------------------------------------------- |
 | 0          | src      | 1            | Source identifier                                 |
 | 1          | dst      | 1            | Destination identifier                            |
 | 2          | next_hop | 1            | Next hop identifier (used for message forwarding) |
 | 3          | msg_id   | 1            | Message identifier                                |
 | 4-5        | checksum | 2            | Checksum for error checking                       |
 | 6-249      | payload  | 244          | Actual data payload                               |
 
-### C++ representation
+### Raw Message code representation
 
-```C++
-struct Header {
-    uint8_t src;
-    uint8_t dst;
-    uint8_t next_hop;
-    uint8_t msg_id;
-
-    union{
-        uint16_t checksum;
-
-        struct{
-            uint8_t checksum_low;
-            uint8_t checksum_high;
-        };
-    };
-};
-
-class LMsg {
-   public:
-    Header header;
-    uint8_t payload[MAX_PAYLOAD_SIZE];
-    uint8_t payload_size;
-
-    LMsg(uint8_t payload_size = 0);
-    uint16_t calculate_checksum();
-    bool valid_checksum();
-};
-```
+-   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c++/generated_code/lions.hpp)
+-   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/lions.js)
 
 ## Defining Messages
 
 LIONS uses `.lmsg.yaml` files to define message specifications for IoT networks. Each file can contain multiple message definitions that are used by the LIONS compiler to generate C++ code for message handling.
 
 ### Structure of Message Files
 
@@ -157,71 +133,61 @@
 
 ping:
     id: 0x03
     period: 1000
     description: "Ping message"
 ```
 
-### Generated Code Overview
+### Generated Code
 
 The LIONS compiler auto-generates code to facilitate handling, encoding and decoding of messages defined in `.lmsg.yaml` files. Below is an example of how part of the generated code might look for the yaml file above.
 
 #### Constants
 
 The code defines namespaces to hold constants for message IDs and periods, ensuring easy reference throughout the codebase:
 
+C++ example:
+
 ```C++
 namespace msg_id {
     constexpr uint8_t ACCELEROMETER = 1;
     constexpr uint8_t MICROPHONE = 2;
     constexpr uint8_t PING = 3;
 }  // namespace msg_id
 
 namespace msg_period {
     constexpr uint8_t ACCELEROMETER = 1000;
     constexpr uint8_t MICROPHONE = 0;
     constexpr uint8_t PING = 1000;
 }  // namespace msg_period
 ```
 
-#### Message Class Structure
+#### Message Struct/Class
 
-For each message type defined in the YAML files, the LIONS compiler generates a corresponding C++ class. This class includes the specific fields of the message, two constructors, and an encode method.
+For each message type defined in the YAML files, the LIONS compiler generates a corresponding struct/class. This class includes the specific fields of the message, two constructors, and an encode method.
 
--   **Constructors**:
+1. **Initialization Constructor**
 
-    1. **Initialization Constructor**: Used to create a new instance of the message class with predefined field values. This constructor initializes the message with specific data relevant to its type.
-    2. **Decoding Constructor**: Transforms a generic, raw-form message (`LMsg`) into the structured format of the class. This conversion facilitates easier manipulation and interpretation of the message contents within the application.
+    - Used to create a new instance of the message class with predefined field values. This constructor initializes the message with specific data relevant to its type.
 
--   **Encode Method**: Converts the structured message back into its raw binary form (`LMsg`) for transmission. This method ensures that the message is properly packaged with its header and payload according to the protocol specifications before being sent over the network.
+2. **Decoding Constructor**
 
-```C++
-class AccelerometerMsg {
-   public:
-    Header header;  // Header as defined in the base LIONS framework
-
-    float acc_x;  // Acceleration in x-axis
-    float acc_y;  // Acceleration in y-axis
-    float acc_z;  // Acceleration in z-axis
-
-    /** Create a new accelerometer msg */
-    AccelerometerMsg(const float acc_x, const float acc_y, const float acc_z);
-
-    /** Decode LMsg to accelerometer msg */
-    AccelerometerMsg(const LMsg &msg);
-
-    /** Encode accelerometer msg to LMsg */
-    LMsg encode(const uint8_t src, const uint8_t dst, const uint8_t next_hop);
-};
+    - Transforms a generic, raw-form message (`LMsg`) into the structured format of the class. This conversion facilitates easier manipulation and interpretation of the message contents within the application.
 
-```
+3. **Encode Method**
+    - Converts the structured message back into its raw binary form (`LMsg`) for transmission. This method ensures that the message is properly packaged with its header and payload according to the protocol specifications before being sent over the network.
+
+---
+-   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c%2B%2B/generated_code/my_messages_lmsg.hpp)
+-   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/my_messages_lmsg.js)
 
 ## Examples
 
 [Examples](https://github.com/ItsNotSoftware/lions/tree/main/examples)
 
 ## Target language support
 
 -   [x] C++
+-   [x] JavaScript
+-   [ ] TypeScript
 -   [ ] C
--   [ ] JavaScript
 -   [ ] Python
```

### Comparing `lions-1.2.0/README.md` & `lions-1.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -32,62 +32,38 @@
 
 ## Install
 
     $ pip install lions
 
 ## Usage
 
-    $ lions [msg_files_dir] [output_dir]
+    $ lions <msg_files_dir> <output_dir> <target_language>
 
 -   **msg_files_dir**: Directory containing your .lmsg.yaml files
 -   **output_dir**: Directory to place the generated code
+-   **target_language**: Target language for the generated code
+    -   cpp; c; js; ts; py
 
 ## Raw Message format
 
 The message structure is composed of a 6-byte header, followed by a variable-length payload. The payload length can range from 0 to 244 bytes, allowing for flexible data encapsulation. Fields within the payload are tightly packed, with no intervening spaces, to maximize message efficiency and minimize overhead.
 
 | Byte Index | Field    | Size (Bytes) | Description                                       |
 | ---------- | -------- | ------------ | ------------------------------------------------- |
 | 0          | src      | 1            | Source identifier                                 |
 | 1          | dst      | 1            | Destination identifier                            |
 | 2          | next_hop | 1            | Next hop identifier (used for message forwarding) |
 | 3          | msg_id   | 1            | Message identifier                                |
 | 4-5        | checksum | 2            | Checksum for error checking                       |
 | 6-249      | payload  | 244          | Actual data payload                               |
 
-### C++ representation
+### Raw Message code representation
 
-```C++
-struct Header {
-    uint8_t src;
-    uint8_t dst;
-    uint8_t next_hop;
-    uint8_t msg_id;
-
-    union{
-        uint16_t checksum;
-
-        struct{
-            uint8_t checksum_low;
-            uint8_t checksum_high;
-        };
-    };
-};
-
-class LMsg {
-   public:
-    Header header;
-    uint8_t payload[MAX_PAYLOAD_SIZE];
-    uint8_t payload_size;
-
-    LMsg(uint8_t payload_size = 0);
-    uint16_t calculate_checksum();
-    bool valid_checksum();
-};
-```
+-   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c++/generated_code/lions.hpp)
+-   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/lions.js)
 
 ## Defining Messages
 
 LIONS uses `.lmsg.yaml` files to define message specifications for IoT networks. Each file can contain multiple message definitions that are used by the LIONS compiler to generate C++ code for message handling.
 
 ### Structure of Message Files
 
@@ -136,71 +112,61 @@
 
 ping:
     id: 0x03
     period: 1000
     description: "Ping message"
 ```
 
-### Generated Code Overview
+### Generated Code
 
 The LIONS compiler auto-generates code to facilitate handling, encoding and decoding of messages defined in `.lmsg.yaml` files. Below is an example of how part of the generated code might look for the yaml file above.
 
 #### Constants
 
 The code defines namespaces to hold constants for message IDs and periods, ensuring easy reference throughout the codebase:
 
+C++ example:
+
 ```C++
 namespace msg_id {
     constexpr uint8_t ACCELEROMETER = 1;
     constexpr uint8_t MICROPHONE = 2;
     constexpr uint8_t PING = 3;
 }  // namespace msg_id
 
 namespace msg_period {
     constexpr uint8_t ACCELEROMETER = 1000;
     constexpr uint8_t MICROPHONE = 0;
     constexpr uint8_t PING = 1000;
 }  // namespace msg_period
 ```
 
-#### Message Class Structure
+#### Message Struct/Class
 
-For each message type defined in the YAML files, the LIONS compiler generates a corresponding C++ class. This class includes the specific fields of the message, two constructors, and an encode method.
+For each message type defined in the YAML files, the LIONS compiler generates a corresponding struct/class. This class includes the specific fields of the message, two constructors, and an encode method.
 
--   **Constructors**:
+1. **Initialization Constructor**
 
-    1. **Initialization Constructor**: Used to create a new instance of the message class with predefined field values. This constructor initializes the message with specific data relevant to its type.
-    2. **Decoding Constructor**: Transforms a generic, raw-form message (`LMsg`) into the structured format of the class. This conversion facilitates easier manipulation and interpretation of the message contents within the application.
+    - Used to create a new instance of the message class with predefined field values. This constructor initializes the message with specific data relevant to its type.
 
--   **Encode Method**: Converts the structured message back into its raw binary form (`LMsg`) for transmission. This method ensures that the message is properly packaged with its header and payload according to the protocol specifications before being sent over the network.
+2. **Decoding Constructor**
 
-```C++
-class AccelerometerMsg {
-   public:
-    Header header;  // Header as defined in the base LIONS framework
-
-    float acc_x;  // Acceleration in x-axis
-    float acc_y;  // Acceleration in y-axis
-    float acc_z;  // Acceleration in z-axis
-
-    /** Create a new accelerometer msg */
-    AccelerometerMsg(const float acc_x, const float acc_y, const float acc_z);
-
-    /** Decode LMsg to accelerometer msg */
-    AccelerometerMsg(const LMsg &msg);
-
-    /** Encode accelerometer msg to LMsg */
-    LMsg encode(const uint8_t src, const uint8_t dst, const uint8_t next_hop);
-};
+    - Transforms a generic, raw-form message (`LMsg`) into the structured format of the class. This conversion facilitates easier manipulation and interpretation of the message contents within the application.
 
-```
+3. **Encode Method**
+    - Converts the structured message back into its raw binary form (`LMsg`) for transmission. This method ensures that the message is properly packaged with its header and payload according to the protocol specifications before being sent over the network.
+
+---
+-   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c%2B%2B/generated_code/my_messages_lmsg.hpp)
+-   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/my_messages_lmsg.js)
 
 ## Examples
 
 [Examples](https://github.com/ItsNotSoftware/lions/tree/main/examples)
 
 ## Target language support
 
 -   [x] C++
+-   [x] JavaScript
+-   [ ] TypeScript
 -   [ ] C
--   [ ] JavaScript
 -   [ ] Python
```

### Comparing `lions-1.2.0/lions/cpp_gen/cpp_generator.py` & `lions-1.2.1/lions/cpp_gen/cpp_generator.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.0/lions/cpp_gen/templates/lions.cpp.jinja` & `lions-1.2.1/lions/cpp_gen/templates/lions.cpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.2.0/lions/cpp_gen/templates/lions.hpp.jinja` & `lions-1.2.1/lions/cpp_gen/templates/lions.hpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.2.0/lions/cpp_gen/templates/msg.cpp.jinja` & `lions-1.2.1/lions/cpp_gen/templates/msg.cpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.2.0/lions/cpp_gen/templates/msg.hpp.jinja` & `lions-1.2.1/lions/cpp_gen/templates/msg.hpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.2.0/lions/errors.py` & `lions-1.2.1/lions/errors.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.0/lions/js_gen/js_generator.py` & `lions-1.2.1/lions/js_gen/js_generator.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.0/lions/lmsg.py` & `lions-1.2.1/lions/lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.0/lions/main.py` & `lions-1.2.1/lions/main.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.0/lions/yaml_parser.py` & `lions-1.2.1/lions/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.0/lions.egg-info/PKG-INFO` & `lions-1.2.1/lions.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.2.0
+Version: 1.2.1
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -53,62 +53,38 @@
 
 ## Install
 
     $ pip install lions
 
 ## Usage
 
-    $ lions [msg_files_dir] [output_dir]
+    $ lions <msg_files_dir> <output_dir> <target_language>
 
 -   **msg_files_dir**: Directory containing your .lmsg.yaml files
 -   **output_dir**: Directory to place the generated code
+-   **target_language**: Target language for the generated code
+    -   cpp; c; js; ts; py
 
 ## Raw Message format
 
 The message structure is composed of a 6-byte header, followed by a variable-length payload. The payload length can range from 0 to 244 bytes, allowing for flexible data encapsulation. Fields within the payload are tightly packed, with no intervening spaces, to maximize message efficiency and minimize overhead.
 
 | Byte Index | Field    | Size (Bytes) | Description                                       |
 | ---------- | -------- | ------------ | ------------------------------------------------- |
 | 0          | src      | 1            | Source identifier                                 |
 | 1          | dst      | 1            | Destination identifier                            |
 | 2          | next_hop | 1            | Next hop identifier (used for message forwarding) |
 | 3          | msg_id   | 1            | Message identifier                                |
 | 4-5        | checksum | 2            | Checksum for error checking                       |
 | 6-249      | payload  | 244          | Actual data payload                               |
 
-### C++ representation
+### Raw Message code representation
 
-```C++
-struct Header {
-    uint8_t src;
-    uint8_t dst;
-    uint8_t next_hop;
-    uint8_t msg_id;
-
-    union{
-        uint16_t checksum;
-
-        struct{
-            uint8_t checksum_low;
-            uint8_t checksum_high;
-        };
-    };
-};
-
-class LMsg {
-   public:
-    Header header;
-    uint8_t payload[MAX_PAYLOAD_SIZE];
-    uint8_t payload_size;
-
-    LMsg(uint8_t payload_size = 0);
-    uint16_t calculate_checksum();
-    bool valid_checksum();
-};
-```
+-   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c++/generated_code/lions.hpp)
+-   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/lions.js)
 
 ## Defining Messages
 
 LIONS uses `.lmsg.yaml` files to define message specifications for IoT networks. Each file can contain multiple message definitions that are used by the LIONS compiler to generate C++ code for message handling.
 
 ### Structure of Message Files
 
@@ -157,71 +133,61 @@
 
 ping:
     id: 0x03
     period: 1000
     description: "Ping message"
 ```
 
-### Generated Code Overview
+### Generated Code
 
 The LIONS compiler auto-generates code to facilitate handling, encoding and decoding of messages defined in `.lmsg.yaml` files. Below is an example of how part of the generated code might look for the yaml file above.
 
 #### Constants
 
 The code defines namespaces to hold constants for message IDs and periods, ensuring easy reference throughout the codebase:
 
+C++ example:
+
 ```C++
 namespace msg_id {
     constexpr uint8_t ACCELEROMETER = 1;
     constexpr uint8_t MICROPHONE = 2;
     constexpr uint8_t PING = 3;
 }  // namespace msg_id
 
 namespace msg_period {
     constexpr uint8_t ACCELEROMETER = 1000;
     constexpr uint8_t MICROPHONE = 0;
     constexpr uint8_t PING = 1000;
 }  // namespace msg_period
 ```
 
-#### Message Class Structure
+#### Message Struct/Class
 
-For each message type defined in the YAML files, the LIONS compiler generates a corresponding C++ class. This class includes the specific fields of the message, two constructors, and an encode method.
+For each message type defined in the YAML files, the LIONS compiler generates a corresponding struct/class. This class includes the specific fields of the message, two constructors, and an encode method.
 
--   **Constructors**:
+1. **Initialization Constructor**
 
-    1. **Initialization Constructor**: Used to create a new instance of the message class with predefined field values. This constructor initializes the message with specific data relevant to its type.
-    2. **Decoding Constructor**: Transforms a generic, raw-form message (`LMsg`) into the structured format of the class. This conversion facilitates easier manipulation and interpretation of the message contents within the application.
+    - Used to create a new instance of the message class with predefined field values. This constructor initializes the message with specific data relevant to its type.
 
--   **Encode Method**: Converts the structured message back into its raw binary form (`LMsg`) for transmission. This method ensures that the message is properly packaged with its header and payload according to the protocol specifications before being sent over the network.
+2. **Decoding Constructor**
 
-```C++
-class AccelerometerMsg {
-   public:
-    Header header;  // Header as defined in the base LIONS framework
-
-    float acc_x;  // Acceleration in x-axis
-    float acc_y;  // Acceleration in y-axis
-    float acc_z;  // Acceleration in z-axis
-
-    /** Create a new accelerometer msg */
-    AccelerometerMsg(const float acc_x, const float acc_y, const float acc_z);
-
-    /** Decode LMsg to accelerometer msg */
-    AccelerometerMsg(const LMsg &msg);
-
-    /** Encode accelerometer msg to LMsg */
-    LMsg encode(const uint8_t src, const uint8_t dst, const uint8_t next_hop);
-};
+    - Transforms a generic, raw-form message (`LMsg`) into the structured format of the class. This conversion facilitates easier manipulation and interpretation of the message contents within the application.
 
-```
+3. **Encode Method**
+    - Converts the structured message back into its raw binary form (`LMsg`) for transmission. This method ensures that the message is properly packaged with its header and payload according to the protocol specifications before being sent over the network.
+
+---
+-   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c%2B%2B/generated_code/my_messages_lmsg.hpp)
+-   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/my_messages_lmsg.js)
 
 ## Examples
 
 [Examples](https://github.com/ItsNotSoftware/lions/tree/main/examples)
 
 ## Target language support
 
 -   [x] C++
+-   [x] JavaScript
+-   [ ] TypeScript
 -   [ ] C
--   [ ] JavaScript
 -   [ ] Python
```

### Comparing `lions-1.2.0/lions.egg-info/SOURCES.txt` & `lions-1.2.1/lions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lions-1.2.0/setup.py` & `lions-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lions",
-    version="1.2.0",
+    version="1.2.1",
     author="Diogo Ferreira",
     author_email="itsnotsoftware@gmail.com",
     description="LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={"lions": ["cpp_gen/templates/*.jinja"]},
     url="https://github.com/ItsNotSoftware/lions",
```

### Comparing `lions-1.2.0/tests/test_cpp_gen.py` & `lions-1.2.1/tests/test_cpp_gen.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.0/tests/test_js_gen.py` & `lions-1.2.1/tests/test_js_gen.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.0/tests/test_lmsg.py` & `lions-1.2.1/tests/test_lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.2.0/tests/test_yaml_parser.py` & `lions-1.2.1/tests/test_yaml_parser.py`

 * *Files identical despite different names*

