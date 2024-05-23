# Comparing `tmp/cqueue-1.0.0.tar.gz` & `tmp/cqueue-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqueue-1.0.0.tar", last modified: Tue May 21 19:39:08 2024, max compression
+gzip compressed data, was "cqueue-1.0.1.tar", last modified: Thu May 23 16:40:15 2024, max compression
```

## Comparing `cqueue-1.0.0.tar` & `cqueue-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-21 19:39:08.627743 cqueue-1.0.0/
--rw-r--r--   0 khiat     (1000) khiat     (1000)     5404 2024-05-21 19:39:08.627743 cqueue-1.0.0/PKG-INFO
--rw-rw-r--   0 khiat     (1000) khiat     (1000)     4957 2024-05-21 19:29:06.000000 cqueue-1.0.0/README.md
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-21 19:39:08.623742 cqueue-1.0.0/cqueue/
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      309 2024-05-21 18:40:51.000000 cqueue-1.0.0/cqueue/__init__.py
--rw-r--r--   0 khiat     (1000) khiat     (1000)    12157 2024-05-21 18:14:16.000000 cqueue-1.0.0/cqueue/cqueue.py
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-21 19:39:08.627743 cqueue-1.0.0/cqueue.egg-info/
--rw-r--r--   0 khiat     (1000) khiat     (1000)     5404 2024-05-21 19:39:08.000000 cqueue-1.0.0/cqueue.egg-info/PKG-INFO
--rw-r--r--   0 khiat     (1000) khiat     (1000)      203 2024-05-21 19:39:08.000000 cqueue-1.0.0/cqueue.egg-info/SOURCES.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-21 19:39:08.000000 cqueue-1.0.0/cqueue.egg-info/dependency_links.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       32 2024-05-21 19:39:08.000000 cqueue-1.0.0/cqueue.egg-info/requires.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        7 2024-05-21 19:39:08.000000 cqueue-1.0.0/cqueue.egg-info/top_level.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-21 19:39:08.627743 cqueue-1.0.0/setup.cfg
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      741 2024-05-21 18:45:42.000000 cqueue-1.0.0/setup.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 16:40:15.595941 cqueue-1.0.1/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)     5404 2024-05-23 16:40:15.595941 cqueue-1.0.1/PKG-INFO
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)     4957 2024-05-21 19:29:06.000000 cqueue-1.0.1/README.md
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 16:40:15.591941 cqueue-1.0.1/cqueue/
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)    13075 2024-05-23 16:29:42.000000 cqueue-1.0.1/cqueue/__init__.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 16:40:15.595941 cqueue-1.0.1/cqueue.egg-info/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)     5404 2024-05-23 16:40:15.000000 cqueue-1.0.1/cqueue.egg-info/PKG-INFO
+-rw-r--r--   0 khiat     (1000) khiat     (1000)      186 2024-05-23 16:40:15.000000 cqueue-1.0.1/cqueue.egg-info/SOURCES.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-23 16:40:15.000000 cqueue-1.0.1/cqueue.egg-info/dependency_links.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       32 2024-05-23 16:40:15.000000 cqueue-1.0.1/cqueue.egg-info/requires.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        7 2024-05-23 16:40:15.000000 cqueue-1.0.1/cqueue.egg-info/top_level.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-23 16:40:15.595941 cqueue-1.0.1/setup.cfg
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      741 2024-05-23 16:39:23.000000 cqueue-1.0.1/setup.py
```

### Comparing `cqueue-1.0.0/PKG-INFO` & `cqueue-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqueue
-Version: 1.0.0
+Version: 1.0.1
 Summary: Sophisticate Circular Queue
 Home-page: https://pypi.org/project/cqueue/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: queue
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cqueue-1.0.0/README.md` & `cqueue-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cqueue-1.0.0/cqueue/cqueue.py` & `cqueue-1.0.1/cqueue/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,48 +16,44 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Khiat Mohammed Abderrezzak <khiat.abderrezzak@gmail.com>
 
-"""Sophisticate Circular Queue"""
-
-from linkedit import singlyLinkedList
-from tabulate import tabulate
-
 
-def red(text: str) -> str:
-    """Red Coloring Function"""
-    return "\033[91;1m{}\033[00m".format(text)
+"""Sophisticate Circular Queue"""
 
 
-def green(text: str) -> str:
-    """Green Coloring Function"""
-    return "\033[92;1m{}\033[00m".format(text)
+__all__ = [
+    "circularQueue",
+    "linkedCircularQueue",
+    "CapacityError",
+    "QueueOverflowError",
+    "QueueUnderflowError",
+]
 
 
-def blue(text: str) -> str:
-    """Blue Coloring Function"""
-    return "\033[94;1m{}\033[00m".format(text)
+from linkedit import singlyLinkedList, _red, _green, _blue
+from tabulate import tabulate
 
 
 class CapacityError(BaseException):
     pass
 
 
 class QueueOverflowError(BaseException):
     pass
 
 
 class QueueUnderflowError(BaseException):
     pass
 
 
