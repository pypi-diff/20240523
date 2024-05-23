# Comparing `tmp/pyvns-2.1-cp312-cp312-win_amd64.whl.zip` & `tmp/pyvns-2.2-cp312-cp312-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 230785 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat    27030 b- defN 24-Feb-17 02:14 pyvns/LICENSE
--rw-rw-rw-  2.0 fat     6159 b- defN 24-Feb-17 02:14 pyvns/README.md
--rw-rw-rw-  2.0 fat    20992 b- defN 24-Feb-17 02:14 pyvns/__init__.cp312-win_amd64.pyd
--rw-rw-rw-  2.0 fat      132 b- defN 24-Feb-17 02:14 pyvns/__init__.pyi
--rw-rw-rw-  2.0 fat      119 b- defN 24-Feb-17 02:14 pyvns/py.typed
--rw-rw-rw-  2.0 fat   479744 b- defN 24-Feb-17 02:14 pyvns/vns_python_wrapper.cp312-win_amd64.pyd
--rw-rw-rw-  2.0 fat     9273 b- defN 24-Feb-14 06:04 pyvns/vns_python_wrapper.pyi
--rw-rw-rw-  2.0 fat       90 b- defN 24-Feb-16 20:57 pyvns/__pyinstaller/__init__.py
--rw-rw-rw-  2.0 fat      958 b- defN 24-Feb-17 02:14 pyvns/__pyinstaller/hook-pyvns.py
--rw-rw-rw-  2.0 fat    27030 b- defN 24-Feb-17 02:14 pyvns-2.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6902 b- defN 24-Feb-17 02:14 pyvns-2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-17 02:14 pyvns-2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       62 b- defN 24-Feb-17 02:14 pyvns-2.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-Feb-17 02:14 pyvns-2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1199 b- defN 24-Feb-17 02:14 pyvns-2.1.dist-info/RECORD
-15 files, 579788 bytes uncompressed, 228813 bytes compressed:  60.5%
+Zip file size: 398220 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat    27030 b- defN 24-May-23 21:50 pyvns/LICENSE
+-rw-rw-rw-  2.0 fat     3619 b- defN 24-May-23 21:50 pyvns/README.md
+-rw-rw-rw-  2.0 fat    25600 b- defN 24-May-23 21:50 pyvns/__init__.cp312-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      314 b- defN 24-May-23 21:50 pyvns/__init__.pyi
+-rw-rw-rw-  2.0 fat      119 b- defN 24-May-23 21:50 pyvns/py.typed
+-rw-rw-rw-  2.0 fat   873984 b- defN 24-May-23 21:50 pyvns/vns_python_wrapper.cp312-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    12310 b- defN 24-May-23 21:48 pyvns/vns_python_wrapper.pyi
+-rw-rw-rw-  2.0 fat       90 b- defN 24-May-22 19:18 pyvns/__pyinstaller/__init__.py
+-rw-rw-rw-  2.0 fat      958 b- defN 24-May-23 21:50 pyvns/__pyinstaller/hook-pyvns.py
+-rw-rw-rw-  2.0 fat    27030 b- defN 24-May-23 21:51 pyvns-2.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4362 b- defN 24-May-23 21:51 pyvns-2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 21:51 pyvns-2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       62 b- defN 24-May-23 21:51 pyvns-2.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-23 21:51 pyvns-2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1200 b- defN 24-May-23 21:51 pyvns-2.2.dist-info/RECORD
+15 files, 976776 bytes uncompressed, 396248 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: pyvns/__pyinstaller/__init__.py
 Comment: 
 
 Filename: pyvns/__pyinstaller/hook-pyvns.py
 Comment: 
 
-Filename: pyvns-2.1.dist-info/LICENSE
+Filename: pyvns-2.2.dist-info/LICENSE
 Comment: 
 
-Filename: pyvns-2.1.dist-info/METADATA
+Filename: pyvns-2.2.dist-info/METADATA
 Comment: 
 
-Filename: pyvns-2.1.dist-info/WHEEL
+Filename: pyvns-2.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyvns-2.1.dist-info/entry_points.txt
+Filename: pyvns-2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyvns-2.1.dist-info/top_level.txt
+Filename: pyvns-2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyvns-2.1.dist-info/RECORD
+Filename: pyvns-2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyvns/README.md

