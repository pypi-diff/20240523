# Comparing `tmp/linkedit-1.0.4.tar.gz` & `tmp/linkedit-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedit-1.0.4.tar", last modified: Mon May 20 22:03:21 2024, max compression
+gzip compressed data, was "linkedit-1.0.5.tar", last modified: Thu May 23 15:49:44 2024, max compression
```

## Comparing `linkedit-1.0.4.tar` & `linkedit-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-20 22:03:21.227932 linkedit-1.0.4/
--rw-r--r--   0 khiat     (1000) khiat     (1000)    71475 2024-05-20 22:03:21.227932 linkedit-1.0.4/PKG-INFO
--rw-rw-r--   0 khiat     (1000) khiat     (1000)    71021 2024-05-20 21:58:55.000000 linkedit-1.0.4/README.md
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-20 22:03:21.227932 linkedit-1.0.4/linkedit/
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      280 2024-05-19 17:39:14.000000 linkedit-1.0.4/linkedit/__init__.py
--rw-r--r--   0 khiat     (1000) khiat     (1000)   100341 2024-05-20 22:01:42.000000 linkedit-1.0.4/linkedit/linkedit.py
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-20 22:03:21.227932 linkedit-1.0.4/linkedit.egg-info/
--rw-r--r--   0 khiat     (1000) khiat     (1000)    71475 2024-05-20 22:03:21.000000 linkedit-1.0.4/linkedit.egg-info/PKG-INFO
--rw-r--r--   0 khiat     (1000) khiat     (1000)      219 2024-05-20 22:03:21.000000 linkedit-1.0.4/linkedit.egg-info/SOURCES.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-20 22:03:21.000000 linkedit-1.0.4/linkedit.egg-info/dependency_links.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       16 2024-05-20 22:03:21.000000 linkedit-1.0.4/linkedit.egg-info/requires.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        9 2024-05-20 22:03:21.000000 linkedit-1.0.4/linkedit.egg-info/top_level.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-20 22:03:21.227932 linkedit-1.0.4/setup.cfg
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      721 2024-05-20 21:54:11.000000 linkedit-1.0.4/setup.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 15:49:44.963789 linkedit-1.0.5/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)    71475 2024-05-23 15:49:44.963789 linkedit-1.0.5/PKG-INFO
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)    71021 2024-05-20 21:58:54.000000 linkedit-1.0.5/README.md
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 15:49:44.963789 linkedit-1.0.5/linkedit/
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)   110724 2024-05-23 15:48:09.000000 linkedit-1.0.5/linkedit/__init__.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 15:49:44.963789 linkedit-1.0.5/linkedit.egg-info/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)    71475 2024-05-23 15:49:44.000000 linkedit-1.0.5/linkedit.egg-info/PKG-INFO
+-rw-r--r--   0 khiat     (1000) khiat     (1000)      198 2024-05-23 15:49:44.000000 linkedit-1.0.5/linkedit.egg-info/SOURCES.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-23 15:49:44.000000 linkedit-1.0.5/linkedit.egg-info/dependency_links.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       16 2024-05-23 15:49:44.000000 linkedit-1.0.5/linkedit.egg-info/requires.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        9 2024-05-23 15:49:44.000000 linkedit-1.0.5/linkedit.egg-info/top_level.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-23 15:49:44.963789 linkedit-1.0.5/setup.cfg
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      721 2024-05-23 15:49:04.000000 linkedit-1.0.5/setup.py
```

### Comparing `linkedit-1.0.4/PKG-INFO` & `linkedit-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedit
-Version: 1.0.4
+Version: 1.0.5
 Summary: Sophisticate Linked List
 Home-page: https://pypi.org/project/linkedit/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: linked list
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linkedit-1.0.4/README.md` & `linkedit-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `linkedit-1.0.4/linkedit/linkedit.py` & `linkedit-1.0.5/linkedit/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,196 +16,342 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Khiat Mohammed Abderrezzak <khiat.abderrezzak@gmail.com>
 
+
 """Sophisticate Linked List"""
 
+
+__all__ = [
+    "singlyLinkedList",
+    "sll",
+    "doublyLinkedList",
+    "dll",
+    "orthogonalLinkedList",
+    "oll",
+]
+
+
 from tabulate import tabulate
 
 
-def red(text: str) -> str:
+def _red(text: str) -> str:
     """Red Coloring Function"""
     return "\033[91;1m{}\033[00m".format(text)
 
 
-def green(text: str) -> str:
+def _green(text: str) -> str:
     """Green Coloring Function"""
     return "\033[92;1m{}\033[00m".format(text)
 
 
-def yellow(text: str) -> str:
+def _yellow(text: str) -> str:
     """Yellow Coloring Function"""
     return "\033[93;1m{}\033[00m".format(text)
 
 
-def blue(text: str) -> str:
+def _blue(text: str) -> str:
     """Blue Coloring Function"""
     return "\033[94;1m{}\033[00m".format(text)
 
 
-def cyan(text: str) -> str:
+def _cyan(text: str) -> str:
     """Cyan Coloring Function"""
     return "\033[36;1m{}\033[00m".format(text)
 
 
-def white(text: str) -> str:
+def _white(text: str) -> str:
     """White Coloring Function"""
     return "\033[37;1m{}\033[00m".format(text)
 
 
 # for the background coloring
-BG_RED: str = "\033[41m"
-RESET: str = "\033[0m"
+_BG_RED: str = "\033[41m"
+_RESET: str = "\033[0m"
+
+
+class singlyLinkedListNode:
+    def __init__(
+        self: "singlyLinkedListNode",
+        data: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
+    ) -> None:
+        self.data: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ) = data
+        self.next: singlyLinkedListNode | None = None
+
+    def get_data(
+        self: "singlyLinkedListNode",
+    ) -> object | int | float | complex | str | list | tuple | set | dict | None | bool:
+        return self.data
+
+    def next_node(self: "singlyLinkedListNode") -> "singlyLinkedListNode":
+        return self.next
+
+
+class doublyLinkedListNode:
+    def __init__(
+        self: "doublyLinkedListNode",
+        data: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
+    ) -> None:
+        self.data: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ) = data
+        self.prev: doublyLinkedListNode | None = None
+        self.next: doublyLinkedListNode | None = None
 
+    def get_data(
+        self: "doublyLinkedListNode",
+    ) -> object | int | float | complex | str | list | tuple | set | dict | None | bool:
+        return self.data
 
-class linkedList:
+    def prev_node(self: "doublyLinkedListNode") -> "doublyLinkedListNode":
+        return self.prev
+
+    def next_node(self: "doublyLinkedListNode") -> "doublyLinkedListNode":
+        return self.next
+
+
+class _linkedList:
     def __init__(
-        self: "linkedList",
-        data: int | float | complex | str | list | tuple | set | dict | None = None,
+        self: object,
+        data: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ) = None,
         *,
         circular: bool = False,
         detail: bool = False,
         base: int = 16,
         reverse: bool = False,
     ) -> None:
         """constructor special method"""
         self.circular: bool = circular
         self.detail: bool = detail
         if self.detail:
             self.base: int = base
         else:
             # if detail is not true we assign directely the default base 16 hexa
-            self._base: int = base
+            self._base: int = 16
         # O(1) len (track the object)
         self.len: int = 0
-        self._tail: object | None = None
-        self.head: object | None = data
+        self._tail: singlyLinkedListNode | doublyLinkedListNode | None = None
+        self.head: singlyLinkedListNode | doublyLinkedListNode | None = data
         self.rev: bool = reverse
 
-    def __len__(self: "linkedList") -> int:
+    def __len__(self: object) -> int:
         """length special method"""
         return self.len
 
     def __contains__(
-        self: "linkedList",
-        item: int | float | complex | str | list | tuple | set | dict | None,
+        self: object,
+        item: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> bool:
-        head = self._head
+        head: singlyLinkedListNode | doublyLinkedListNode = self._head
         for _ in range(self.len):
             if head.data == item:
                 return True
-            head = head.next
+            head: object | None = head.next
         return False
 
-    def __mul__(self: "linkedList", other: int) -> None:
+    def __mul__(self: object, other: int) -> object:
         if not isinstance(other, int):
             raise ValueError("Unsupported operand type for *")
-        if self.isEmpty:
+        if self.isEmpty():
             for _ in range(other):
                 self.append(None)
-            return self
         else:
             length = self.len
             for _ in range(other - 1):
-                head = self._head
+                head: singlyLinkedListNode | doublyLinkedListNode = self._head
                 for _ in range(length):
                     self.append(head.data)
                     head = head.next
-            return self
+        return self
 
     def __setitem__(
-        self: "linkedList",
+        self: object,
         index: int,
-        value: int | float | complex | str | list | tuple | set | dict | None,
+        value: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> None:
         self.node(index).data = value
 
-    def __eq__(self, other) -> bool:
+    def __eq__(
+        self: object,
+        other: object,
+    ) -> bool:
         if isinstance(other, singlyLinkedList) or isinstance(other, doublyLinkedList):
             if id(self) == id(other):
                 return True
             elif len(self) != len(other):
                 return False
             elif len(self) == 0 and len(other) == 0:
                 return True
             else:
-                head1 = self._head
-                head2 = other._head
+                head1: singlyLinkedListNode | doublyLinkedListNode = self._head
+                head2: singlyLinkedListNode | doublyLinkedListNode = other._head
                 for _ in range(len(self)):
                     if head1.data == head2.data:
                         pass
                     else:
                         return False
-                    head1 = head1.next
-                    head2 = head2.next
+                    head1: singlyLinkedListNode | doublyLinkedListNode | None = (
+                        head1.next
+                    )
+                    head2: singlyLinkedListNode | doublyLinkedListNode | None = (
+                        head2.next
+                    )
                 return True
         else:
             return False
 
-    def __gt__(self, other) -> bool:
+    def __gt__(
+        self: object,
+        other: object,
+    ) -> bool:
         if isinstance(other, singlyLinkedList) or isinstance(other, doublyLinkedList):
             return len(self) > len(other)
         else:
             raise TypeError(
                 f"'>' not supported between instances of '{type(self).__name__}' and '{type(other).__name__}'"
             )
 
-    def __ge__(self, other) -> bool:
+    def __ge__(
+        self: object,
+        other: object,
+    ) -> bool:
         if isinstance(other, singlyLinkedList) or isinstance(other, doublyLinkedList):
             return len(self) >= len(other)
         else:
             raise TypeError(
                 f"'>=' not supported between instances of '{type(self).__name__}' and '{type(other).__name__}'"
             )
 
     @property
-    def base(self: "linkedList") -> int:
+    def base(self: object) -> int:
         """base getter"""
         return self._base
 
     @base.setter
-    def base(self: "linkedList", base: int) -> None:
+    def base(self: object, base: int) -> None:
         """base setter"""
         valid_bases: list = [2, 8, 10, 16]
         if not isinstance(base, int):
             # if the base is not an integer we keep the default base 16 hexa
             self._base: int = 16
             print(
-                red("Warning")
-                + white(" : Base must be integer, ")
-                + red(f"{type(base)} ")
-                + white("object not valid")
+                _red("Warning")
+                + _white(" : Base must be integer, ")
+                + _red(f"{type(base)} ")
+                + _white("object not valid")
             )
         else:
             if base not in valid_bases:
                 # if the base is not a valid base integer we keep the default base 16 hexa
                 self._base: int = 16
                 print(
-                    red("Warning")
-                    + white(" : Base must be one of these ")
-                    + green("[")
-                    + blue("2")
-                    + white(", ")
-                    + blue("8")
-                    + white(", ")
-                    + blue("10")
-                    + white(", ")
-                    + blue("16")
-                    + green("]")
-                    + white(", ")
-                    + red(f"{base} ")
-                    + white("not a valid base")
+                    _red("Warning")
+                    + _white(" : Base must be one of these ")
+                    + _green("[")
+                    + _blue("2")
+                    + _white(", ")
+                    + _blue("8")
+                    + _white(", ")
+                    + _blue("10")
+                    + _white(", ")
+                    + _blue("16")
+                    + _green("]")
+                    + _white(", ")
+                    + _red(f"{base} ")
+                    + _white("not a valid base")
                 )
             else:
                 self._base: int = base
 
-    def node(self: "linkedList", index: int) -> object:
+    def node(self: object, index: int) -> singlyLinkedListNode | doublyLinkedListNode:
         """node(s) searching method"""
         if not isinstance(index, int):
             if not self.circular:
                 raise TypeError(
                     "non circular singly linked list indices must be integers"
                 )
             else:
@@ -227,267 +373,297 @@
                             raise IndexError(
                                 "non circular singly linked list index out of range"
                             )
                         else:
                             raise IndexError(
                                 "circular singly linked list index out of range"
                             )
-                head: object = self._head
+                head: singlyLinkedListNode | doublyLinkedListNode = self._head
                 if index == self.len - 1:
                     return self._tail
                 for _ in range(index):
-                    head: object | None = head.next
+                    head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
                 return head
 
     @property
     def tail(
-        self: "linkedList",
-    ) -> int | float | complex | str | list | tuple | set | dict | None:
-        try:
-            return self._tail
-        except AttributeError as e1:
-            pass
-        if not self.circular:
-            raise TypeError("Empty non circular singly linked list")
-        else:
-            raise TypeError("Empty circular singly linked list")
+        self: object,
+    ) -> singlyLinkedListNode | doublyLinkedListNode:
+        return self._tail
 
     @tail.deleter
-    def tail(self: "linkedList") -> None:
+    def tail(self: object) -> None:
         self._tail = None
 
-    def isEmpty(self: "linkedList") -> bool:
+    def isEmpty(self: object) -> bool:
         return not self._head
 
     def index(
-        self: "linkedList",
-        value: int | float | complex | str | list | tuple | set | dict | None,
+        self: object,
+        value: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> int:
         """Return first index of value.
 
         Raises ValueError if the value is not present."""
-        head: object | None = self._head
+        head: singlyLinkedListNode | doublyLinkedListNode | None = self._head
         for i in range(self.len):
             if head.data == value:
                 return i
-            head: object | None = head.next
+            head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
         if not self.circular:
             error_msg: str = f"{value} is not in the non circular linked list"
             raise ValueError(error_msg)
         else:
             error_msg: str = f"{value} is not in the circular linked list"
             raise ValueError(error_msg)
 
-    def clear(self: "linkedList") -> None:
+    def clear(self: object) -> None:
         self._head: None = None
         self._tail: None = None
         self.len: int = 0
 
     def append(
-        self: "linkedList",
-        data: int | float | complex | str | list | tuple | set | dict | None,
+        self: object,
+        data: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> None:
         """Append object to the end of the linked list."""
         self.insert(self.len, data)
 
     def remove(
-        self: "linkedList",
-        value: int | float | complex | str | list | tuple | set | dict | None,
+        self: object,
+        value: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> None:
         """Remove first occurrence of value.
 
         Raises ValueError if the value is not present."""
         node_index: int = self.index(value)
         try:
             self.pop(node_index)
             return
-        except IndexError as e2:
+        except IndexError as e0:
             pass
         if not self.circular:
             error_msg: str = f"{value} not in the non circular singly linked list"
             raise ValueError(error_msg)
         else:
             error_msg: str = f"{value} not in the circular singly linked list"
             raise ValueError(error_msg)
 
     # O(n log n) sort (Tim Sort => hybrid sorting algorithm = Merge Sort + Insertion Sort)
-    def sort(self: "linkedList", *, reverse: bool = False) -> None:
+    def sort(self: object, *, reverse: bool = False) -> None:
         """Sort the linked list in ascending order and return None.
 
         The sort is in-place (i.e. the linked list itself is modified) and stable (i.e. the order of two equal elements is maintained).
 
         If a key function is given, apply it once to each linked list item and sort them, ascending or descending, according to their function values.
 
         The reverse flag can be set to sort in descending order."""
         non_sorted_list: list = []
-        head: object | None = self._head
+        head: singlyLinkedListNode | doublyLinkedListNode | None = self._head
         if self.len >= 1:
             for _ in range(self.len - 1):
                 if type(head.data) == type(head.next.data):
                     non_sorted_list.append(head.data)
-                    head: object | None = head.next
+                    head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
                 else:
                     raise TypeError(
                         f"'<' not supported between instances of '{type(head.data).__name__}' and '{type(head.next.data).__name__}'"
                     )
             non_sorted_list.append(head.data)
             non_sorted_list.sort(reverse=reverse)
-            head: object = self._head
+            head: singlyLinkedListNode | doublyLinkedListNode = self._head
             for i in range(self.len):
                 head.data = non_sorted_list[i]
-                head: object | None = head.next
+                head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
 
     def count(
-        self: "linkedList",
-        value: int | float | complex | str | list | tuple | set | dict | None,
+        self: object,
+        value: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> int:
         """Return number of occurrences of value."""
-        head: object | None = self._head
+        head: singlyLinkedListNode | doublyLinkedListNode | None = self._head
         counter: int = 0
         if self.len >= 1:
             for _ in range(self.len):
                 if head.data == value:
                     counter += 1
-                head: object | None = head.next
+                head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
             return counter
 
-    def reverse(self: "linkedList") -> None:
-        head: object | None = self._head
-        elements: list = []
-        for _ in range(self.len):
-            elements.append(head.data)
-            head: object | None = head.next
-        head: object | None = self._head
-        for i in range(1, self.len + 1):
-            head.data = elements[-i]
-            head: object | None = head.next
-
-    def right_shift(self: "linkedList", rotate: int) -> None:
+    def right_shift(self: object, rotate: int) -> None:
         if not isinstance(rotate, int):
             raise TypeError("rotate must be an integer")
         helper1: list = []
         helper2: list = []
-        head: object | None = self._head
+        head: singlyLinkedListNode | doublyLinkedListNode | None = self._head
         try:
             rotate: int = rotate % self.len
-        except ZeroDivisionError as e3:
+        except ZeroDivisionError as e1:
             return
         for _ in range(self.len - rotate):
             helper1.append(head.data)
-            head: object | None = head.next
+            head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
         for _ in range(self.len - rotate, self.len):
             helper2.append(head.data)
-            head: object | None = head.next
-        head: object | None = self._head
+            head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
+        head: singlyLinkedListNode | doublyLinkedListNode | None = self._head
         helper2.extend(helper1)
         for i in range(self.len):
             head.data = helper2[i]
-            head: object | None = head.next
+            head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
 
-    def left_shift(self: "linkedList", rotate: int) -> None:
+    def left_shift(self: object, rotate: int) -> None:
         if not isinstance(rotate, int):
             raise TypeError("rotate must be an integer")
         helper1: list = []
         helper2: list = []
-        head: object | None = self._head
+        head: singlyLinkedListNode | doublyLinkedListNode | None = self._head
         try:
             rotate: int = rotate % self.len
-        except ZeroDivisionError as e4:
+        except ZeroDivisionError as e2:
             return
         for _ in range(rotate):
             helper1.append(head.data)
-            head: object | None = head.next
+            head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
         for _ in range(rotate, self.len):
             helper2.append(head.data)
-            head: object | None = head.next
+            head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
         head: object | None = self._head
         helper2.extend(helper1)
         for i in range(self.len):
             head.data = helper2[i]
-            head: object | None = head.next
+            head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
 
     def prepend(
-        self: "linkedList",
-        data: int | float | complex | str | list | tuple | set | dict | None,
+        self: object,
+        data: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> None:
         self.insert(0, data)
 
 
-class singlyLinkedListNode:
-    def __init__(
-        self: "singlyLinkedListNode",
-        data: int | float | complex | str | list | tuple | set | dict | None,
-    ) -> object:
-        self.data: int | float | complex | str | list | tuple | set | dict | None = data
-        self.next: object | None = None
-
-    def get_data(
-        self: "singlyLinkedListNode",
-    ) -> int | float | complex | str | list | tuple | set | dict | None:
-        return self.data
-
-    def next_node(self: "singlyLinkedListNode") -> object:
-        return self.next
-
-
-class singlyLinkedList(linkedList):
+class singlyLinkedList(_linkedList):
     @property
     def head(
         self: "singlyLinkedList",
-    ) -> int | float | complex | str | list | tuple | set | dict | None:
-        try:
-            return self._head
-        except AttributeError as e5:
-            pass
-        if not self.circular:
-            raise TypeError("Empty non circular singly linked list")
-        else:
-            raise TypeError("Empty circular singly linked list")
+    ) -> singlyLinkedListNode:
+        return self._head
 
     @head.setter
     def head(
         self: "singlyLinkedList",
-        data: int | float | str | complex | list | tuple | set | dict | None,
+        data: (
+            object
+            | int
+            | float
+            | str
+            | complex
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> None:
         self._head: None = None
         if isinstance(data, singlyLinkedList):
-            self._head: object | None = data._head
+            self._head: singlyLinkedListNode | None = data._head
         elif isinstance(data, singlyLinkedListNode):
-            old_head: object = data
-            old_self_head: object = data
-            new_head: object = singlyLinkedListNode(data.data)
-            self._head: object = new_head
+            old_head: singlyLinkedListNode = data
+            old_self_head: singlyLinkedListNode = data
+            new_head: singlyLinkedListNode = singlyLinkedListNode(data.data)
+            self._head: singlyLinkedListNode = new_head
             self.len += 1
-            old_head: object | None = old_head.next
+            old_head: singlyLinkedListNode | None = old_head.next
             while old_head and old_head != old_self_head:
-                new_node: object = singlyLinkedListNode(old_head.data)
+                new_node: singlyLinkedListNode = singlyLinkedListNode(old_head.data)
                 self.len += 1
                 new_head.next = new_node
-                new_head: object | None = new_head.next
-                old_head: object | None = old_head.next
+                new_head: singlyLinkedListNode | None = new_head.next
+                old_head: singlyLinkedListNode | None = old_head.next
             if self.circular:
                 new_node.next = self._head
-            self._tail: object = new_node
+            self._tail: singlyLinkedListNode = new_node
         else:
             try:
                 if len(data) > 0:
                     for i in data:
                         self.append(i)
-            except TypeError as e6:
+            except TypeError as e3:
                 if data is not None:
-                    new_node: object = singlyLinkedListNode(data)
+                    new_node: singlyLinkedListNode = singlyLinkedListNode(data)
                     self.len += 1
-                    self._head: object = new_node
+                    self._head: singlyLinkedListNode = new_node
                     if self.circular:
                         new_node.next = new_node
-                    self._tail: object = new_node
+                    self._tail: singlyLinkedListNode = new_node
 
     @head.deleter
     def head(self: "singlyLinkedList") -> None:
-        self._head = None
+        self._head: None = None
 
     def copy(self: "singlyLinkedList") -> "singlyLinkedList":
         """Return a shallow copy of the non circular/circular singly linked list."""
         return singlyLinkedList(
             self._head,
             detail=self.detail,
             circular=self.circular,
@@ -500,54 +676,66 @@
 
     def set_non_circular(self: "singlyLinkedList") -> None:
         self._tail.next = None
         self.circular: bool = False
 
     def __add__(
         self: "singlyLinkedList",
-        other: object | int | float | complex | str | list | tuple | set | dict | None,
+        other: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> None:
         helper: list = []
-        head1: object | None = self._head
+        head1: singlyLinkedListNode | None = self._head
         if isinstance(other, singlyLinkedList) or isinstance(other, doublyLinkedList):
-            head2: object | None = other._head
+            head2: singlyLinkedListNode | None = other._head
         else:
-            other: object = singlyLinkedList(other)
-            head2: object = other._head
+            other: singlyLinkedList = singlyLinkedList(other)
+            head2: singlyLinkedListNode = other._head
         for _ in range(self.len):
             helper.append(head1.data)
-            head1: object | None = head1.next
+            head1: singlyLinkedListNode | None = head1.next
         for _ in range(other.len):
             helper.append(head2.data)
-            head2: object | None = head2.next
+            head2: singlyLinkedListNode | None = head2.next
         return singlyLinkedList(helper, circular=other.circular)
 
     def __str__(self: "singlyLinkedList") -> str:
         """Return str(self)."""
         if not self._head:
             if not self.circular:
                 raise TypeError("Empty non circular singly linked list")
             else:
                 raise TypeError("Empty circular singly linked list")
         else:
-            head: object = self._head
+            head: singlyLinkedListNode = self._head
             linked_list: list = []
             counter: int = 0
             if not self.detail:
                 while head and head.next != self._head:
                     if isinstance(head.data, str):
                         if len(head.data) == 0:
                             linked_list.append(f"[{head.data}] -> ")
                         elif len(head.data) == 1:
                             linked_list.append(f"['{head.data}'] -> ")
                         else:
                             linked_list.append(f'["{head.data}"] -> ')
                     else:
                         linked_list.append(f"[{head.data}] -> ")
-                    head: object | None = head.next
+                    head: singlyLinkedListNode | None = head.next
                 if not self.circular:
                     linked_list.append("None (NULL)")
                 else:
                     linked_list.insert(0, "> ")
                     if isinstance(head.data, str):
                         if len(head.data) == 0:
                             linked_list.append(f"[{head.data}]")
@@ -558,489 +746,562 @@
                     else:
                         linked_list.append(f"[{head.data}]")
                     linked_list.append(" -")
                 return "".join(linked_list)
             else:
                 linked_list.append(
                     [
-                        white("current value"),
-                        white("current value ") + green("@") + white("ddress"),
-                        white("next value"),
-                        white("next value ") + green("@") + white("ddress"),
+                        _white("current value"),
+                        _white("current value ") + _green("@") + _white("ddress"),
+                        _white("next value"),
+                        _white("next value ") + _green("@") + _white("ddress"),
                     ]
                 )
                 if head.next == self._head:
                     linked_list.append(
                         [
                             (
-                                blue(f"{head.data}")
+                                _blue(f"{head.data}")
                                 if not isinstance(head.data, str)
                                 else (
-                                    blue(f"'{head.data}'")
+                                    _blue(f"'{head.data}'")
                                     if len(head.data) == 1
                                     else (
-                                        blue(f'"{head.data}"')
+                                        _blue(f'"{head.data}"')
                                         if len(head.data) > 1
                                         else f"{head.data}"
                                     )
                                 )
                             ),
-                            cyan(
+                            _cyan(
                                 f"{bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head))}"
                             ),
                             (
-                                blue(f"{head.next.data}")
+                                _blue(f"{head.next.data}")
                                 if not isinstance(head.next.data, str)
                                 else (
-                                    blue(f"'{head.next.data}'")
+                                    _blue(f"'{head.next.data}'")
                                     if len(head.next.data) == 1
                                     else (
-                                        blue(f'"{head.next.data}"')
+                                        _blue(f'"{head.next.data}"')
                                         if len(head.next.data) > 1
                                         else f"{head.next.data}"
                                     )
                                 )
                             ),
-                            cyan(
+                            _cyan(
                                 f"{bin(id(head.next)) if self._base == 2 else oct(id(head.next)) if self._base == 8 else id(head.next) if self._base == 10 else hex(id(head.next))}"
                             ),
                         ]
                     )
                 elif not head.next:
                     linked_list.append(
                         [
                             (
-                                blue(f"{head.data}")
+                                _blue(f"{head.data}")
                                 if not isinstance(head.data, str)
                                 else (
-                                    blue(f"'{head.data}'")
+                                    _blue(f"'{head.data}'")
                                     if len(head.data) == 1
                                     else (
-                                        blue(f'"{head.data}"')
+                                        _blue(f'"{head.data}"')
                                         if len(head.data) > 1
                                         else f"{head.data}"
                                     )
                                 )
                             ),
-                            cyan(
+                            _cyan(
                                 f"{bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head))}"
                             ),
-                            f"{blue('None')} {green('(')}{red('NULL')}{green(')')}",
-                            yellow(
+                            f"{_blue('None')} {_green('(')}{_red('NULL')}{_green(')')}",
+                            _yellow(
                                 f"{bin(id(head.next)) if self._base == 2 else oct(id(head.next)) if self._base == 8 else id(head.next) if self._base == 10 else hex(id(head.next))} "
                             )
-                            + white("(")
-                            + red("nil")
-                            + white("/")
+                            + _white("(")
+                            + _red("nil")
+                            + _white("/")
                             + (
-                                red("0b0")
+                                _red("0b0")
                                 if self._base == 2
                                 else (
-                                    red("0o0")
+                                    _red("0o0")
                                     if self._base == 8
-                                    else (red("0") if self._base == 10 else red("0x0"))
+                                    else (
+                                        _red("0") if self._base == 10 else _red("0x0")
+                                    )
                                 )
                             )
-                            + white(")"),
+                            + _white(")"),
                         ]
                     )
-                    head: object | None = head.next
+                    head: singlyLinkedListNode | None = head.next
                 else:
                     linked_list.append(
                         [
                             (
-                                blue(f"{head.data}")
+                                _blue(f"{head.data}")
                                 if not isinstance(head.data, str)
                                 else (
-                                    blue(f"'{head.data}'")
+                                    _blue(f"'{head.data}'")
                                     if len(head.data) == 1
                                     else (
-                                        blue(f'"{head.data}"')
+                                        _blue(f'"{head.data}"')
                                         if len(head.data) > 1
                                         else f"{head.data}"
                                     )
                                 )
                             ),
-                            f"{cyan(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))}",
+                            f"{_cyan(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))}",
                             (
-                                blue(f"{head.next.data}")
+                                _blue(f"{head.next.data}")
                                 if not isinstance(head.next.data, str)
                                 else (
-                                    blue(f"'{head.next.data}'")
+                                    _blue(f"'{head.next.data}'")
                                     if len(head.next.data) == 1
                                     else (
-                                        blue(f'"{head.next.data}"')
+                                        _blue(f'"{head.next.data}"')
                                         if len(head.next.data) > 1
                                         else f"{head.next.data}"
                                     )
                                 )
                             ),
-                            f"{yellow(bin(id(head.next)) if self._base == 2 else oct(id(head.next)) if self._base == 8 else id(head.next) if self._base == 10 else hex(id(head.next)))}",
+                            f"{_yellow(bin(id(head.next)) if self._base == 2 else oct(id(head.next)) if self._base == 8 else id(head.next) if self._base == 10 else hex(id(head.next)))}",
                         ]
                     )
-                    head: object | None = head.next
+                    head: singlyLinkedListNode | None = head.next
                     while head and head.next != self._head:
                         first: str = (
                             f"{(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))}"
                         )
                         second: str = (
                             f"{bin(id(head.next)) if self._base == 2 else oct(id(head.next)) if self._base == 8 else id(head.next) if self._base == 10 else hex(id(head.next))}"
                             + (" " if head.next is None else "")
                         )
                         try:
                             after: str = (
-                                blue(f"{head.next.data}")
+                                _blue(f"{head.next.data}")
                                 if not isinstance(head.next.data, str)
                                 else (
-                                    blue(f"'{head.next.data}'")
+                                    _blue(f"'{head.next.data}'")
                                     if len(head.next.data) == 1
                                     else (
-                                        blue(f'"{head.next.data}"')
+                                        _blue(f'"{head.next.data}"')
                                         if len(head.next.data) > 1
                                         else f"{head.next.data}"
                                     )
                                 )
                             )
-                        except AttributeError as e7:
+                        except AttributeError as e4:
                             after: str = (
-                                f"{blue('None')} {green('(')}{red('NULL')}{green(')')}"
+                                f"{_blue('None')} {_green('(')}{_red('NULL')}{_green(')')}"
                             )
                         linked_list.append(
                             [
                                 (
-                                    blue(f"{head.data}")
+                                    _blue(f"{head.data}")
                                     if not isinstance(head.data, str)
                                     else (
-                                        blue(f"'{head.data}'")
+                                        _blue(f"'{head.data}'")
                                         if len(head.data) == 1
                                         else (
-                                            blue(f'"{head.data}"')
+                                            _blue(f'"{head.data}"')
                                             if len(head.data) > 1
                                             else f"{head.data}"
                                         )
                                     )
                                 ),
-                                yellow(first) if counter % 2 == 0 else red(first),
+                                _yellow(first) if counter % 2 == 0 else _red(first),
                                 after,
                                 (
                                     (
-                                        red(second)
-                                        + white("(")
-                                        + green("nil")
-                                        + white("/")
+                                        _red(second)
+                                        + _white("(")
+                                        + _green("nil")
+                                        + _white("/")
                                         + (
-                                            green("0b0")
+                                            _green("0b0")
                                             if self._base == 2
                                             else (
-                                                green("0o0")
+                                                _green("0o0")
                                                 if self._base == 8
                                                 else (
-                                                    green("0")
+                                                    _green("0")
                                                     if self._base == 10
-                                                    else green("0x0")
+                                                    else _green("0x0")
                                                 )
                                             )
                                         )
-                                        + white(")")
+                                        + _white(")")
                                         if second.endswith(" ")
-                                        else red(second)
+                                        else _red(second)
                                     )
                                     if counter % 2 == 0
                                     else (
-                                        yellow(second)
-                                        + white("(")
-                                        + red("nil")
-                                        + white("/")
+                                        _yellow(second)
+                                        + _white("(")
+                                        + _red("nil")
+                                        + _white("/")
                                         + (
-                                            red("0b0")
+                                            _red("0b0")
                                             if self._base == 2
                                             else (
-                                                red("0o0")
+                                                _red("0o0")
                                                 if self._base == 8
                                                 else (
-                                                    red("0")
+                                                    _red("0")
                                                     if self._base == 10
-                                                    else red("0x0")
+                                                    else _red("0x0")
                                                 )
                                             )
                                         )
-                                        + white(")")
+                                        + _white(")")
                                         if second.endswith(" ")
-                                        else yellow(second)
+                                        else _yellow(second)
                                     )
                                 ),
                             ]
                         )
                         counter += 1
-                        head: object | None = head.next
+                        head: singlyLinkedListNode | None = head.next
                     if self.circular:
                         first: str = (
                             f"{(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))}"
                         )
                         second: str = (
                             f"{bin(id(head.next)) if self._base == 2 else oct(id(head.next)) if self._base == 8 else id(head.next) if self._base == 10 else hex(id(head.next))}"
                         )
                         linked_list.append(
                             [
                                 (
-                                    blue(f"{head.data}")
+                                    _blue(f"{head.data}")
                                     if not isinstance(head.data, str)
                                     else (
-                                        blue(f"'{head.data}'")
+                                        _blue(f"'{head.data}'")
                                         if len(head.data) == 1
                                         else (
-                                            blue(f'"{head.data}"')
+                                            _blue(f'"{head.data}"')
                                             if len(head.data) > 1
                                             else f"{head.data}"
                                         )
                                     )
                                 ),
-                                yellow(first) if counter % 2 == 0 else red(first),
+                                _yellow(first) if counter % 2 == 0 else _red(first),
                                 (
-                                    blue(f"{head.next.data}")
+                                    _blue(f"{head.next.data}")
                                     if not isinstance(head.next.data, str)
                                     else (
-                                        blue(f"'{head.next.data}'")
+                                        _blue(f"'{head.next.data}'")
                                         if len(head.next.data) == 1
                                         else (
-                                            blue(f'"{head.next.data}"')
+                                            _blue(f'"{head.next.data}"')
                                             if len(head.next.data) > 1
                                             else f"{head.next.data}"
                                         )
                                     )
                                 ),
-                                cyan(second),
+                                _cyan(second),
                             ]
                         )
                 if not self.circular:
                     linked_list.append(
                         [
-                            f"{blue('None')} {green('(')}{red('NULL')}{green(')')}",
+                            f"{_blue('None')} {_green('(')}{_red('NULL')}{_green(')')}",
                             (
                                 (
-                                    f"{yellow(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))} "
-                                    + white("(")
-                                    + red("nil")
-                                    + white("/")
+                                    f"{_yellow(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))} "
+                                    + _white("(")
+                                    + _red("nil")
+                                    + _white("/")
                                     + (
-                                        red("0b0")
+                                        _red("0b0")
                                         if self._base == 2
                                         else (
-                                            red("0o0")
+                                            _red("0o0")
                                             if self._base == 8
                                             else (
-                                                red("0")
+                                                _red("0")
                                                 if self._base == 10
-                                                else red("0x0")
+                                                else _red("0x0")
                                             )
                                         )
                                     )
-                                    + white(")")
+                                    + _white(")")
                                 )
                                 if counter % 2 == 0
                                 else (
-                                    f"{red(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))} "
-                                    + white("(")
-                                    + green("nil")
-                                    + white("/")
+                                    f"{_red(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))} "
+                                    + _white("(")
+                                    + _green("nil")
+                                    + _white("/")
                                     + (
-                                        green("0b0")
+                                        _green("0b0")
                                         if self._base == 2
                                         else (
-                                            green("0o0")
+                                            _green("0o0")
                                             if self._base == 8
                                             else (
-                                                green("0")
+                                                _green("0")
                                                 if self._base == 10
-                                                else green("0x0")
+                                                else _green("0x0")
                                             )
                                         )
                                     )
-                                    + white(")")
+                                    + _white(")")
                                 )
                             ),
-                            BG_RED + " " * len("next value") + RESET,
-                            BG_RED + " " * len("next value @ddress") + RESET,
+                            _BG_RED + " " * len("next value") + _RESET,
+                            _BG_RED + " " * len("next value @ddress") + _RESET,
                         ]
                     )
                 return tabulate(linked_list, headers="firstrow", tablefmt="fancy_grid")
 
     def insert(
         self: "singlyLinkedList",
         index: int,
-        data: int | float | complex | str | list | tuple | set | dict | None,
+        data: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> None:
         """Insert object before index."""
         if not isinstance(index, int):
             raise TypeError("index must be an integer")
         if not self._head:
-            new_node: object = singlyLinkedListNode(data)
-            self._head: object = new_node
+            new_node: singlyLinkedListNode = singlyLinkedListNode(data)
+            self._head: singlyLinkedListNode = new_node
             self.len += 1
-            self._tail: object = new_node
+            self._tail: singlyLinkedListNode = new_node
             if self.circular:
                 self._head.next = self._head
         else:
             if index == 0:
-                new_node: object = singlyLinkedListNode(data)
+                new_node: singlyLinkedListNode = singlyLinkedListNode(data)
                 self.len += 1
                 new_node.next = self._head
                 if self.circular:
                     self._tail.next = new_node
                 self._head: object = new_node
             elif index >= self.len:
-                new_node: object = singlyLinkedListNode(data)
+                new_node: singlyLinkedListNode = singlyLinkedListNode(data)
                 self._tail.next = new_node
                 if self.circular:
                     new_node.next = self._head
                 self.len += 1
-                self._tail: object = new_node
+                self._tail: singlyLinkedListNode = new_node
             else:
                 if index < 0:
                     if index > -self.len:
                         index = self.len + index
                     else:
                         self.insert(0, data)
                         return
-                new_node: object = singlyLinkedListNode(data)
-                prev_head: object = self.node(index - 1)
+                new_node: singlyLinkedListNode = singlyLinkedListNode(data)
+                prev_head: singlyLinkedListNode = self.node(index - 1)
                 new_node.next = prev_head.next
                 prev_head.next = new_node
                 self.len += 1
 
     def pop(
         self: "singlyLinkedList", index: int = -1
-    ) -> int | float | complex | str | list | tuple | set | dict | None:
+    ) -> object | int | float | complex | str | list | tuple | set | dict | None | bool:
         """Remove and return item at index (default last).
 
         Raises IndexError if list is empty or index is out of range."""
         if not isinstance(index, int):
             raise TypeError("index must be an integer")
         if not self._head:
             if not self.circular:
                 raise IndexError("pop from empty non circular singly linked list")
             else:
                 raise IndexError("pop from empty circular singly linked list")
         else:
-            head: object = self._head
+            head: singlyLinkedListNode = self._head
             if index == 0 or index == -self.len:
                 old_head_value: (
-                    int | float | complex | str | list | tuple | set | dict | None
+                    object
+                    | int
+                    | float
+                    | complex
+                    | str
+                    | list
+                    | tuple
+                    | set
+                    | dict
+                    | None
+                    | bool
                 ) = self._head.data
-                old_head: object = self._head
+                old_head: singlyLinkedListNode = self._head
                 if not self.circular:
-                    self._head: object = head.next
+                    self._head: singlyLinkedListNode = head.next
                     if self.len == 1:
                         self._tail: None = None
                     self.len -= 1
                 else:
                     if self._head != head.next:
                         self._tail.next = head.next
-                        self._head: object = head.next
+                        self._head: singlyLinkedListNode = head.next
                     else:
                         self._head: None = None
                         self._tail: None = None
                     self.len -= 1
                 del old_head
                 return old_head_value
             elif index == -1 or index == self.len - 1:
-                prev_current: object = self.node(index - 1)
+                prev_current: singlyLinkedListNode = self.node(index - 1)
                 removed_node_value: (
-                    int | float | complex | str | list | tuple | set | dict | None
+                    object
+                    | int
+                    | float
+                    | complex
+                    | str
+                    | list
+                    | tuple
+                    | set
+                    | dict
+                    | None
+                    | bool
                 ) = prev_current.next.data
-                removed_node: object = prev_current.next
+                removed_node: singlyLinkedListNode = prev_current.next
                 if self.circular:
                     prev_current.next = self._head
                 else:
                     prev_current.next = None
                 self.len -= 1
-                self._tail: object = prev_current
+                self._tail: singlyLinkedListNode = prev_current
                 del removed_node
                 return removed_node_value
             elif index > self.len - 1 or index < -self.len:
                 raise IndexError("pop index out of range")
             else:
-                prev_node: object = self.node(index - 1)
+                prev_node: singlyLinkedListNode = self.node(index - 1)
                 removed_node_value: (
-                    int | float | complex | str | list | tuple | set | dict | None
+                    object
+                    | int
+                    | float
+                    | complex
+                    | str
+                    | list
+                    | tuple
+                    | set
+                    | dict
+                    | None
+                    | bool
                 ) = prev_node.next.data
-                removed_node: object = prev_node.next
+                removed_node: singlyLinkedListNode = prev_node.next
                 prev_node.next = prev_node.next.next
                 self.len -= 1
                 del removed_node
                 return removed_node_value
 
     def extend(
         self: "singlyLinkedList",
         extended_object: (
             singlyLinkedListNode
+            | object
             | int
             | float
             | complex
             | str
             | list
             | tuple
             | set
             | dict
             | None
+            | bool
         ),
     ) -> None:
         """Extend non circular/circular singly linked list by appending elements from the iterable."""
         if isinstance(extended_object, singlyLinkedList):
-            first_last_node: object | None = self._tail
-            second_first_node: object | None = extended_object._head
+            first_last_node: singlyLinkedListNode | None = self._tail
+            second_first_node: singlyLinkedListNode | None = extended_object._head
             for _ in range(extended_object.len):
-                new_node: object = singlyLinkedListNode(second_first_node.data)
+                new_node: singlyLinkedListNode = singlyLinkedListNode(
+                    second_first_node.data
+                )
                 first_last_node.next = new_node
-                first_last_node: object = first_last_node.next
-                second_first_node: object | None = second_first_node.next
+                first_last_node: singlyLinkedListNode = first_last_node.next
+                second_first_node: singlyLinkedListNode | None = second_first_node.next
             self.len += extended_object.len
             if self.circular:
                 first_last_node.next = self._head
         else:
-            extended_linked_list: object = singlyLinkedList(extended_object)
+            extended_linked_list: singlyLinkedList = singlyLinkedList(extended_object)
             self.extend(extended_linked_list)
 
     def __getitem__(
-        self: "linkedList", index: int
-    ) -> str | int | complex | float | list | tuple | set | dict | None:
+        self: "singlyLinkedList", index: int
+    ) -> (
+        object
+        | str
+        | int
+        | complex
+        | float
+        | list
+        | tuple
+        | set
+        | dict
+        | None
+        | bool
+        | object
+    ):
         if not isinstance(index, slice):
             return self.node(index).data
         else:
-            head: object | None = self._head
+            head: singlyLinkedListNode | None = self._head
             new_list: list = []
             for _ in range(self.len):
                 new_list.append(head.data)
-                head: object | None = head.next
+                head: singlyLinkedListNode | None = head.next
             try:
                 new_list: list = new_list[index.start : index.stop : index.step]
                 return singlyLinkedList(
                     new_list,
                     detail=self.detail,
                     circular=self.circular,
                     base=self._base,
                 )
-            except TypeError as e8:
+            except TypeError as e5:
                 pass
             raise TypeError(
                 "slice indices must be integers or None or have an __index__ method"
             )
 
-    def to_doubly(self: "singlyLinkedList") -> object:
+    def to_doubly(self: "singlyLinkedList") -> "doublyLinkedList":
         return doublyLinkedList() + self
 
     def add(
         self: "singlyLinkedList",
-        data: int | float | complex | str | list | tuple | set | dict | None,
+        data: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> None:
         """To add in an organized manner"""
         if not self._head:
             self._head: singlyLinkedListNode = singlyLinkedListNode(data)
             self.len += 1
-            self._tail = self._head
+            self._tail: singlyLinkedListNode = self._head
             if self.circular:
                 self._head.next = self._head
         else:
             head: singlyLinkedListNode = self._head
             prev_head: singlyLinkedListNode | None = None
             for i in range(self.len):
                 if type(head.data) != type(data):
@@ -1079,23 +1340,32 @@
                                 break
                         else:
                             prev_head: singlyLinkedListNode = head
                             head: singlyLinkedListNode = head.next
             else:
                 self.insert(self.len, data)
 
-    def to_dict(self: "linkedList", node: bool = False) -> dict:
-        head: object | None = self._head
+    def to_dict(self: "singlyLinkedList", node: bool = False) -> dict:
+        head: singlyLinkedListNode | None = self._head
         new_dict: dict = {}
         for _ in range(self.len):
             try:
                 next_value: (
-                    int | float | complex | str | list | tuple | set | dict | None
+                    int
+                    | float
+                    | complex
+                    | str
+                    | list
+                    | tuple
+                    | set
+                    | dict
+                    | None
+                    | bool
                 ) = head.next.data
-            except AttributeError as e9:
+            except AttributeError as e6:
                 next_value: None = None
             new_dict[head.data] = {
                 "current value @ddress" if not node else "current node": (
                     (
                         (
                             bin(id(head))
                             if self._base == 2
@@ -1124,140 +1394,148 @@
                             )
                         )
                     )
                     if not node
                     else head.next
                 ),
             }
-            head: object | None = head.next
+            head: singlyLinkedListNode | None = head.next
         return new_dict
 
+    def reverse(self: "singlyLinkedList") -> None:
+        head: singlyLinkedListNode | None = self._head
+        elements: list = []
+        for _ in range(self.len):
+            elements.append(head.data)
+            head: singlyLinkedListNode | None = head.next
+        head: singlyLinkedListNode | None = self._head
+        for i in range(1, self.len + 1):
+            head.data = elements[-i]
+            head: singlyLinkedListNode | None = head.next
+
 
 class sll(singlyLinkedList):
     pass
 
 
-class doublyLinkedListNode:
-    def __init__(
-        self: "doublyLinkedListNode",
-        data: int | float | complex | str | list | tuple | set | dict | None,
-    ) -> object:
-        self.data: int | float | complex | str | list | tuple | set | dict | None = data
-        self.prev: object | None = None
-        self.next: object | None = None
-
-    def get_data(
-        self: "doublyLinkedListNode",
-    ) -> int | float | complex | str | list | tuple | set | dict | None:
-        return self.data
-
-    def prev_node(self: "doublyLinkedListNode") -> object:
-        return self.prev
-
-    def next_node(self: "doublyLinkedListNode") -> object:
-        return self.next
-
-
-class doublyLinkedList(linkedList):
+class doublyLinkedList(_linkedList):
     @property
     def head(
-        self: "linkedList",
-    ) -> int | float | complex | str | list | tuple | set | dict | None:
-        try:
-            return self._head
-        except AttributeError as e10:
-            if not self.circular:
-                raise TypeError("Empty non circular doubly linked list")
-            else:
-                raise TypeError("Empty circular doubly linked list")
+        self: "doublyLinkedList",
+    ) -> doublyLinkedListNode:
+        return self._head
 
     @head.setter
     def head(
         self: "doublyLinkedList",
-        data: int | float | complex | str | list | tuple | set | dict | None,
+        data: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> None:
         self._head: None = None
         if isinstance(data, doublyLinkedList):
-            self._head: object | None = data._head
+            self._head: doublyLinkedListNode | None = data._head
         elif isinstance(data, doublyLinkedListNode):
-            old_head: object = data
-            old_self_head: object = data
-            new_head: object = doublyLinkedListNode(data.data)
+            old_head: doublyLinkedListNode = data
+            old_self_head: doublyLinkedListNode = data
+            new_head: doublyLinkedListNode = doublyLinkedListNode(data.data)
             if self.circular:
                 new_head.prev = data.prev
-            self._head: object = new_head
+            self._head: doublyLinkedListNode = new_head
             self.len += 1
-            old_head: object | None = old_head.next
+            old_head: doublyLinkedListNode | None = old_head.next
             while old_head and old_head != old_self_head:
-                new_node: object = doublyLinkedListNode(old_head.data)
+                new_node: doublyLinkedListNode = doublyLinkedListNode(old_head.data)
                 self.len += 1
                 new_head.next = new_node
                 new_node.prev = new_head
-                new_head: object | None = new_head.next
-                old_head: object | None = old_head.next
+                new_head: doublyLinkedListNode | None = new_head.next
+                old_head: doublyLinkedListNode | None = old_head.next
             if self.circular:
                 new_node.next = self._head
-            self._tail: object = new_node
+            self._tail: doublyLinkedListNode = new_node
         else:
             try:
                 if len(data) > 0:
                     for i in data:
                         self.append(i)
-            except TypeError as e11:
+            except TypeError as e7:
                 if data is not None:
-                    new_node: object = doublyLinkedListNode(data)
+                    new_node: doublyLinkedListNode = doublyLinkedListNode(data)
                     self.len += 1
-                    self._head: object = new_node
+                    self._head: doublyLinkedListNode = new_node
                     if self.circular:
                         new_node.next = new_node
                         new_node.prev = new_node
-                    self._tail: object = new_node
+                    self._tail: doublyLinkedListNode = new_node
 
     @head.deleter
     def head(self: "doublyLinkedList") -> None:
-        self._head = None
+        self._head: None = None
 
     def set_circular(self: "doublyLinkedList") -> None:
         self._tail.next = self._head
         self._head.prev = self._tail
         self.circular: bool = True
 
     def set_non_circular(self: "doublyLinkedList") -> None:
         self._tail.next = None
         self._head.prev = None
         self.circular: bool = False
 
     def __add__(
         self: "doublyLinkedList",
-        other: object | int | float | complex | str | list | tuple | set | dict | None,
+        other: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> None:
         helper: list = []
-        head1: object | None = self._head
+        head1: doublyLinkedListNode | None = self._head
         if isinstance(other, doublyLinkedList) or isinstance(other, singlyLinkedList):
-            head2: object | None = other._head
+            head2: doublyLinkedListNode | None = other._head
         else:
-            other: object = doublyLinkedList(other)
-            head2: object = other._head
+            other: doublyLinkedListNode = doublyLinkedList(other)
+            head2: doublyLinkedListNode = other._head
         for _ in range(self.len):
             helper.append(head1.data)
-            head1: object | None = head1.next
+            head1: doublyLinkedListNode | None = head1.next
         for _ in range(other.len):
             helper.append(head2.data)
-            head2: object | None = head2.next
+            head2: doublyLinkedListNode | None = head2.next
         return doublyLinkedList(helper, circular=other.circular)
 
     def __str__(self: "doublyLinkedList") -> str:
         """Return str(self)."""
         if not self._head:
             if not self.circular:
                 raise TypeError("Empty non circular doubly linked list")
             else:
                 raise TypeError("Empty circular doubly linked list")
         else:
-            head: object = self._head
+            head: doublyLinkedListNode = self._head
             linked_list: list = []
             counter: int = 0
             if not self.detail:
                 if not self.circular:
                     linked_list.append("None (NULL) <- ")
                 else:
                     linked_list.append("=> ")
@@ -1275,15 +1553,15 @@
                             linked_list.append(
                                 f"['{head.data}'] " + ("<=> " if head.next else "-> ")
                             )
                         else:
                             linked_list.append(
                                 f'["{head.data}"] ' + ("<=> " if head.next else "-> ")
                             )
-                    head = head.next
+                    head: doublyLinkedListNode | None = head.next
                 if not self.circular:
                     if self.len > 1:
                         linked_list.append("None (NULL)")
                     else:
                         try:
                             if not isinstance(head.data, str):
                                 linked_list.append(f"[{head.data}] -> None (NULL)")
@@ -1294,15 +1572,15 @@
                                     linked_list.append(
                                         f"['{head.data}'] -> None (NULL)"
                                     )
                                 else:
                                     linked_list.append(
                                         f'["{head.data}"] -> None (NULL)'
                                     )
-                        except AttributeError as e12:
+                        except AttributeError as e8:
                             linked_list.append("None (NULL)")
                 else:
                     if not isinstance(head.data, str):
                         linked_list.append(f"[{head.data}] <=")
                     else:
                         if len(head.data) == 0:
                             linked_list.append(f"[{head.data}] <=")
@@ -1310,554 +1588,640 @@
                             linked_list.append(f"['{head.data}'] <=")
                         else:
                             linked_list.append(f'["{head.data}"] <=')
                 return "".join(linked_list)
             else:
                 linked_list.append(
                     [
-                        white("previous value"),
-                        white("previous value ") + green("@") + white("ddress"),
-                        white("current value"),
-                        white("current value ") + green("@") + white("ddress"),
-                        white("next value"),
-                        white("next value ") + green("@") + white("ddress"),
+                        _white("previous value"),
+                        _white("previous value ") + _green("@") + _white("ddress"),
+                        _white("current value"),
+                        _white("current value ") + _green("@") + _white("ddress"),
+                        _white("next value"),
+                        _white("next value ") + _green("@") + _white("ddress"),
                     ]
                 )
                 if not self.circular:
                     linked_list.append(
                         [
-                            BG_RED + " " * len("previous value") + RESET,
-                            BG_RED + " " * len("previous value @ddress") + RESET,
-                            f"{blue('None')} {green('(')}{red('NULL')}{green(')')}",
-                            f"{yellow(bin(id(None)) if self._base == 2 else oct(id(None)) if self._base == 8 else id(None) if self._base == 10 else hex(id(None)))} "
-                            + white("(")
-                            + red("nil")
-                            + white("/")
+                            _BG_RED + " " * len("previous value") + _RESET,
+                            _BG_RED + " " * len("previous value @ddress") + _RESET,
+                            f"{_blue('None')} {_green('(')}{_red('NULL')}{_green(')')}",
+                            f"{_yellow(bin(id(None)) if self._base == 2 else oct(id(None)) if self._base == 8 else id(None) if self._base == 10 else hex(id(None)))} "
+                            + _white("(")
+                            + _red("nil")
+                            + _white("/")
                             + (
-                                red("0b0")
+                                _red("0b0")
                                 if self._base == 2
                                 else (
-                                    red("0o0")
+                                    _red("0o0")
                                     if self._base == 8
-                                    else (red("0") if self._base == 10 else red("0x0"))
+                                    else (
+                                        _red("0") if self._base == 10 else _red("0x0")
+                                    )
                                 )
                             )
-                            + white(")"),
-                            BG_RED + " " * len("next value") + RESET,
-                            BG_RED + " " * len("next value @ddress") + RESET,
+                            + _white(")"),
+                            _BG_RED + " " * len("next value") + _RESET,
+                            _BG_RED + " " * len("next value @ddress") + _RESET,
                         ]
                     )
                 try:
                     helper: (
-                        int | float | complex | str | list | tuple | set | dict | None
+                        object
+                        | int
+                        | float
+                        | complex
+                        | str
+                        | list
+                        | tuple
+                        | set
+                        | dict
+                        | None
+                        | bool
                     ) = head.next.data
-                except AttributeError as e13:
+                except AttributeError as e9:
                     helper: None = None
                 linked_list.append(
                     [
                         (
-                            f"{blue('None')} {green('(')}{red('NULL')}{green(')')}"
+                            f"{_blue('None')} {_green('(')}{_red('NULL')}{_green(')')}"
                             if not head.prev
                             else (
-                                blue(f"{head.prev.data}")
+                                _blue(f"{head.prev.data}")
                                 if not isinstance(head.prev.data, str)
                                 else (
-                                    blue(f"'{head.prev.data}'")
+                                    _blue(f"'{head.prev.data}'")
                                     if len(head.prev.data) == 1
                                     else (
-                                        blue(f'"{head.prev.data}"')
+                                        _blue(f'"{head.prev.data}"')
                                         if len(head.prev.data) > 1
                                         else f"{head.prev.data}"
                                     )
                                 )
                             )
                         ),
-                        f"{yellow(bin(id(head.prev)) if self._base == 2 else oct(id(head.prev)) if self._base == 8 else id(head.prev) if self._base == 10 else hex(id(head.prev)))} "
+                        f"{_yellow(bin(id(head.prev)) if self._base == 2 else oct(id(head.prev)) if self._base == 8 else id(head.prev) if self._base == 10 else hex(id(head.prev)))} "
                         + (
-                            white("(")
-                            + red("nil")
-                            + white("/")
+                            _white("(")
+                            + _red("nil")
+                            + _white("/")
                             + (
-                                red("0b0")
+                                _red("0b0")
                                 if self._base == 2
                                 else (
-                                    red("0o0")
+                                    _red("0o0")
                                     if self._base == 8
-                                    else (red("0") if self._base == 10 else red("0x0"))
+                                    else (
+                                        _red("0") if self._base == 10 else _red("0x0")
+                                    )
                                 )
                             )
-                            + white(")")
+                            + _white(")")
                             if head.prev is None
                             else ""
                         ),
                         (
-                            blue(f"{head.data}")
+                            _blue(f"{head.data}")
                             if not isinstance(head.data, str)
                             else (
-                                blue(f"'{head.data}'")
+                                _blue(f"'{head.data}'")
                                 if len(head.data) == 1
                                 else (
-                                    blue(f'"{head.data}"')
+                                    _blue(f'"{head.data}"')
                                     if len(head.data) > 1
                                     else f"{head.data}"
                                 )
                             )
                         ),
-                        f"{red(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))}",
+                        f"{_red(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))}",
                         (
-                            blue(
+                            _blue(
                                 f"{helper}"
-                                + f"{(green(' (') + red('NULL') + green(')')) if not helper else ''}"
+                                + f"{(_green(' (') + _red('NULL') + _green(')')) if not helper else ''}"
                             )
                             if not isinstance(helper, str)
                             else (
-                                blue(f"'{helper}'")
+                                _blue(f"'{helper}'")
                                 if len(head.next.data) == 1
                                 else (
-                                    blue(f'"{helper}"')
+                                    _blue(f'"{helper}"')
                                     if len(head.next.data) > 1
                                     else f"{helper}"
                                 )
                             )
                         ),
                         (
-                            f"{yellow(bin(id(head.next)) if self._base == 2 else oct(id(head.next)) if self._base == 8 else id(head.next) if self._base == 10 else hex(id(head.next)))} "
+                            f"{_yellow(bin(id(head.next)) if self._base == 2 else oct(id(head.next)) if self._base == 8 else id(head.next) if self._base == 10 else hex(id(head.next)))} "
                             + (
-                                white("(")
-                                + red("nil")
-                                + white("/")
+                                _white("(")
+                                + _red("nil")
+                                + _white("/")
                                 + (
-                                    red("0b0")
+                                    _red("0b0")
                                     if self._base == 2
                                     else (
-                                        red("0o0")
+                                        _red("0o0")
                                         if self._base == 8
                                         else (
-                                            red("0") if self._base == 10 else red("0x0")
+                                            _red("0")
+                                            if self._base == 10
+                                            else _red("0x0")
                                         )
                                     )
                                 )
-                                + white(")")
+                                + _white(")")
                                 if head.next is None
                                 else ""
                             )
                         ),
                     ]
                 )
-                head: object | None = head.next
+                head: doublyLinkedListNode | None = head.next
                 while head and head.next != self._head:
                     first: str = (
                         f"{bin(id(head.prev)) if self._base == 2 else oct(id(head.prev)) if self._base == 8 else id(head.prev) if self._base == 10 else hex(id(head.prev))}"
                     )
                     second: str = (
                         f"{(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))}"
                     )
                     last: str = (
                         f"{bin(id(head.next)) if self._base == 2 else oct(id(head.next)) if self._base == 8 else id(head.next) if self._base == 10 else hex(id(head.next))}"
                         + (" " if head.next is None else "")
                     )
                     try:
                         after: str = (
-                            blue(f"{head.next.data}")
+                            _blue(f"{head.next.data}")
                             if not isinstance(head.next.data, str)
                             else (
-                                blue(f"'{head.next.data}'")
+                                _blue(f"'{head.next.data}'")
                                 if len(head.next.data) == 1
                                 else (
-                                    blue(f'"{head.next.data}"')
+                                    _blue(f'"{head.next.data}"')
                                     if len(head.next.data) > 1
                                     else f"{head.next.data}"
                                 )
                             )
                         )
-                    except AttributeError as e14:
+                    except AttributeError as e10:
                         after: str = (
-                            f"{blue('None')} {green('(')}{red('NULL')}{green(')')}"
+                            f"{_blue('None')} {_green('(')}{_red('NULL')}{_green(')')}"
                         )
                     linked_list.append(
                         [
                             (
-                                blue(f"{head.prev.data}")
+                                _blue(f"{head.prev.data}")
                                 if not isinstance(head.prev.data, str)
                                 else (
-                                    blue(f"'{head.prev.data}'")
+                                    _blue(f"'{head.prev.data}'")
                                     if len(head.prev.data) == 1
                                     else (
-                                        blue(f'"{head.prev.data}"')
+                                        _blue(f'"{head.prev.data}"')
                                         if len(head.prev.data) > 1
                                         else f"{head.prev.data}"
                                     )
                                 )
                             ),
-                            red(first) if counter % 2 == 0 else yellow(first),
+                            _red(first) if counter % 2 == 0 else _yellow(first),
                             (
-                                blue(f"{head.data}")
+                                _blue(f"{head.data}")
                                 if not isinstance(head.data, str)
                                 else (
-                                    blue(f"'{head.data}'")
+                                    _blue(f"'{head.data}'")
                                     if len(head.data) == 1
                                     else (
-                                        blue(f'"{head.data}"')
+                                        _blue(f'"{head.data}"')
                                         if len(head.data) > 1
                                         else f"{head.data}"
                                     )
                                 )
                             ),
-                            yellow(second) if counter % 2 == 0 else red(second),
+                            _yellow(second) if counter % 2 == 0 else _red(second),
                             after,
                             (
                                 (
-                                    red(last)
-                                    + white("(")
-                                    + yellow("nil")
-                                    + white("/")
+                                    _red(last)
+                                    + _white("(")
+                                    + _yellow("nil")
+                                    + _white("/")
                                     + (
-                                        yellow("0b0")
+                                        _yellow("0b0")
                                         if self._base == 2
                                         else (
-                                            yellow("0o0")
+                                            _yellow("0o0")
                                             if self._base == 8
                                             else (
-                                                yellow("0")
+                                                _yellow("0")
                                                 if self._base == 10
-                                                else yellow("0x0")
+                                                else _yellow("0x0")
                                             )
                                         )
                                     )
-                                    + white(")")
+                                    + _white(")")
                                     if last.endswith(" ")
-                                    else red(last)
+                                    else _red(last)
                                 )
                                 if counter % 2 == 0
                                 else (
-                                    yellow(last)
-                                    + white("(")
-                                    + red("nil")
-                                    + white("/")
+                                    _yellow(last)
+                                    + _white("(")
+                                    + _red("nil")
+                                    + _white("/")
                                     + (
-                                        red("0b0")
+                                        _red("0b0")
                                         if self._base == 2
                                         else (
-                                            red("0o0")
+                                            _red("0o0")
                                             if self._base == 8
                                             else (
-                                                red("0")
+                                                _red("0")
                                                 if self._base == 10
-                                                else red("0x0")
+                                                else _red("0x0")
                                             )
                                         )
                                     )
-                                    + white(")")
+                                    + _white(")")
                                     if last.endswith(" ")
-                                    else yellow(last)
+                                    else _yellow(last)
                                 )
                             ),
                         ]
                     )
                     counter += 1
-                    head: object | None = head.next
+                    head: doublyLinkedListNode | None = head.next
                 if not self.circular:
                     linked_list.append(
                         [
-                            BG_RED + " " * len("previous value") + RESET,
-                            BG_RED + " " * len("previous value @ddress") + RESET,
-                            f"{blue('None')} {green('(')}{red('NULL')}{green(')')}",
+                            _BG_RED + " " * len("previous value") + _RESET,
+                            _BG_RED + " " * len("previous value @ddress") + _RESET,
+                            f"{_blue('None')} {_green('(')}{_red('NULL')}{_green(')')}",
                             (
-                                f"{yellow(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))} "
-                                + white("(")
-                                + red("nil")
-                                + white("/")
+                                f"{_yellow(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))} "
+                                + _white("(")
+                                + _red("nil")
+                                + _white("/")
                                 + (
-                                    red("0b0")
+                                    _red("0b0")
                                     if self._base == 2
                                     else (
-                                        red("0o0")
+                                        _red("0o0")
                                         if self._base == 8
                                         else (
-                                            red("0") if self._base == 10 else red("0x0")
+                                            _red("0")
+                                            if self._base == 10
+                                            else _red("0x0")
                                         )
                                     )
                                 )
-                                + white(")")
+                                + _white(")")
                                 if counter % 2 == 0
-                                else f"{red(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))} "
-                                + white("(")
-                                + yellow("nil")
-                                + white("/")
+                                else f"{_red(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))} "
+                                + _white("(")
+                                + _yellow("nil")
+                                + _white("/")
                                 + (
-                                    yellow("0b0")
+                                    _yellow("0b0")
                                     if self._base == 2
                                     else (
-                                        yellow("0o0")
+                                        _yellow("0o0")
                                         if self._base == 8
                                         else (
-                                            yellow("0")
+                                            _yellow("0")
                                             if self._base == 10
-                                            else yellow("0x0")
+                                            else _yellow("0x0")
                                         )
                                     )
                                 )
-                                + white(")")
+                                + _white(")")
                             ),
-                            BG_RED + " " * len("next value") + RESET,
-                            BG_RED + " " * len("next value @ddress") + RESET,
+                            _BG_RED + " " * len("next value") + _RESET,
+                            _BG_RED + " " * len("next value @ddress") + _RESET,
                         ]
                     )
                 else:
                     if self.len != 1:
                         first: str = (
                             f"{bin(id(head.prev)) if self._base == 2 else oct(id(head.prev)) if self._base == 8 else id(head.prev) if self._base == 10 else hex(id(head.prev))}"
                         )
                         second: str = (
                             f"{(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))}"
                         )
                         last: str = (
                             f"{bin(id(head.next)) if self._base == 2 else oct(id(head.next)) if self._base == 8 else id(head.next) if self._base == 10 else hex(id(head.next))}"
                         )
                         after: str = (
-                            blue(f"{head.next.data}")
+                            _blue(f"{head.next.data}")
                             if not isinstance(head.next.data, str)
                             else (
-                                blue(f"'{head.next.data}'")
+                                _blue(f"'{head.next.data}'")
                                 if len(head.next.data) == 1
                                 else (
-                                    blue(f'"{head.next.data}"')
+                                    _blue(f'"{head.next.data}"')
                                     if len(head.next.data) > 1
                                     else f"{head.next.data}"
                                 )
                             )
                         )
                         linked_list.append(
                             [
                                 (
-                                    blue(f"{head.prev.data}")
+                                    _blue(f"{head.prev.data}")
                                     if not isinstance(head.prev.data, str)
                                     else (
-                                        blue(f"'{head.prev.data}'")
+                                        _blue(f"'{head.prev.data}'")
                                         if len(head.prev.data) == 1
                                         else (
-                                            blue(f'"{head.prev.data}"')
+                                            _blue(f'"{head.prev.data}"')
                                             if len(head.prev.data) > 1
                                             else f"{head.prev.data}"
                                         )
                                     )
                                 ),
-                                red(first) if counter % 2 == 0 else yellow(first),
+                                _red(first) if counter % 2 == 0 else _yellow(first),
                                 (
-                                    blue(f"{head.data}")
+                                    _blue(f"{head.data}")
                                     if not isinstance(head.data, str)
                                     else (
-                                        blue(f"'{head.data}'")
+                                        _blue(f"'{head.data}'")
                                         if len(head.data) == 1
                                         else (
-                                            blue(f'"{head.data}"')
+                                            _blue(f'"{head.data}"')
                                             if len(head.data) > 1
                                             else f"{head.data}"
                                         )
                                     )
                                 ),
-                                yellow(second) if counter % 2 == 0 else red(second),
+                                _yellow(second) if counter % 2 == 0 else _red(second),
                                 after,
-                                red(last) if counter % 2 == 0 else yellow(last),
+                                _red(last) if counter % 2 == 0 else _yellow(last),
                             ]
                         )
                 return tabulate(linked_list, headers="firstrow", tablefmt="fancy_grid")
 
     def copy(self: "doublyLinkedList") -> "doublyLinkedList":
         """Return a shallow copy of a non circular/circular doubly linked list."""
         return doublyLinkedList(
             self._head,
             detail=self.detail,
             circular=self.circular,
             base=self._base,
         )
 
     def __getitem__(
-        self: "linkedList", index: int
-    ) -> str | int | complex | float | list | tuple | set | dict | None:
+        self: "doublyLinkedList", index: int
+    ) -> object | str | int | complex | float | list | tuple | set | dict | None | bool:
         if not isinstance(index, slice):
             return self.node(index).data
         else:
-            head: object | None = self._head
+            head: doublyLinkedListNode | None = self._head
             new_list: list = []
             for _ in range(self.len):
                 new_list.append(head.data)
-                head: object | None = head.next
+                head: doublyLinkedListNode | None = head.next
             try:
                 new_list: list = new_list[index.start : index.stop : index.step]
                 return doublyLinkedList(
                     new_list,
                     detail=self.detail,
                     circular=self.circular,
                     base=self._base,
                 )
-            except TypeError as e15:
+            except TypeError as e11:
                 pass
             raise TypeError(
                 "slice indices must be integers or None or have an __index__ method"
             )
 
     def insert(
         self: "doublyLinkedList",
         index: int,
-        data: int | float | complex | str | list | tuple | set | dict | None,
+        data: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> None:
         """Insert object before index."""
         if not isinstance(index, int):
             raise TypeError("index must be an integer")
         if not self._head:
-            new_node: object = doublyLinkedListNode(data)
-            self._head: object = new_node
-            self._tail: object = new_node
+            new_node: doublyLinkedListNode = doublyLinkedListNode(data)
+            self._head: doublyLinkedListNode = new_node
+            self._tail: doublyLinkedListNode = new_node
             self.len: int = 1
             if self.circular:
                 new_node.next = new_node
                 new_node.prev = new_node
         else:
             if index >= self.len:
-                new_node: object = doublyLinkedListNode(data)
+                new_node: doublyLinkedListNode = doublyLinkedListNode(data)
                 self._tail.next = new_node
                 new_node.prev = self._tail
-                self._tail: object = new_node
+                self._tail: doublyLinkedListNode = new_node
                 if self.circular:
                     self._tail.next = self._head
                     self._head.prev = self._tail
                 self.len += 1
             elif index <= -self.len or index == 0:
-                new_node: object = doublyLinkedListNode(data)
+                new_node: doublyLinkedListNode = doublyLinkedListNode(data)
                 new_node.next = self._head
                 self._head.prev = new_node
-                self._head: object = new_node
+                self._head: doublyLinkedListNode = new_node
                 if self.circular:
                     self._head.prev = self._tail
                     self._tail.next = self._head
                 self.len += 1
             else:
-                current: object = self.node(index)
-                new_node: object = doublyLinkedListNode(data)
+                current: doublyLinkedListNode = self.node(index)
+                new_node: doublyLinkedListNode = doublyLinkedListNode(data)
                 new_node.prev = current.prev
                 new_node.next = current
                 current.prev.next = new_node
                 current.prev = new_node
                 self.len += 1
 
     def pop(
         self: "doublyLinkedList", index: int = -1
-    ) -> int | float | complex | str | list | tuple | set | dict | None:
+    ) -> object | int | float | complex | str | list | tuple | set | dict | None | bool:
         """Remove and return item at index (default last).
 
         Raises IndexError if list is empty or index is out of range."""
         if not isinstance(index, int):
             raise TypeError("index must be an integer")
         if not self._head:
             if not self.circular:
                 raise IndexError("pop from empty non circular doubly linked list")
             else:
                 raise IndexError("pop from empty circular doubly linked list")
         else:
             if self.len > 1:
                 if index == -1 or index == self.len - 1:
                     returned_value: (
-                        int | float | complex | str | list | tuple | set | dict | None
+                        object
+                        | int
+                        | float
+                        | complex
+                        | str
+                        | list
+                        | tuple
+                        | set
+                        | dict
+                        | None
+                        | bool
                     ) = self._tail.data
-                    removed_node = self._tail
-                    self._tail: object = self._tail.prev
+                    removed_node: doublyLinkedListNode = self._tail
+                    self._tail: doublyLinkedListNode = self._tail.prev
                     if self.circular:
                         self._tail.next = self._head
                         self._head.prev = self._tail
                     else:
                         self._tail.next = None
                     self.len -= 1
                     del removed_node
                     return returned_value
                 elif index == 0 or index == -self.len:
                     returned_value: (
-                        int | float | complex | str | list | tuple | set | dict | None
+                        object
+                        | int
+                        | float
+                        | complex
+                        | str
+                        | list
+                        | tuple
+                        | set
+                        | dict
+                        | None
+                        | bool
                     ) = self._head.data
-                    removed_node = self._head
-                    self._head: object = self._head.next
+                    removed_node: doublyLinkedListNode = self._head
+                    self._head: doublyLinkedListNode = self._head.next
                     if self.circular:
                         self._head.prev = self._tail
                         self._tail.next = self._head
                     else:
                         self._head.prev = None
                     self.len -= 1
                     del removed_node
                     return returned_value
                 elif index >= self.len or index < -self.len:
                     raise IndexError("pop index out of range")
                 else:
-                    current: object = self.node(index)
+                    current: doublyLinkedListNode = self.node(index)
                     returned_value: (
-                        int | float | complex | str | list | tuple | set | dict | None
+                        object
+                        | int
+                        | float
+                        | complex
+                        | str
+                        | list
+                        | tuple
+                        | set
+                        | dict
+                        | None
+                        | bool
                     ) = current.data
                     current.prev.next = current.next
                     current.next.prev = current.prev
                     self.len -= 1
                     del current
                     return returned_value
             else:
                 if index == 0 or index == -1:
                     returned_value: (
-                        int | float | complex | str | list | tuple | set | dict | None
+                        object
+                        | int
+                        | float
+                        | complex
+                        | str
+                        | list
+                        | tuple
+                        | set
+                        | dict
+                        | None
+                        | bool
                     ) = self._head.data
-                    removed_node = self._head
+                    removed_node: doublyLinkedListNode = self._head
                     self._head: None = None
                     self._tail: None = None
                     self.len: int = 0
                     del removed_node
                     return returned_value
                 else:
                     raise IndexError("pop index out of range")
 
     def extend(
         self: "doublyLinkedList",
         extended_object: (
             doublyLinkedListNode
+            | object
             | int
             | float
             | complex
             | str
             | list
             | tuple
             | set
             | dict
             | None
+            | bool
         ),
     ) -> None:
         """Extend non circular/circular doubly linked list by appending elements from the iterable."""
         if isinstance(extended_object, doublyLinkedList):
-            first_last_node: object | None = self._tail
-            second_first_node: object | None = extended_object._head
+            first_last_node: doublyLinkedListNode | None = self._tail
+            second_first_node: doublyLinkedListNode | None = extended_object._head
             for _ in range(extended_object.len):
-                new_node: object = doublyLinkedListNode(second_first_node.data)
+                new_node: doublyLinkedListNode = doublyLinkedListNode(
+                    second_first_node.data
+                )
                 first_last_node.next = new_node
                 new_node.prev = first_last_node
-                first_last_node: object = first_last_node.next
-                second_first_node: object | None = second_first_node.next
+                first_last_node: doublyLinkedListNode = first_last_node.next
+                second_first_node: doublyLinkedListNode | None = second_first_node.next
             self.len += extended_object.len
             if self.circular:
                 first_last_node.next = self._head
                 self._head.prev = first_last_node
         else:
-            extended_linked_list: object = doublyLinkedList(extended_object)
+            extended_linked_list: doublyLinkedList = doublyLinkedList(extended_object)
             self.extend(extended_linked_list)
 
-    def to_singly(self: "doublyLinkedList") -> object:
+    def to_singly(self: "doublyLinkedList") -> singlyLinkedList:
         return singlyLinkedList() + self
 
     def add(
         self: "doublyLinkedList",
-        data: int | float | complex | str | list | tuple | set | dict | None,
+        data: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> None:
         """To add in an organized manner"""
         if not self._head:
             self._head: doublyLinkedListNode = doublyLinkedListNode(data)
             self.len += 1
-            self._tail = self._head
+            self._tail: doublyLinkedListNode = self._head
             if self.circular:
                 self._head.next = self._head
                 self._head.prev = self._head
         else:
             head: doublyLinkedListNode = self._head
             for i in range(self.len):
                 if type(head.data) != type(data):
@@ -1877,15 +2241,15 @@
                                 new_node.next = head
                                 new_node.prev = head.prev
                                 head.prev.next = new_node
                                 head.prev = new_node
                                 self.len += 1
                                 break
                         else:
-                            head = head.next
+                            head: doublyLinkedListNode | None = head.next
                     else:
                         if data > head.data:
                             if i == 0 or i == self.len - 1:
                                 self.insert(i, data)
                                 break
                             else:
                                 new_node: doublyLinkedListNode = doublyLinkedListNode(
@@ -1894,27 +2258,37 @@
                                 new_node.next = head
                                 new_node.prev = head.prev
                                 head.prev.next = new_node
                                 head.prev = new_node
                                 self.len += 1
                                 break
                         else:
-                            head = head.next
+                            head: doublyLinkedListNode | None = head.next
             else:
                 self.insert(self.len, data)
 
-    def to_dict(self: "linkedList", node: bool = False) -> dict:
-        head: object | None = self._head
+    def to_dict(self: "doublyLinkedList", node: bool = False) -> dict:
+        head: doublyLinkedListNode | None = self._head
         new_dict: dict = {}
         for _ in range(self.len):
             try:
                 next_value: (
-                    int | float | complex | str | list | tuple | set | dict | None
+                    object
+                    | int
+                    | float
+                    | complex
+                    | str
+                    | list
+                    | tuple
+                    | set
+                    | dict
+                    | None
+                    | bool
                 ) = head.next.data
-            except AttributeError as e16:
+            except AttributeError as e12:
                 next_value: None = None
             new_dict[head.data] = {
                 "prev value" if not node else "prev node value": (
                     (head.prev.data if head.prev is not None else None)
                     if not node
                     else head.prev.data if head.prev is not None else None
                 ),
@@ -1965,157 +2339,201 @@
                             )
                         )
                     )
                     if not node
                     else head.next
                 ),
             }
-            head: object | None = head.next
+            head: doublyLinkedListNode | None = head.next
         return new_dict
 
+    def reverse(self: "doublyLinkedList") -> None:
+        head: doublyLinkedListNode = self._head
+        tail: doublyLinkedListNode = self._tail
+        for _ in range(self.len // 2):
+            head.data, tail.data = tail.data, head.data
+            head: doublyLinkedListNode | None = head.next
+            tail: doublyLinkedListNode | None = tail.prev
+
 
 class dll(doublyLinkedList):
     pass
 
 
 class orthogonalLinkedListNode:
     def __init__(
         self: "orthogonalLinkedListNode",
-        data: int | float | complex | str | list | tuple | set | dict | None,
-    ) -> object:
-        self.prev = None
-        self.next = None
-        self.up = None
-        self.down = None
-        self.data = data
+        data: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
+    ) -> None:
+        self.prev: None = None
+        self.next: None = None
+        self.up: None = None
+        self.down: None = None
+        self.data: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ) = data
 
-    def prev_node(self: "orthogonalLinkedListNode") -> object:
+    def prev_node(self: "orthogonalLinkedListNode") -> "orthogonalLinkedListNode":
         return self.prev
 
-    def next_node(self: "orthogonalLinkedListNode") -> object:
+    def next_node(self: "orthogonalLinkedListNode") -> "orthogonalLinkedListNode":
         return self.next
 
-    def up_node(self: "orthogonalLinkedListNode") -> object:
+    def up_node(self: "orthogonalLinkedListNode") -> "orthogonalLinkedListNode":
         return self.up
 
-    def down_node(self: "orthogonalLinkedListNode") -> object:
+    def down_node(self: "orthogonalLinkedListNode") -> "orthogonalLinkedListNode":
         return self.down
 
     def get_data(
         self: "orthogonalLinkedListNode",
-    ) -> int | float | complex | str | list | tuple | set | dict | None:
+    ) -> object | int | float | complex | str | list | tuple | set | dict | None | bool:
         return self.data
 
 
 class orthogonalLinkedList:
     def __init__(
         self: "orthogonalLinkedList",
         data: list,
         *,
         circular: bool = False,
         detail: bool = False,
     ) -> None:
-        self.circular = circular
-        self.detail = detail
-        self.head = data
+        self.circular: bool = circular
+        self.detail: bool = detail
+        self.head: list = data
 
     @property
     def tail(
         self: "orthogonalLinkedList",
-    ) -> int | float | complex | str | list | tuple | set | dict | None:
+    ) -> orthogonalLinkedListNode:
         return self._head[-1][-1]
 
     def __len__(self: "orthogonalLinkedList") -> int:
         return len(self._head) * len(self._head[0])
 
     @property
     def shape(self: "orthogonalLinkedList") -> tuple[int, int]:
         return (len(self._head), len(self._head[0]))
 
-    def __getitem__(self, index):
-        values = []
+    def __getitem__(self: "orthogonalLinkedList", index: int):
+        values: list = []
         for i in range(len(self._head[index])):
             values.append(self._head[index][i].data)
         return values
 
     def __setitem__(
         self: "orthogonalLinkedList",
         index: int,
-        value: int | float | complex | str | list | tuple | set | dict | None,
+        value: (
+            object
+            | int
+            | float
+            | complex
+            | str
+            | list
+            | tuple
+            | set
+            | dict
+            | None
+            | bool
+        ),
     ) -> None:
         if len(value) == len(self._head[index]):
             for i in range(len(self._head[index])):
                 self._head[index][i].data = value[i]
         else:
             raise TypeError("columns len not the same")
 
     @property
     def head(
         self: "orthogonalLinkedList",
-    ) -> int | float | complex | str | list | tuple | set | dict | None:
+    ) -> orthogonalLinkedListNode:
         return self._head[0][0]
 
     @head.setter
     def head(self: "orthogonalLinkedList", data: list) -> None:
         if isinstance(data, list):
-            som = 0
+            som: int = 0
             for i in range(len(data)):
                 try:
                     som += len(data[i])
-                except TypeError as e17:
+                except TypeError as e13:
                     raise TypeError("just 2D array(list) allowed") from None
             if som % len(data):
                 raise TypeError("2D array(list) columns is not with the same length")
             else:
                 data[0][0] = orthogonalLinkedListNode(data[0][0])
                 for i in range(len(data)):
                     for j in range(len(data[i])):
                         if i == 0:
                             try:
                                 data[i][j + 1] = orthogonalLinkedListNode(
                                     data[i][j + 1]
                                 )
-                            except IndexError as e18:
+                            except IndexError as e14:
                                 pass
                         try:
                             data[i + 1][j] = orthogonalLinkedListNode(data[i + 1][j])
-                        except IndexError as e19:
+                        except IndexError as e15:
                             pass
                         if i == 0:
                             if j == 0:
                                 try:
                                     data[i][j].next = data[i][j + 1]
-                                except IndexError as e20:
+                                except IndexError as e16:
                                     pass
                             elif j == len(data[i]) - 1:
                                 data[i][j].prev = data[i][j - 1]
                             else:
                                 data[i][j].prev = data[i][j - 1]
                                 data[i][j].next = data[i][j + 1]
                             try:
                                 data[i][j].down = data[i + 1][j]
-                            except IndexError as e21:
+                            except IndexError as e17:
                                 pass
                         elif i == len(data) - 1:
                             if j == 0:
                                 try:
                                     data[i][j].next = data[i][j + 1]
-                                except IndexError as e22:
+                                except IndexError as e18:
                                     pass
                             elif j == len(data[i]) - 1:
                                 data[i][j].prev = data[i][j - 1]
                             else:
                                 data[i][j].prev = data[i][j - 1]
                                 data[i][j].next = data[i][j + 1]
                             data[i][j].up = data[i - 1][j]
                         else:
                             if j == 0:
                                 try:
                                     data[i][j].next = data[i][j + 1]
-                                except IndexError as e23:
+                                except IndexError as e19:
                                     pass
                             elif j == len(data[i]) - 1:
                                 data[i][j].prev = data[i][j - 1]
                             else:
                                 data[i][j].prev = data[i][j - 1]
                                 data[i][j].next = data[i][j + 1]
                             data[i][j].up = data[i - 1][j]
@@ -2127,26 +2545,26 @@
                                 data[i][j].prev = data[i][-1]
                             if data[i][j].next is None:
                                 data[i][j].next = data[i][0]
                             if data[i][j].up is None:
                                 data[i][j].up = data[-1][j]
                             if data[i][j].down is None:
                                 data[i][j].down = data[0][j]
-                self._head = data
+                self._head: list = data
         else:
             raise TypeError("just array(list) data type allowed")
 
     def __str__(self: "orthogonalLinkedList") -> str:
-        linked_list = []
+        linked_list: list = []
         if not self.detail:
             if not self.circular:
                 linked_list.append(["None"] * (len(self._head[0]) + 2))
                 linked_list[0][0], linked_list[0][-1] = "", ""
             for i in range(len(self._head)):
-                helper = []
+                helper: list = []
                 if not self.circular:
                     helper.append("None")
                 for j in range(len(self._head[i])):
                     if not isinstance(self._head[i][j].data, str):
                         helper.append(self._head[i][j].data)
                     else:
                         if len(self._head[i][j].data) == 0:
@@ -2159,140 +2577,152 @@
                     helper.append("None")
                 linked_list.append(helper)
             if not self.circular:
                 linked_list.append(["None"] * (len(self._head[0]) + 2))
                 linked_list[-1][0], linked_list[-1][-1] = "", ""
             return tabulate(linked_list, tablefmt="fancy_grid")
         else:
-            counter = 0
+            counter: int = 0
             linked_list.append(
                 [
-                    white("up"),
-                    white("up ") + green("@"),
-                    white("previous"),
-                    white("previous ") + green("@"),
-                    white("current"),
-                    white("current ") + green("@"),
-                    white("down"),
-                    white("down ") + green("@"),
-                    white("next"),
-                    white("next ") + green("@"),
+                    _white("up"),
+                    _white("up ") + _green("@"),
+                    _white("previous"),
+                    _white("previous ") + _green("@"),
+                    _white("current"),
+                    _white("current ") + _green("@"),
+                    _white("down"),
+                    _white("down ") + _green("@"),
+                    _white("next"),
+                    _white("next ") + _green("@"),
                 ]
             )
             for i in range(len(self._head)):
                 for j in range(len(self._head[i])):
                     try:
                         if not isinstance(self._head[i][j].prev.data, str):
-                            prev_data = blue(f"{self._head[i][j].prev.data}")
+                            prev_data: str = _blue(f"{self._head[i][j].prev.data}")
                         else:
                             if len(self._head[i][j].prev.data) == 0:
-                                prev_data = self._head[i][j].prev.data
+                                prev_data: str = self._head[i][j].prev.data
                             elif len(self._head[i][j].prev.data) == 1:
-                                prev_data = blue(f"'{self._head[i][j].prev.data}'")
+                                prev_data: str = _blue(
+                                    f"'{self._head[i][j].prev.data}'"
+                                )
                             else:
-                                prev_data = blue(f'"{self._head[i][j].prev.data}"')
-                    except AttributeError as e24:
-                        prev_data = blue("None")
+                                prev_data: str = _blue(
+                                    f'"{self._head[i][j].prev.data}"'
+                                )
+                    except AttributeError as e20:
+                        prev_data: str = _blue("None")
                     try:
                         if not isinstance(self._head[i][j].next.data, str):
-                            next_data = blue(f"{self._head[i][j].next.data}")
+                            next_data: str = _blue(f"{self._head[i][j].next.data}")
                         else:
                             if len(self._head[i][j].next.data) == 0:
-                                next_data = self._head[i][j].next.data
+                                next_data: str = self._head[i][j].next.data
                             elif len(self._head[i][j].next.data) == 1:
-                                next_data = blue(f"'{self._head[i][j].next.data}'")
+                                next_data: str = _blue(
+                                    f"'{self._head[i][j].next.data}'"
+                                )
                             else:
-                                next_data = blue(f'"{self._head[i][j].next.data}"')
-                    except AttributeError as e25:
-                        next_data = blue("None")
+                                next_data: str = _blue(
+                                    f'"{self._head[i][j].next.data}"'
+                                )
+                    except AttributeError as e21:
+                        next_data: str = _blue("None")
                     try:
                         if not isinstance(self._head[i][j].up.data, str):
-                            up_data = blue(f"{self._head[i][j].up.data}")
+                            up_data: str = _blue(f"{self._head[i][j].up.data}")
                         else:
                             if len(self._head[i][j].up.data) == 0:
-                                up_data = self._head[i][j].up.data
+                                up_data: str = self._head[i][j].up.data
                             elif len(self._head[i][j].up.data) == 1:
-                                up_data = blue(f"'{self._head[i][j].up.data}'")
+                                up_data: str = _blue(f"'{self._head[i][j].up.data}'")
                             else:
-                                up_data = blue(f'"{self._head[i][j].up.data}"')
-                    except AttributeError as e26:
-                        up_data = blue("None")
+                                up_data: str = _blue(f'"{self._head[i][j].up.data}"')
+                    except AttributeError as e22:
+                        up_data: str = _blue("None")
                     try:
                         if not isinstance(self._head[i][j].down.data, str):
-                            down_data = blue(f"{self._head[i][j].down.data}")
+                            down_data: str = _blue(f"{self._head[i][j].down.data}")
                         else:
                             if len(self._head[i][j].down.data) == 0:
-                                down_data = self._head[i][j].down.data
+                                down_data: str = self._head[i][j].down.data
                             elif len(self._head[i][j].down.data) == 1:
-                                down_data = blue(f"'{self._head[i][j].down.data}'")
+                                down_data: str = _blue(
+                                    f"'{self._head[i][j].down.data}'"
+                                )
                             else:
-                                down_data = blue(f'"{self._head[i][j].down.data}"')
-                    except AttributeError as e27:
-                        down_data = blue("None")
-                    current_data = (
-                        blue(f"{self._head[i][j].data}")
+                                down_data: str = _blue(
+                                    f'"{self._head[i][j].down.data}"'
+                                )
+                    except AttributeError as e23:
+                        down_data: str = _blue("None")
+                    current_data: str = (
+                        _blue(f"{self._head[i][j].data}")
                         if not isinstance(self._head[i][j].data, str)
                         else (
                             self._head[i][j].data
                             if len(self._head[i][j].data) == 0
                             else (
-                                blue(f"'{self._head[i][j].data}'")
+                                _blue(f"'{self._head[i][j].data}'")
                                 if len(self._head[i][j].data) == 1
-                                else blue(f'"{self._head[i][j].data}"')
+                                else _blue(f'"{self._head[i][j].data}"')
                             )
                         )
                     )
-                    up_add = (
+                    up_add: str = (
                         (
-                            yellow(f"{hex(id(self._head[i][j].up))}")
+                            _yellow(f"{hex(id(self._head[i][j].up))}")
                             if counter % 2 == 0
-                            else red(f"{hex(id(self._head[i][j].up))}")
+                            else _red(f"{hex(id(self._head[i][j].up))}")
                         )
                         if self._head[i][j].up is not None
-                        else cyan(f"{hex(id(self._head[i][j].up))}")
+                        else _cyan(f"{hex(id(self._head[i][j].up))}")
                     )
                     counter += 1
-                    prev_add = (
+                    prev_add: str = (
                         (
-                            yellow(f"{hex(id(self._head[i][j].prev))}")
+                            _yellow(f"{hex(id(self._head[i][j].prev))}")
                             if counter % 2 == 0
-                            else red(f"{hex(id(self._head[i][j].prev))}")
+                            else _red(f"{hex(id(self._head[i][j].prev))}")
                         )
                         if self._head[i][j].prev is not None
-                        else cyan(f"{hex(id(self._head[i][j].prev))}")
+                        else _cyan(f"{hex(id(self._head[i][j].prev))}")
                     )
                     counter += 1
-                    current_add = (
+                    current_add: str = (
                         (
-                            yellow(f"{hex(id(self._head[i][j]))}")
+                            _yellow(f"{hex(id(self._head[i][j]))}")
                             if counter % 2 == 0
-                            else red(f"{hex(id(self._head[i][j]))}")
+                            else _red(f"{hex(id(self._head[i][j]))}")
                         )
                         if self._head[i][j] is not None
-                        else cyan(f"{hex(id(self._head[i][j]))}")
+                        else _cyan(f"{hex(id(self._head[i][j]))}")
                     )
                     counter += 1
-                    down_add = (
+                    down_add: str = (
                         (
-                            yellow(f"{hex(id(self._head[i][j].down))}")
+                            _yellow(f"{hex(id(self._head[i][j].down))}")
                             if counter % 2 == 0
-                            else red(f"{hex(id(self._head[i][j].down))}")
+                            else _red(f"{hex(id(self._head[i][j].down))}")
                         )
                         if self._head[i][j].down is not None
-                        else cyan(f"{hex(id(self._head[i][j].down))}")
+                        else _cyan(f"{hex(id(self._head[i][j].down))}")
                     )
                     counter += 1
-                    next_add = (
+                    next_add: str = (
                         (
-                            yellow(f"{hex(id(self._head[i][j].next))}")
+                            _yellow(f"{hex(id(self._head[i][j].next))}")
                             if counter % 2 == 0
-                            else red(f"{hex(id(self._head[i][j].next))}")
+                            else _red(f"{hex(id(self._head[i][j].next))}")
                         )
                         if self._head[i][j].next is not None
-                        else cyan(f"{hex(id(self._head[i][j].next))}")
+                        else _cyan(f"{hex(id(self._head[i][j].next))}")
                     )
                     counter += 1
                     linked_list.append(
                         [
                             up_data,
                             up_add,
                             prev_data,
@@ -2312,13 +2742,13 @@
         return self._head
 
 
 class oll(orthogonalLinkedList):
     pass
 
 
-def main() -> None:
+def _main() -> None:
     print("linkedit")
 
 
 if __name__ == "__main__":
-    main()
+    _main()
```

### Comparing `linkedit-1.0.4/linkedit.egg-info/PKG-INFO` & `linkedit-1.0.5/linkedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedit
-Version: 1.0.4
+Version: 1.0.5
 Summary: Sophisticate Linked List
 Home-page: https://pypi.org/project/linkedit/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: linked list
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linkedit-1.0.4/setup.py` & `linkedit-1.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="linkedit",
-    version="1.0.4",
+    version="1.0.5",
     author="khiat Mohammed Abderrezzak",
     author_email="khiat.abderrezzak@gmail.com",
     license="MIT",
     description="Sophisticate Linked List",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/linkedit/",
```