-class capacity:
+class _capacity:
     def __init__(self: "capacity", capacity: int) -> None:
         self.capacity = capacity
 
     @property
     def capacity(self: "capacity") -> int:
         return self._capacity
 
@@ -69,20 +65,32 @@
             raise CapacityError("Capacity must ba positif integer !")
         elif capacity == 0:
             raise CapacityError("Capacity must be greater than zero !")
         else:
             self._capacity: int = capacity
 
 
-class circularQueue(capacity):
+class circularQueue(_capacity):
     """Circular Queue Using Static Array"""
 
     def __init__(
         self: "circularQueue",
-        data: int | float | complex | str | list | tuple | set | dict | None = [],
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
+        ) = [],
         *,
         capacity: int,
         detail: bool = False,
     ) -> None:
         super().__init__(capacity)
         self.size: int = 0
         self.detail: bool = detail
@@ -91,15 +99,27 @@
     @property
     def queue(self: "circularQueue") -> list:
         return self._queue
 
     @queue.setter
     def queue(
         self: "circularQueue",
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
         cqueue: list = []
         try:
             if self._capacity >= len(data):
                 for i in data:
                     if i is not None:
                         cqueue.append(i)
@@ -119,49 +139,61 @@
             if data is not None:
                 self.queue: list = [data]
             else:
                 self.queue: list = []
 
     def enqueue(
         self: "circularQueue",
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
         if data is not None:
             if self.queue[self.enqueue_index] is None:
                 self.queue[self.enqueue_index] = data
                 self.size += 1
                 self.enqueue_index: int = (self.enqueue_index + 1) % self._capacity
             else:
                 raise QueueOverflowError("Queue is full !")
 
     def dequeue(
         self: "circularQueue",
-    ) -> int | float | complex | str | list | set | tuple | dict:
+    ) -> object | int | float | complex | str | list | set | tuple | dict | bool:
         if self.queue[self.dequeue_index] is not None:
             returned_value: int | float | complex | str | list | tuple | set | dict = (
                 self.queue[self.dequeue_index]
             )
             self.queue[self.dequeue_index] = None
             self.dequeue_index: int = (self.dequeue_index + 1) % self._capacity
             self.size -= 1
             return returned_value
         else:
             raise QueueUnderflowError("Queue is empty !")
 
     def peek(
         self: "linkedCircularQueue",
-    ) -> int | float | complex | str | list | tuple | set | dict:
+    ) -> object | int | float | complex | str | list | tuple | set | dict | bool:
         if self._queue[self.dequeue_index] is not None:
             return self._queue[self.dequeue_index]
         else:
             raise QueueUnderflowError("Queue is Empty !")
 
     def top(
         self: "linkedCircularQueue",
-    ) -> int | float | complex | str | list | tuple | set | dict:
+    ) -> object | int | float | complex | str | list | tuple | set | dict | bool:
         return self.peek()
 
     def isEmpty(self: "circularQueue") -> bool:
         return not self.size
 
     def isFull(self: "circularQueue") -> bool:
         return self.size == self._capacity
@@ -174,46 +206,58 @@
 
     def __len__(self: "circularQueue") -> int:
         return self.size
 
     def __str__(self: "circularQueue") -> str:
         cqueue: list = [[] for _ in range(1) if self.detail]
         if self.detail:
-            cqueue[0].append(red("<- EXIT"))
+            cqueue[0].append(_red("<- EXIT"))
         tracker_index: int = self.dequeue_index
         for _ in range(self._capacity):
             if self.queue[tracker_index] is not None:
                 if not self.detail:
                     cqueue.append(self.queue[tracker_index])
                 else:
                     if isinstance(self.queue[tracker_index], str):
                         if len(self.queue[tracker_index]) == 0:
                             cqueue[0].append(self.queue[tracker_index])
                         elif len(self.queue[tracker_index]) == 1:
-                            cqueue[0].append(blue(f"'{self.queue[tracker_index]}'"))
+                            cqueue[0].append(_blue(f"'{self.queue[tracker_index]}'"))
                         else:
-                            cqueue[0].append(blue(f'"{self.queue[tracker_index]}"'))
+                            cqueue[0].append(_blue(f'"{self.queue[tracker_index]}"'))
                     else:
-                        cqueue[0].append(blue(f"{self.queue[tracker_index]}"))
+                        cqueue[0].append(_blue(f"{self.queue[tracker_index]}"))
             else:
                 if self.detail:
                     cqueue[0].append("")
             tracker_index: int = (tracker_index + 1) % self._capacity
         if self.detail:
-            cqueue[0].append(green("<- ENTER"))
+            cqueue[0].append(_green("<- ENTER"))
             return f"{tabulate(cqueue, tablefmt='fancy_grid')}"
         return f"{cqueue}"
 
 