```diff
@@ -10,21 +10,21 @@
 
 Unlike Ren'py, writing visual novel script is more like writing a story instead of a program, and the developers also have the choice to create their own implementation.
 
 # How it started:
 
 The development of the VNS can be traced all the way back to the initial stages of Linpg's development. During this period, the team faced the challenge of finding an efficient method to store the dialogue. Each conversation required the storage of multiple variables, including the narrator, the actual dialogue content, associated character images, ambient background music, and various other components:
 
-![](doc/readme_conv_ex.png)
+![](vns-docs/docs/readme_conv_ex.png)
 
 Ultimately, the team opted for a design inspired by doubly linked list, but implemented using dictionary (HashMap for Java forks). This approach not only facilitated easier access to the data but also  streamlined the saving process, enabling compatibility with formats like JSON or YAML. This method preserved readability while efficiently  managing the dialogue. Today, the current system closely resembles our initial design, with only a few subtle refinements:
 
 ```yaml
-compiledAt: ...
-dialogs:
+compiler: ...
+dialogues:
   dialog1:
     head:
       background_image: bg1.jpg
       background_music: bgm1.mp3
       character_images:
       - alice.png
       contents:
@@ -55,129 +55,22 @@
 language: English
 ```
 
 Although the overall data is easy to read, it is somewhat inconvenient to write. We came up with a dedicated dialogue editor to resolve the issue, but it's still a bit of a hassle. That is the reason why we begin to inquire about the possibility of simplifying the process.
 
 Would it be possible to make it feel like we're writing the dialogue in a Microsoft Word document? Thus, VNS is born.
 
-# Tutorials:
-
-VNS are written in a plain text file with the `.vns` extension. The script file contains a series of tags, which are used to specify the different elements of the visual novel, such as the characters, backgrounds, dialogue, music, and so on.
-
-## Tags with value
-
-`[tag]value`
-
-The `[tag]` represents the kind of value you are trying to represent, and the value is, well, the value. 
-
-### ID:
-
-`[id]str`, ex: `[id]1`
-
-Specifies a (unique) ID for the current dialogue file. Every script file must have an ID.
-
-### Language:
-
-`[language]str`, ex: `[language]English`
-
-Specifies the language of the current dialogue. Every script file must specifies a language.
-
-### Section:
-
-`[section]str`, ex: `[section]dialog_example`
-
-Specifies the section of all the following dialogues.
-
-### Background image:
-
-`[bgi]str`, ex: `[bgi]bg1.png`
-
-Specifies the background image for the current and following dialogues.
-
-### Background music:
-
-`[bgm]str`, ex: `[bgm]bgm1.ogg`
-
-Specifies the background music for the current and following dialogues.
-
-### Display character(s)
-
-`[display]*str`, ex: `[display]character1.png character2.png`
-
-Displays the character(s) for the current and following dialogues.
-
-### Hide character(s)
-
-`[hide]*str`, ex: `[hide]character1.png character2.png` or `[hide]*` for hiding all.
-
-Hides the character(s) for the current and following dialogues.
-
-### New scene
-
-`[scene]str`, ex: `[scene]bg2.png`
-
-Enters a new scene and displays the specified background image.
-
-### Option(s)
-
-`[option]message->label`, ex: `[scene]Can you hear me?->yes_reply`
-
-Adding option(s) to current dialogues, and branch to the specified label according to the option chosen by the player. 
-
-### Label
-
-`[label]str`, ex: `[label]jump_point1`
-
-Creates a label for the branch command. The value will be used as the key for the subsequent conversation.
-
-## Tags without value
-
-### End
-
-`[end]`
-
-Marks the end of the script.
-
-### **Block**
-
-`[block]`
-
-The player can't go back to the previous conversation.
-
-### Comments:
-
-`# this is a comment`
-
-Commenting the script to make it easier to understand.
-
-### Notes:
-
-`// this is a note`
-
-Notes are very similar to comments. It's used to make a note for a specific conversation and is saved to the file that is compiled.
-
-## Dialogue:
-
-Conversations are written in the form of this:
-
-```vns
-Character name:
-- Dialogue text
-- More dialogue text
-```
-
-The character name is followed by a colon and then one or more lines of dialogue text. Each line of dialogue text must start with a hyphen and a space.
-
 ## **Example**:
 
 Here is a simple example of a VNS script:
 
 ```vns
 [id]1
 [language]English
+
 [section]dialog_example
 
 [bgi]bg1.png
 [display]character1.png character2.png
 
 Mabel:
 - Hello my name is Mabel!
@@ -187,12 +80,16 @@
 
 Dipper:
 - Hi Mabel! I'm doing well, thanks for asking.
 ```
 
 This script would display the background image `bg1.png` and the character images `character1.png` and `character2.png`. Mabel would then say "Hello my name is Mabel!" and "How are you doing today!". Next, `character1.png` would be hidden and Dipper would say "Hi Mabel! I'm doing well, thanks for asking." Finally, the script would end.
 
