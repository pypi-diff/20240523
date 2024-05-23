# Comparing `tmp/lions-1.1.2.tar.gz` & `tmp/lions-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lions-1.1.2.tar", last modified: Mon May 13 15:21:09 2024, max compression
+gzip compressed data, was "lions-1.2.0.tar", last modified: Thu May 23 08:51:03 2024, max compression
```

## Comparing `lions-1.1.2.tar` & `lions-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:21:09.315620 lions-1.1.2/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.1.2/LICENSE
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8244 2024-05-13 15:21:09.315429 lions-1.1.2/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)     7391 2024-05-13 15:15:40.000000 lions-1.1.2/README.md
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:21:09.311858 lions-1.1.2/lions/
--rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.1.2/lions/__init__.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:21:09.313011 lions-1.1.2/lions/cpp_gen/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.1.2/lions/cpp_gen/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2709 2024-05-13 14:07:26.000000 lions-1.1.2/lions/cpp_gen/cpp_generator.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:21:09.313999 lions-1.1.2/lions/cpp_gen/templates/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1202 2024-05-13 14:58:05.000000 lions-1.1.2/lions/cpp_gen/templates/lions.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1125 2024-05-13 15:10:01.000000 lions-1.1.2/lions/cpp_gen/templates/lions.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2221 2024-05-13 14:34:59.000000 lions-1.1.2/lions/cpp_gen/templates/msg.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-13 15:20:38.000000 lions-1.1.2/lions/cpp_gen/templates/msg.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3175 2024-05-10 09:08:10.000000 lions-1.1.2/lions/errors.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.1.2/lions/lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2444 2024-05-08 16:10:12.000000 lions-1.1.2/lions/main.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.1.2/lions/yaml_parser.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:21:09.312803 lions-1.1.2/lions.egg-info/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8244 2024-05-13 15:21:09.000000 lions-1.1.2/lions.egg-info/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)      593 2024-05-13 15:21:09.000000 lions-1.1.2/lions.egg-info/SOURCES.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-13 15:21:09.000000 lions-1.1.2/lions.egg-info/dependency_links.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-13 15:21:09.000000 lions-1.1.2/lions.egg-info/entry_points.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-13 15:21:09.000000 lions-1.1.2/lions.egg-info/requires.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-13 15:21:09.000000 lions-1.1.2/lions.egg-info/top_level.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-13 15:21:09.315844 lions-1.1.2/setup.cfg
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-13 15:21:00.000000 lions-1.1.2/setup.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-13 15:21:09.314731 lions-1.1.2/tests/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.1.2/tests/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1353 2024-05-08 14:15:59.000000 lions-1.1.2/tests/test_cpp_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-08 16:10:12.000000 lions-1.1.2/tests/test_lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-10 09:08:10.000000 lions-1.1.2/tests/test_yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:51:03.368620 lions-1.2.0/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.2.0/LICENSE
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8244 2024-05-23 08:51:03.368493 lions-1.2.0/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     7391 2024-05-22 12:07:18.000000 lions-1.2.0/README.md
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:51:03.364705 lions-1.2.0/lions/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.2.0/lions/__init__.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:51:03.365796 lions-1.2.0/lions/cpp_gen/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.2.0/lions/cpp_gen/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2705 2024-05-23 08:42:03.000000 lions-1.2.0/lions/cpp_gen/cpp_generator.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:51:03.366825 lions-1.2.0/lions/cpp_gen/templates/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1202 2024-05-22 12:07:18.000000 lions-1.2.0/lions/cpp_gen/templates/lions.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1125 2024-05-22 12:07:18.000000 lions-1.2.0/lions/cpp_gen/templates/lions.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2218 2024-05-23 08:42:03.000000 lions-1.2.0/lions/cpp_gen/templates/msg.cpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1519 2024-05-23 08:42:03.000000 lions-1.2.0/lions/cpp_gen/templates/msg.hpp.jinja
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3480 2024-05-23 08:42:03.000000 lions-1.2.0/lions/errors.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:51:03.367108 lions-1.2.0/lions/js_gen/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:42:03.000000 lions-1.2.0/lions/js_gen/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2780 2024-05-23 08:42:03.000000 lions-1.2.0/lions/js_gen/js_generator.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     5199 2024-05-08 16:10:12.000000 lions-1.2.0/lions/lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3023 2024-05-23 08:42:03.000000 lions-1.2.0/lions/main.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.2.0/lions/yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:51:03.365593 lions-1.2.0/lions.egg-info/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8244 2024-05-23 08:51:03.000000 lions-1.2.0/lions.egg-info/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)      668 2024-05-23 08:51:03.000000 lions-1.2.0/lions.egg-info/SOURCES.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-23 08:51:03.000000 lions-1.2.0/lions.egg-info/dependency_links.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-23 08:51:03.000000 lions-1.2.0/lions.egg-info/entry_points.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-23 08:51:03.000000 lions-1.2.0/lions.egg-info/requires.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-23 08:51:03.000000 lions-1.2.0/lions.egg-info/top_level.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-23 08:51:03.368818 lions-1.2.0/setup.cfg
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-23 08:42:03.000000 lions-1.2.0/setup.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:51:03.367964 lions-1.2.0/tests/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.2.0/tests/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1609 2024-05-23 08:42:03.000000 lions-1.2.0/tests/test_cpp_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-23 08:42:03.000000 lions-1.2.0/tests/test_js_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-23 08:42:03.000000 lions-1.2.0/tests/test_lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-23 08:42:03.000000 lions-1.2.0/tests/test_yaml_parser.py
```

### Comparing `lions-1.1.2/LICENSE` & `lions-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lions-1.1.2/PKG-INFO` & `lions-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.1.2
+Version: 1.2.0
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lions-1.1.2/README.md` & `lions-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lions-1.1.2/lions/cpp_gen/cpp_generator.py` & `lions-1.2.0/lions/cpp_gen/cpp_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,17 @@
         jinja_dict = {"filename": filename, "msgs": msgs}
 
         for msg in msgs:
             for field in msg.fields:
                 if field.type == "string":
                     field.type = "std::string"
 