-class linkedCircularQueue(capacity):
+class linkedCircularQueue(_capacity):
     """Circular Queue Using Static Circular Singly Linked List"""
 
     def __init__(
         self: "linkedCircularQueue",
-        data: int | float | complex | str | list | tuple | set | dict | None = [],
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
+        ) = [],
         *,
         capacity: int,
         detail: bool = False,
     ) -> None:
         super().__init__(capacity)
         self.size: int = 0
         self.detail: bool = detail
@@ -222,15 +266,27 @@
     @property
     def queue(self: "linkedCircularQueue") -> singlyLinkedList:
         return self._queue
 
     @queue.setter
     def queue(
         self: "linkedCircularQueue",
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
             if self._capacity >= len(data):
                 self._queue: singlyLinkedList = singlyLinkedList(
                     circular=True, detail=self.detail
                 )
                 for i in data:
@@ -251,49 +307,61 @@
             if data is not None:
                 self.queue: list = [data]
             else:
                 self.queue: list = []
 
     def enqueue(
         self: "linkedCircularQueue",
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
         if self.enqueue_index.data is None:
             if data is not None:
                 self.enqueue_index.data = data
                 self.enqueue_index: object = self.enqueue_index.next
                 self.size += 1
         else:
             raise QueueOverflowError("Queue is full !")
 
     def dequeue(
         self: "linkedCircularQueue",
-    ) -> int | float | complex | str | list | tuple | set | dict:
+    ) -> object | int | float | complex | str | list | tuple | set | dict | bool:
         if self.dequeue_index.data is not None:
-            returned_value: int | float | complex | str | list | tuple | set | dict = (
-                self.dequeue_index.data
-            )
+            returned_value: (
+                object | int | float | complex | str | list | tuple | set | dict | bool
+            ) = self.dequeue_index.data
             self.dequeue_index.data = None
             self.dequeue_index: object = self.dequeue_index.next
             self.size -= 1
             return returned_value
         else:
             raise QueueUnderflowError("Queue is empty !")
 
     def peek(
         self: "linkedCircularQueue",
-    ) -> int | float | complex | str | list | tuple | set | dict:
+    ) -> object | int | float | complex | str | list | tuple | set | dict | bool:
         if self.dequeue_index.data is not None:
             return self.dequeue_index.data
         else:
             raise QueueUnderflowError("Queue is empty !")
 
     def top(
         self: "linkedCircularQueue",
-    ) -> int | float | complex | str | list | tuple | set | dict:
+    ) -> object | int | float | complex | str | list | tuple | set | dict | bool:
         return self.peek()
 
     def isEmpty(self: "linkedCircularQueue") -> bool:
         return not self.size
 
     def isFull(self: "linkedCircularQueue") -> bool:
         return self.size == self._capacity
@@ -307,39 +375,39 @@
 
     def __len__(self: "linkedCircularQueue") -> int:
         return self.size
 
     def __str__(self: "linkedCircularQueue") -> str:
         cqueue: list = [[] for _ in range(1) if self.detail]
         if self.detail:
-            cqueue[0].append(red("<- EXIT"))
+            cqueue[0].append(_red("<- EXIT"))
         now: object = self.dequeue_index
         for _ in range(self._capacity):
             if self.detail:
                 if now.data is not None:
                     if isinstance(now.data, str):
                         if len(now.data) == 0:
                             cqueue[0].append(now.data)
                         elif len(now.data) == 1:
-                            cqueue[0].append(blue(f"'{now.data}'"))
+                            cqueue[0].append(_blue(f"'{now.data}'"))
                         else:
-                            cqueue[0].append(blue(f'"{now.data}"'))
+                            cqueue[0].append(_blue(f'"{now.data}"'))
                     else:
-                        cqueue[0].append(blue(f"{now.data}"))
+                        cqueue[0].append(_blue(f"{now.data}"))
                 else:
                     cqueue[0].append("")
             else:
                 if now.data is not None:
                     cqueue.append(now.data)
             now: object = now.next
         if self.detail:
-            cqueue[0].append(green("<- ENTER"))
+            cqueue[0].append(_green("<- ENTER"))
             return f"{tabulate(cqueue, tablefmt='fancy_grid')}"
         return f"{cqueue}"
 
 
-def main() -> None:
+def _main() -> None:
     print("cqueue")
 
 
 if __name__ == "__main__":
-    main()
+    _main()
```

### Comparing `cqueue-1.0.0/cqueue.egg-info/PKG-INFO` & `cqueue-1.0.1/cqueue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqueue
-Version: 1.0.0
+Version: 1.0.1
 Summary: Sophisticate Circular Queue
 Home-page: https://pypi.org/project/cqueue/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: queue
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cqueue-1.0.0/setup.py` & `cqueue-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cqueue",
-    version="1.0.0",
+    version="1.0.1",
     author="khiat Mohammed Abderrezzak",
     author_email="khiat.abderrezzak@gmail.com",
     license="MIT",
     description="Sophisticate Circular Queue",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/cqueue/",
     packages=find_packages(),
     install_requires=[
         "tabulate>=0.9.0",
-        "linkedit>=1.0.4",
+        "linkedit>=1.0.5",
     ],
     keywords=[
         "queue",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