+# Wiki:
+
+If you would like to learn more about VNS, please visit [**vsn.wiki**](https://vns.wiki/).
+
 # License:
 
 VNS is licensed under **LGPL(GNU Lesser General Public License)-2.1-or-later**.
 
 See **[LICENSE](https://github.com/LinpgFoundation/vns/blob/main/LICENSE)**.
```

## pyvns/__init__.pyi

```diff
@@ -1 +1,6 @@
-from .vns_python_wrapper import Compiler as Compiler, Dialogue as Dialogue, DialoguesManager as DialoguesManager, Naming as Naming
+from .vns_python_wrapper import Compiler as Compiler, Dialogue as Dialogue, DialoguesManager as DialoguesManager, Event as Event, Naming as Naming
+from _typeshed import Incomplete
+
+dialogue_data_t: Incomplete
+dialogue_section_t = dict[str, dialogue_data_t]
+dialogue_content_t = dict[str, dialogue_section_t]
```

## pyvns/vns_python_wrapper.pyi

```diff
@@ -2,30 +2,45 @@
 Python bindings for the VNS C++ library
 """
 
 from __future__ import annotations
 
 import typing
 
-__all__ = ["Compiler", "Dialogue", "DialogueNext", "DialoguesManager", "Naming"]
+__all__ = [
+    "Compiler",
+    "Dialogue",
+    "DialogueNext",
+    "DialoguesManager",
+    "Event",
+    "Naming",
+    "Validator",
+]
 
 class Compiler:
     """
     Compiler for compiling vns files
     """
 
     @staticmethod
     def load(
         arg0: str,
     ) -> dict[
         str,
         dict[
             str,
             dict[
-                str, dict[str, str | list[str] | dict[str, str | list[dict[str, str]]]]
+                str,
+                dict[
+                    str,
+                    str
+                    | list[str]
+                    | dict[str, str | list[dict[str, str]]]
+                    | list[dict[str, bool | int | float | str]],
+                ],
             ],
         ]
         | dict[str, int]
         | str,
     ]:
         """
         Load a vns file
@@ -35,60 +50,85 @@
     """
     Class representing dialogue content
     """
 
     background_image: str
     background_music: str
     character_images: list[str]
-    comments: list[str]
     contents: list[str]
     id: str
     narrator: str
     next: DialogueNext
+    notes: list[str]
     previous: str
     def __init__(
         self,
-        arg0: dict[str, str | list[str] | dict[str, str | list[dict[str, str]]]],
-        arg1: str,
+        arg0: str,
+        arg1: dict[
+            str,
+            str
+            | list[str]
+            | dict[str, str | list[dict[str, str]]]
+            | list[dict[str, bool | int | float | str]],
+        ],
     ) -> None: ...
     def has_next(self) -> bool:
         """
         Check if the dialogue has next
         """
 
+    def remove_next(self) -> None:
+        """
+        Remove dialogue next
+        """
+
     @typing.overload
     def set_next(self, arg0: str, arg1: str | list[dict[str, str]]) -> None:
         """
         Set dialogue next
         """
 
     @typing.overload
     def set_next(self, arg0: dict[str, str | list[dict[str, str]]]) -> None:
         """
         Set dialogue next
         """
 
-    def to_map(
+    def to_dict(
         self,
-    ) -> dict[str, str | list[str] | dict[str, str | list[dict[str, str]]]]:
+    ) -> dict[
+        str,
+        str
+        | list[str]
+        | dict[str, str | list[dict[str, str]]]
+        | list[dict[str, bool | int | float | str]],
+    ]:
         """
-        Convert the dialogue object to a map
+        Convert the dialogue object to a dict
         """
 
+    @property
+    def events(self) -> list[Event]: ...
+
 class DialogueNext:
     """
     Class for representing the dialogue next
     """
 
     @typing.overload
     def __init__(self, arg0: str, arg1: str | list[dict[str, str]]) -> None: ...
     @typing.overload
     def __init__(self, arg0: dict[str, str | list[dict[str, str]]]) -> None:
         """
-        Initialize a ContentNext object from a map
+        Initialize a ContentNext object from a dict
+        """
+
+    def contains_target(self, arg0: str) -> bool:
+        """
+        Check if the next is/contains given target
         """
 
     def get_target(self) -> str:
         """
         Get the target of the next
         """
 
@@ -108,22 +148,27 @@
         """
 
     def has_single_target(self) -> bool:
         """
         Check if the next has a single target
         """
 
+    def has_type(self, arg0: str) -> bool:
+        """
+        Whether the next has given type
+        """
+
     def is_null(self) -> bool:
         """
         Check if the next is null
         """
 
-    def to_map(self) -> dict[str, str | list[dict[str, str]]]:
+    def to_dict(self) -> dict[str, str | list[dict[str, str]]]:
         """
-        Convert the next object to a map
+        Convert the next object to a dict
         """
 
 class DialoguesManager:
     """
     Class for managing dialogue contents
     """
 
@@ -139,85 +184,97 @@
         """
 
     def contains_section(self, arg0: str) -> bool:
         """
         Check if dialogues have given section name
         """
 
+    def contains_variable(self, arg0: str) -> bool:
+        """
+        Contains variable
+        """
+
     def empty(self) -> bool:
         """
         Check if data is empty
         """
 
+    def get_bool_variable(self, arg0: str) -> bool:
+        """
+        Get variable as bool
+        """
+
     def get_current(self) -> Dialogue:
         """
         Get current dialogue
         """
 
-    def get_current_dialogue(
-        self,
-    ) -> dict[str, str | list[str] | dict[str, str | list[dict[str, str]]]]:
+    def get_current_dialogue_id(self) -> str:
         """
-        Get current dialogue data
+        Get current dialogue ID
         """
 
-    def get_current_section_dialogues(
-        self,
-    ) -> dict[str, dict[str, str | list[str] | dict[str, str | list[dict[str, str]]]]]:
+    def get_current_section_dialogues(self) -> dict[str, Dialogue]:
         """
         Get current section dialogue contents
         """
 
-    def get_data(
-        self,
-    ) -> dict[
-        str,
-        dict[str, dict[str, str | list[str] | dict[str, str | list[dict[str, str]]]]],
-    ]:
+    def get_dialogue(self, arg0: str, arg1: str) -> Dialogue:
         """
-        Get data
+        Get dialogue data by ID
         """
 
-    def get_dialogue(
-        self, arg0: str, arg1: str
-    ) -> dict[str, str | list[str] | dict[str, str | list[dict[str, str]]]]:
+    def get_dialogues(self, arg0: str) -> dict[str, Dialogue]:
         """
-        Get dialogue data by ID
+        Get current dialogue data
         """
 
-    def get_id(self) -> str:
+    def get_float_variable(self, arg0: str) -> float:
         """
-        Get current dialogue ID
+        Get variable as float
         """
 
-    def get_last(self) -> Dialogue:
+    def get_int_variable(self, arg0: str) -> int:
         """
-        Get last dialogue
+        Get variable as int
         """
 
     def get_previous(self) -> Dialogue:
         """
         Get previous dialogue
         """
 
     def get_section(self) -> str:
         """
         Get current section name
         """
 
-    def get_section_dialogues(
-        self, arg0: str
-    ) -> dict[str, dict[str, str | list[str] | dict[str, str | list[dict[str, str]]]]]:
+    def get_sections(self) -> set[str]:
         """
-        Get section dialogue contents by section name
+        Get the names of all sections
         """
 
-    def get_sections(self) -> set[str]:
+    def get_str_variable(self, arg0: str) -> str:
         """
-        Get the names of all sections
+        Get variable as str
+        """
+
+    def get_variable(self, arg0: str) -> bool | int | float | str:
+        """
+        Get variable
+        """
+
+    def load(self, arg0: str) -> None:
+        """
+        load dialogue data from vns file
+        """
+
+    def next(self) -> None:
+        """
+        Go to next dialogue
         """
 
     def remove_current_dialogue(self) -> None:
         """
         Remove current dialogue
         """
 
@@ -227,80 +284,150 @@
         """
 
     def remove_section(self, arg0: str) -> None:
         """
         Remove section
         """
 
-    def save(self) -> None:
-        """
-        Save modifications to the current dialogue interface
-        """
-
     def set_current_dialogue(
-        self, arg0: dict[str, str | list[str] | dict[str, str | list[dict[str, str]]]]
+        self,
+        arg0: dict[
+            str,
+            str
+            | list[str]
+            | dict[str, str | list[dict[str, str]]]
+            | list[dict[str, bool | int | float | str]],
+        ],
     ) -> None:
         """
         Set current dialogue data
         """
 
-    def set_current_section_dialogues(
-        self,
-        arg0: dict[
-            str, dict[str, str | list[str] | dict[str, str | list[dict[str, str]]]]
-        ],
-    ) -> None:
+    def set_current_dialogue_id(self, arg0: str) -> None:
         """
-        Set current section dialogue contents
+        Set current dialogue ID
         """
 
-    def set_data(
+    def set_current_section_dialogues(
         self,
         arg0: dict[
             str,
             dict[
-                str, dict[str, str | list[str] | dict[str, str | list[dict[str, str]]]]
+                str,
+                str
+                | list[str]
+                | dict[str, str | list[dict[str, str]]]
+                | list[dict[str, bool | int | float | str]],
             ],
         ],
     ) -> None:
         """
-        Update data
+        Set current section dialogue contents
         """
 
     def set_dialogue(
         self,
         arg0: str,
         arg1: str,
-        arg2: dict[str, str | list[str] | dict[str, str | list[dict[str, str]]]],
+        arg2: dict[
+            str,
+            str
+            | list[str]
+            | dict[str, str | list[dict[str, str]]]
+            | list[dict[str, bool | int | float | str]],
+        ],
     ) -> None:
         """
         Set current dialogue data by ID
         """
 
-    def set_id(self, arg0: str) -> None:
+    def set_dialogues(
+        self,
+        arg0: str,
+        arg1: dict[
+            str,
+            dict[
+                str,
+                str
+                | list[str]
+                | dict[str, str | list[dict[str, str]]]
+                | list[dict[str, bool | int | float | str]],
+            ],
+        ],
+    ) -> None:
         """
-        Set current dialogue ID
+        Set section dialogue contents by section name
         """
 
     def set_section(self, arg0: str) -> None:
         """
         Set current section name
         """
 
-    def set_section_dialogues(
+    def set_variable(self, arg0: str, arg1: bool | int | float | str) -> None:
+        """
+        Set variable
+        """
+
+    def to_dict(
         self,
-        arg0: str,
-        arg1: dict[
-            str, dict[str, str | list[str] | dict[str, str | list[dict[str, str]]]]
+    ) -> dict[
+        str,
+        dict[
+            str,
+            dict[
+                str,
+                str
+                | list[str]
+                | dict[str, str | list[dict[str, str]]]
+                | list[dict[str, bool | int | float | str]],
+            ],
+        ],
+    ]:
+        """
+        Get data in dict
+        """
+
+    def update(
+        self,
+        arg0: dict[
+            str,
+            dict[
+                str,
+                dict[
+                    str,
+                    str
+                    | list[str]
+                    | dict[str, str | list[dict[str, str]]]
+                    | list[dict[str, bool | int | float | str]],
+                ],
+            ],
         ],
     ) -> None:
         """
-        Set section dialogue contents by section name
+        Update data
         """
 
+class Event:
+    """
+    Class for representing the event struct
+    """
+
+    @typing.overload
+    def __init__(
+        self, arg0: str, arg1: str, arg2: bool | int | float | str
+    ) -> None: ...
+    @typing.overload
+    def __init__(self, arg0: dict[str, bool | int | float | str]) -> None: ...
+    def to_dict(self) -> dict[str, bool | int | float | str]: ...
+    @property
+    def target(self) -> str: ...
+    @property
+    def type(self) -> str: ...
+
 class Naming:
     """
     Character name preprocessing module
     """
 
     @staticmethod
     def clear_database() -> None:
@@ -321,22 +448,22 @@
         Update the character naming database from a JSON string
         """
 
     @staticmethod
     @typing.overload
     def update_database(arg0: dict[str, set[str]]) -> None:
         """
-        Update the character naming database from a map of names and sets of tags
+        Update the character naming database from a dict of names and sets of tags
         """
 
     @staticmethod
     @typing.overload
     def update_database(arg0: dict[str, list[str]]) -> None:
         """
-        Update the character naming database from a map of names and vectors of tags
+        Update the character naming database from a dict of names and vectors of tags
         """
 
     def __init__(self, arg0: str) -> None: ...
     def contains_tag(self, arg0: str) -> bool:
         """
         Check if the name contains a tag
         """
@@ -385,7 +512,24 @@
         Insert a tag to the name
         """
 
     def to_string(self) -> str:
         """
         Retrieve naming as string
         """
+
+class Validator:
+    """
+    Class for validating vns format json file
+    """
+
+    @staticmethod
+    def ensure(arg0: str) -> None:
+        """
+        Ensure a JSON file is valid VSN format, throw error if not
+        """
+
+    @staticmethod
+    def validate(arg0: str) -> bool:
+        """
+        Validate a JSON file against VSN format dialogues
+        """
```

## Comparing `pyvns-2.1.dist-info/LICENSE` & `pyvns-2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyvns-2.1.dist-info/RECORD` & `pyvns-2.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 pyvns/LICENSE,sha256=f_4ZVFh8d9-6HPjrmy6nQ2cfpuY_nnovJYEZ1C4U7v4,27030
-pyvns/README.md,sha256=Ni_A0dJN7RDt57f2CEIDkTDZg9jHAjrMQ6qKVjnJDs0,6159
-pyvns/__init__.cp312-win_amd64.pyd,sha256=iVMB2HzjUYV5Jo1oa6Kff7h0O9YSevyUU9byt5nG0uo,20992
-pyvns/__init__.pyi,sha256=k-AA40-xMwsewQfWVKqrN7KwWRB99ifEM_4HRHofi-s,132
+pyvns/README.md,sha256=M2kXXzSJX0RiQR9hXLdtiI_Y7B-ZLAUHuw4dM1ugHa0,3619
+pyvns/__init__.cp312-win_amd64.pyd,sha256=W6k7qH2C88piJnIW12sib62D-9d7AhT-K59gyh30xEs,25600
+pyvns/__init__.pyi,sha256=YwniB4sGQ64eWMu1dJ5OBbVULBfPdwbzN7Kbph_sP54,314
 pyvns/py.typed,sha256=BKGW85xUbIOdsH0WSMC5AssR6pudZXjdlzx9DOXLmD8,119
-pyvns/vns_python_wrapper.cp312-win_amd64.pyd,sha256=QwraRLogbOZea4-dlVodlCWYYwacfGSB-rY6RYBx-uE,479744
-pyvns/vns_python_wrapper.pyi,sha256=5wVZ2ulXrOUPueT4Cl50nP84p7EuQfMFvZpvkSEuc2o,9273
+pyvns/vns_python_wrapper.cp312-win_amd64.pyd,sha256=oDs-XS-_CRWkixCvzo-KAmLfM1GFfG7G3g66UQdPRRU,873984
+pyvns/vns_python_wrapper.pyi,sha256=mu52ZmXzRlf63bRIhvmZ0JHuR-RoKcY8UVclFr9GwsA,12310
 pyvns/__pyinstaller/__init__.py,sha256=bqrSMt3YYOZGCGfWJmVuXNV5C6EyRMxN9BowgZHgHKk,90
 pyvns/__pyinstaller/hook-pyvns.py,sha256=JVn_7Pe9-gSGem667xB-upV6cFePneVFV4S0MEfiVF4,958
-pyvns-2.1.dist-info/LICENSE,sha256=f_4ZVFh8d9-6HPjrmy6nQ2cfpuY_nnovJYEZ1C4U7v4,27030
-pyvns-2.1.dist-info/METADATA,sha256=K5h-_X17ktVZzPWwS8e3FKpwYglS15CYCrpj4MiSeDM,6902
-pyvns-2.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-pyvns-2.1.dist-info/entry_points.txt,sha256=AZT6SILopvb_7x8jlIiH1FsdEoojBPo8b6FGy_VfdGM,62
-pyvns-2.1.dist-info/top_level.txt,sha256=77EmcIhXvwvuP3z0eOUfe4La0IwQb8OLFpW9ihqqBYg,6
-pyvns-2.1.dist-info/RECORD,,
+pyvns-2.2.dist-info/LICENSE,sha256=f_4ZVFh8d9-6HPjrmy6nQ2cfpuY_nnovJYEZ1C4U7v4,27030
+pyvns-2.2.dist-info/METADATA,sha256=75fKZu6Hx7oEDl4ytj1mrG2r3cPGen3cxRTzm54UNC4,4362
+pyvns-2.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyvns-2.2.dist-info/entry_points.txt,sha256=AZT6SILopvb_7x8jlIiH1FsdEoojBPo8b6FGy_VfdGM,62
+pyvns-2.2.dist-info/top_level.txt,sha256=77EmcIhXvwvuP3z0eOUfe4La0IwQb8OLFpW9ihqqBYg,6
+pyvns-2.2.dist-info/RECORD,,
```

