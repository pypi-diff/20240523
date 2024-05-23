# Comparing `tmp/lstack-1.0.2.tar.gz` & `tmp/lstack-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lstack-1.0.2.tar", last modified: Tue May 21 22:11:37 2024, max compression
+gzip compressed data, was "lstack-1.0.3.tar", last modified: Thu May 23 16:41:17 2024, max compression
```

## Comparing `lstack-1.0.2.tar` & `lstack-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-21 22:11:37.527879 lstack-1.0.2/
--rw-r--r--   0 khiat     (1000) khiat     (1000)     6166 2024-05-21 22:11:37.527879 lstack-1.0.2/PKG-INFO
--rw-rw-r--   0 khiat     (1000) khiat     (1000)     5728 2024-05-21 22:10:25.000000 lstack-1.0.2/README.md
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-21 22:11:37.527879 lstack-1.0.2/lstack/
--rw-r--r--   0 khiat     (1000) khiat     (1000)      244 2024-05-21 21:36:16.000000 lstack-1.0.2/lstack/__init__.py
--rw-r--r--   0 khiat     (1000) khiat     (1000)     7776 2024-05-21 21:36:34.000000 lstack-1.0.2/lstack/lstack.py
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-21 22:11:37.527879 lstack-1.0.2/lstack.egg-info/
--rw-r--r--   0 khiat     (1000) khiat     (1000)     6166 2024-05-21 22:11:37.000000 lstack-1.0.2/lstack.egg-info/PKG-INFO
--rw-r--r--   0 khiat     (1000) khiat     (1000)      203 2024-05-21 22:11:37.000000 lstack-1.0.2/lstack.egg-info/SOURCES.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-21 22:11:37.000000 lstack-1.0.2/lstack.egg-info/dependency_links.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       32 2024-05-21 22:11:37.000000 lstack-1.0.2/lstack.egg-info/requires.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        7 2024-05-21 22:11:37.000000 lstack-1.0.2/lstack.egg-info/top_level.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-21 22:11:37.527879 lstack-1.0.2/setup.cfg
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      732 2024-05-21 22:11:25.000000 lstack-1.0.2/setup.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 16:41:17.643939 lstack-1.0.3/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)     6166 2024-05-23 16:41:17.643939 lstack-1.0.3/PKG-INFO
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)     5728 2024-05-21 22:10:24.000000 lstack-1.0.3/README.md
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 16:41:17.639939 lstack-1.0.3/lstack/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)     8117 2024-05-23 16:36:35.000000 lstack-1.0.3/lstack/__init__.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 16:41:17.643939 lstack-1.0.3/lstack.egg-info/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)     6166 2024-05-23 16:41:17.000000 lstack-1.0.3/lstack.egg-info/PKG-INFO
+-rw-r--r--   0 khiat     (1000) khiat     (1000)      186 2024-05-23 16:41:17.000000 lstack-1.0.3/lstack.egg-info/SOURCES.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-23 16:41:17.000000 lstack-1.0.3/lstack.egg-info/dependency_links.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       32 2024-05-23 16:41:17.000000 lstack-1.0.3/lstack.egg-info/requires.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        7 2024-05-23 16:41:17.000000 lstack-1.0.3/lstack.egg-info/top_level.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-23 16:41:17.643939 lstack-1.0.3/setup.cfg
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      732 2024-05-23 16:40:32.000000 lstack-1.0.3/setup.py
```

### Comparing `lstack-1.0.2/PKG-INFO` & `lstack-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lstack
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sophisticate Stack
 Home-page: https://pypi.org/project/lstack/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: stack
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lstack-1.0.2/README.md` & `lstack-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lstack-1.0.2/lstack/lstack.py` & `lstack-1.0.3/lstack/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,33 +16,28 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Khiat Mohammed Abderrezzak <khiat.abderrezzak@gmail.com>
 
-"""Sophisticate Stack"""
-
-from linkedit import doublyLinkedList
-from tabulate import tabulate
-
 
-def red(text: str) -> str:
-    """Red Coloring Function"""
-    return "\033[91;1m{}\033[00m".format(text)
+"""Sophisticate Stack"""
 
 
-def green(text: str) -> str:
-    """Green Coloring Function"""
-    return "\033[92;1m{}\033[00m".format(text)
+__all__ = [
+    "linkedStack",
+    "CapacityError",
+    "StackOverflowError",
+    "StackUnderflowError",
+]
 
 
-def blue(text: str) -> str:
-    """Blue Coloring Function"""
-    return "\033[94;1m{}\033[00m".format(text)
+from linkedit import doublyLinkedList, _red, _green, _blue
+from tabulate import tabulate
 
 
 class CapacityError(BaseException):
     pass
 
 
 class StackOverflowError(BaseException):
@@ -54,15 +49,27 @@
 
 
 class linkedStack:
     """Stack Using Static Non Circular Doubly Linked List"""
 
     def __init__(
         self: "linkedStack",
-        data: int | float | complex | str | list | tuple | set | dict | None = None,
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
         capacity: int,
         detail: bool = False,
     ) -> None:
         self.capacity: int = capacity
         self.size: int = 0
         self.detail: bool = detail