-        with open(f"{file}_lmsgs.hpp", "w") as f_hpp, open(
-            f"{file}_lmsgs.cpp", "w"
+        with open(f"{file}_lmsg.hpp", "w") as f_hpp, open(
+            f"{file}_lmsg.cpp", "w"
         ) as f_cpp:
             # hpp
             f_hpp.write(self.msg_hpp_template.render(jinja_dict))
-            print_generation_status(self.output_dir, f"{filename}_lmsgs.hpp")
+            print_generation_status(self.output_dir, f"{filename}_lmsg.hpp")
 
             # cpp
             f_cpp.write(self.msg_cpp_template.render(jinja_dict))
-            print_generation_status(self.output_dir, f"{filename}_lmsgs.cpp\n")
+            print_generation_status(self.output_dir, f"{filename}_lmsg.cpp\n")
```

### Comparing `lions-1.1.2/lions/cpp_gen/templates/lions.cpp.jinja` & `lions-1.2.0/lions/cpp_gen/templates/lions.cpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.1.2/lions/cpp_gen/templates/lions.hpp.jinja` & `lions-1.2.0/lions/cpp_gen/templates/lions.hpp.jinja`

 * *Files identical despite different names*

### Comparing `lions-1.1.2/lions/cpp_gen/templates/msg.cpp.jinja` & `lions-1.2.0/lions/cpp_gen/templates/msg.cpp.jinja`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 /**
- * @file {{filename}}_lmsgs.cpp
+ * @file {{filename}}_lmsg.cpp
  *
- * @brief Implementation of {{filename}}_lmsgs.hpp Classes
+ * @brief Implementation of {{filename}}_lmsg.hpp Classes
  * 
  * This file contains the implementation of the message classes generated by the Lions Compiler.
  * 
  * @details
  * This file was generated by the Lions Compiler (https://github.com/ItsNotSoftware/lions) on {{date}}.
  * Modifying this file manually is not recommended as it may lead to unexpected behavior.
  * 
  * @note
  * Generated files should not be manually edited.
  * 
  * @author Lions Compiler
 */
 
-#include "{{filename}}_lmsgs.hpp"
+#include "{{filename}}_lmsg.hpp"
 
 #include <algorithm>
 #include <utility>
 
 namespace lions {
 {% for msg in msgs %} 
 {{ msg.name | capitalize }}Msg::{{ msg.name | capitalize }}Msg({% for field in msg.fields %}const {{ field.type }} {{ field.name }}{% if not loop.last %}, {% endif %}{% endfor %})
```

### Comparing `lions-1.1.2/lions/cpp_gen/templates/msg.hpp.jinja` & `lions-1.2.0/lions/cpp_gen/templates/msg.hpp.jinja`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 /**
- * @file {{filename}}_lmsgs.hpp
+ * @file {{filename}}_lmsg.hpp
  *
- * @brief {{filename}}_lmsgs Classes
+ * @brief {{filename}}_lmsg Classes
  * 
  * This file contains the declaration of the message classes generated by the Lions Compiler.
  * 
  * @details
  * This file was generated by the Lions Compiler (https://github.com/ItsNotSoftware/lions) on {{date}}.
  * Modifying this file manually is not recommended as it may lead to unexpected behavior.
  * 
  * @note
  * Generated files should not be manually edited.
  * 
  * @author Lions Compiler
 */
 
-#ifndef {{filename | upper}}_LMSGS_HPP
-#define {{filename | upper}}_LMSGS_HPP
+#ifndef {{filename | upper}}_LMSG_HPP
+#define {{filename | upper}}_LMSG_HPP
 
 #include "lions.hpp"
 #include <string>
 
 
 namespace lions {
 
-   namespace msg_id {
-{% for msg in msgs %}   constexpr uint8_t {{msg.name|upper}} = {{msg.id}};
-{% endfor %}   }  // namespace msg_id
+namespace msg_id {
+{% for msg in msgs %}constexpr uint8_t {{msg.name|upper}} = {{msg.id}};
+{% endfor %}}  // namespace msg_id
    
-   namespace msg_period {
-{% for msg in msgs %}   constexpr uint32_t {{msg.name|upper}} = {{msg.period}};
-{% endfor %}   }  // namespace msg_period
+namespace msg_period {
+{% for msg in msgs %}constexpr uint32_t {{msg.name|upper}} = {{msg.period}};
+{% endfor %}}  // namespace msg_period
 
 {% for msg in msgs %}
 class {{msg.name | capitalize }}Msg {
-   public:
-    Header header;
-    {% for field in msg.fields %}
-    {{field.type}} {{field.name}};{% endfor %}
+  public:
+   Header header;
+   {% for field in msg.fields %}
+   {{field.type}} {{field.name}};{% endfor %}
     
-    /** Create a new {{msg.name}} msg */
-    {{ msg.name | capitalize }}Msg({% for field in msg.fields %}const {{ field.type }} {{ field.name }}{% if not loop.last %}, {% endif %}{% endfor %});
+   /** Create a new {{msg.name}} msg */
+   {{ msg.name | capitalize }}Msg({% for field in msg.fields %}const {{ field.type }} {{ field.name }}{% if not loop.last %}, {% endif %}{% endfor %});
     
-    /** Decode LMsg to {{msg.name}} msg */
-    {{msg.name | capitalize}}Msg(const LMsg &msg); 
+   /** Decode LMsg to {{msg.name}} msg */
+   {{msg.name | capitalize}}Msg(const LMsg &msg); 
     
-    /** Encode {{msg.name}} msg to LMsg */
-    LMsg encode(const uint8_t src, const uint8_t dst, const uint8_t next_hop);
+   /** Encode {{msg.name}} msg to LMsg */
+   LMsg encode(const uint8_t src, const uint8_t dst, const uint8_t next_hop);
 };
 {% endfor %}
 
 }  // namespace lions
 
 #endif
```

### Comparing `lions-1.1.2/lions/errors.py` & `lions-1.2.0/lions/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,7 +89,15 @@
 
 class MsgFilesNotFoundError(Exception):
     """Exception raised when the message file is not found."""
 
     def __init__(self, dir):
         message = f'Error: No ".lmsg.yaml" files found in the directory "{dir}".'
         super().__init__(Fore.RED + message)
+
+
+class InvalidTargetLanguageError(Exception):
+    """Exception raised when the target language is invalid."""
+
+    def __init__(self, target_language):
+        message = f'Error: Invalid target language "{target_language}". Supported languages: "cpp", "js".'
+        super().__init__(Fore.RED + message)
```

### Comparing `lions-1.1.2/lions/lmsg.py` & `lions-1.2.0/lions/lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.1.2/lions/main.py` & `lions-1.2.0/lions/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 
 License:
     Copyright (c) 2024 Diogo Ferreira. All rights reserved.
     This code is licensed under the MIT License.
 """
 
 import sys
+import colorama
 from lions.cpp_gen.cpp_generator import CppGenerator
 from lions.yaml_parser import YamlParser
-import colorama
 from colorama import Fore, Style
+from lions.js_gen.js_generator import JsGenerator
+from lions.errors import InvalidTargetLanguageError
 
 
 def print_title():
     """Function to print title of the program in ASCII art"""
 
     print(Fore.GREEN)
 
@@ -47,25 +49,43 @@
     print(Fore.GREEN + "+" + "-" * (len(success_message) + 2) + "+" + Style.RESET_ALL)
 
 
 def main():
     colorama.init(autoreset=True)
 
     # Check if the number of arguments is correct
-    if len(sys.argv) != 3:
-        print("Usage: lions <msg_files_dir> <output_dir>")
+    if len(sys.argv) != 4:
+        print("Usage: lions <msg_files_dir> <output_dir> <target_language>")
+
+        # targert language help
+        print(
+            """
+    Target Language:
+        cpp - C++
+        js - JavaScript
+        """
+        )
+
         sys.exit(1)
 
     msg_files_dir = sys.argv[1]
     output_dir = sys.argv[2]
 
     print_title()
 
     # Initialize the parser and generator objects
     parser = YamlParser(msg_files_dir)
-    cpp_generator = CppGenerator(output_dir)
+    code_generator = None
+
+    # Check the target language and initialize the corresponding code generator
+    if sys.argv[3] == "c++" or sys.argv[3] == "cpp":
+        code_generator = CppGenerator(output_dir)
+    elif sys.argv[3] == "js":
+        code_generator = JsGenerator(output_dir)
+    else:
+        raise InvalidTargetLanguageError(sys.argv[3])
 
     # Parse the message files and generate the corresponding C++ files
     for filename, msgs in parser.parse_file():
-        cpp_generator.generate_msg_files(filename, msgs)
+        code_generator.generate_msg_files(filename, msgs)
 
     print_success_message()
```

### Comparing `lions-1.1.2/lions/yaml_parser.py` & `lions-1.2.0/lions/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `lions-1.1.2/lions.egg-info/PKG-INFO` & `lions-1.2.0/lions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.1.2
+Version: 1.2.0
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lions-1.1.2/lions.egg-info/SOURCES.txt` & `lions-1.2.0/lions.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -15,11 +15,14 @@
 lions.egg-info/top_level.txt
 lions/cpp_gen/__init__.py
 lions/cpp_gen/cpp_generator.py
 lions/cpp_gen/templates/lions.cpp.jinja
 lions/cpp_gen/templates/lions.hpp.jinja
 lions/cpp_gen/templates/msg.cpp.jinja
 lions/cpp_gen/templates/msg.hpp.jinja
+lions/js_gen/__init__.py
+lions/js_gen/js_generator.py
 tests/__init__.py
 tests/test_cpp_gen.py
+tests/test_js_gen.py
 tests/test_lmsg.py
 tests/test_yaml_parser.py
```

### Comparing `lions-1.1.2/setup.py` & `lions-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lions",
-    version="1.1.2",
+    version="1.2.0",
     author="Diogo Ferreira",
     author_email="itsnotsoftware@gmail.com",
     description="LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={"lions": ["cpp_gen/templates/*.jinja"]},
     url="https://github.com/ItsNotSoftware/lions",
```

### Comparing `lions-1.1.2/tests/test_lmsg.py` & `lions-1.2.0/tests/test_lmsg.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pytest
 from lions.lmsg import LMsg, MsgField, _used_ids, _used_names
 from lions.errors import *
 
 
 def reset(func):
     def wrapper(*args, **kwargs):
-        result = func(*args, **kwargs)
         _used_ids.clear()
         _used_names.clear()
+        result = func(*args, **kwargs)
         return result
 
     return wrapper
 
 
 # Test valid LMsg creation
 @reset
```

### Comparing `lions-1.1.2/tests/test_yaml_parser.py` & `lions-1.2.0/tests/test_yaml_parser.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from lions.yaml_parser import YamlParser
 from lions.lmsg import LMsg, MsgField, _used_ids, _used_names
 from lions.errors import *
 
 
 def reset(func):
     def wrapper(*args, **kwargs):
-        result = func(*args, **kwargs)
         _used_ids.clear()
         _used_names.clear()
+        result = func(*args, **kwargs)
         return result
 
     return wrapper
 
 
 @reset
 def test_invalid_dir():
```