@@ -86,15 +93,27 @@
     @property
     def stack(self: "linkedStack") -> doublyLinkedList:
         return self._stack
 
     @stack.setter
     def stack(
         self: "linkedStack",
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
         try:
             if len(data) > self._capacity:
                 raise CapacityError(
                     "Capacity must be greater than or equal the len of data"
                 )
             else:
@@ -115,15 +134,27 @@
             else:
                 self.stack: list = []
         except AttributeError as e2:
             self.pop_index: object = self._stack._tail
 
     def push(
         self: "linkedStack",
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
         if self.size != self._capacity:
             if data is not None:
                 self.push_index.data = data
                 self.size += 1
                 self.push_index: object | None = self.push_index.next
                 if self.pop_index is not None:
@@ -133,61 +164,61 @@
         else:
             raise StackOverflowError("Stack is full !")
 
     def pop(self: "linkedStack") -> None:
         if not self.size:
             raise StackUnderflowError("Stack is empty !")
         else:
-            returned_value: int | float | complex | str | list | tuple | set | dict = (
-                self.pop_index.data
-            )
+            returned_value: (
+                object | int | float | complex | str | list | tuple | set | dict | bool
+            ) = self.pop_index.data
             self.pop_index.data = None
             self.size -= 1
             self.pop_index: object | None = self.pop_index.prev
             if self.push_index is None:
                 self.push_index: object = self._stack._tail
             else:
                 self.push_index: object = self.push_index.prev
             return returned_value
 
     def __str__(self: "linkedStack") -> str:
         stack: list = []
         if self.detail:
             stack.append(
                 [
-                    green("ENTER")
-                    + red("  ^")
+                    _green("ENTER")
+                    + _red("  ^")
                     + "\n"
                     + " " * len("En")
-                    + green("|")
+                    + _green("|")
                     + " " * len("er  ")
-                    + red("|")
+                    + _red("|")
                     + "\n"
                     + " " * len("En")
-                    + green("v")
+                    + _green("v")
                     + " " * len("er ")
-                    + red("EXIT")
+                    + _red("EXIT")
                 ]
             )
             for _ in range(self._capacity - self.size):
                 stack.append([""])
             tracker: object = self.pop_index
         else:
             tracker: object = self._stack._head
         for _ in range(self.size):
             if self.detail:
                 if not isinstance(tracker.data, str):
-                    stack.append([blue(f"{tracker.data}")])
+                    stack.append([_blue(f"{tracker.data}")])
                 else:
                     if len(tracker.data) == 0:
                         stack.append([tracker.data])
                     elif len(tracker.data) == 1:
-                        stack.append([blue(f"'{tracker.data}'")])
+                        stack.append([_blue(f"'{tracker.data}'")])
                     else:
-                        stack.append([blue(f'"{tracker.data}"')])
+                        stack.append([_blue(f'"{tracker.data}"')])
                 tracker: object | None = tracker.prev
             else:
                 stack.append(tracker.data)
                 tracker: object | None = tracker.next
         if self.detail:
             return tabulate(stack, tablefmt="fancy_grid")
         else:
@@ -200,32 +231,32 @@
         return not self.size
 
     def isFull(self: "linkedStack") -> bool:
         return self.size == self._capacity
 
     def peek(
         self: "linkedStack",
-    ) -> int | float | complex | str | list | tuple | set | dict:
+    ) -> object | int | float | complex | str | list | tuple | set | dict | bool:
         if self.pop_index is not None:
             return self.pop_index.data
         else:
             raise StackUnderflowError("Stack is empty !")
 
     def top(
         self: "linkedStack",
-    ) -> int | float | complex | str | list | tuple | set | dict:
+    ) -> object | int | float | complex | str | list | tuple | set | dict | bool:
         return self.peek()
 
     def clear(self: "linkedStack") -> None:
         self._stack.clear()
         self._stack *= self._capacity
         self.push_index: object = self._stack._head
         self.pop_index: None = None
         self.size: int = 0
 
 
-def main() -> None:
+def _main() -> None:
     print("lstack")
 
 
 if __name__ == "__main__":
-    main()
+    _main()
```

### Comparing `lstack-1.0.2/lstack.egg-info/PKG-INFO` & `lstack-1.0.3/lstack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lstack
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sophisticate Stack
 Home-page: https://pypi.org/project/lstack/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: stack
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lstack-1.0.2/setup.py` & `lstack-1.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="lstack",
-    version="1.0.2",
+    version="1.0.3",
     author="khiat Mohammed Abderrezzak",
     author_email="khiat.abderrezzak@gmail.com",
     license="MIT",
     description="Sophisticate Stack",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/lstack/",
     packages=find_packages(),
     install_requires=[
         "tabulate>=0.9.0",
-        "linkedit>=1.0.4",
+        "linkedit>=1.0.5",
     ],
     keywords=[
         "stack",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

